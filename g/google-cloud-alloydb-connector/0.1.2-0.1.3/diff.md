# Comparing `tmp/google-cloud-alloydb-connector-0.1.2.tar.gz` & `tmp/google-cloud-alloydb-connector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-connector-0.1.2.tar", last modified: Tue Jul 11 18:22:32 2023, max compression
+gzip compressed data, was "google-cloud-alloydb-connector-0.1.3.tar", last modified: Tue Aug  8 18:17:03 2023, max compression
```

## Comparing `google-cloud-alloydb-connector-0.1.2.tar` & `google-cloud-alloydb-connector-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/
--rw-rw-r--   0 root         (0)     1003    11357 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/LICENSE
--rw-r--r--   0 root         (0)     1003     9269 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     8401 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.806615 google-cloud-alloydb-connector-0.1.2/google/
--rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/
--rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/
--rw-rw-r--   0 root         (0)     1003      746 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/
--rw-rw-r--   0 root         (0)     1003      803 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     6271 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/client.py
--rw-rw-r--   0 root         (0)     1003     7945 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/connector.py
--rw-rw-r--   0 root         (0)     1003      616 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003     8388 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1970 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003     2764 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     4328 2023-07-11 18:19:38.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/refresh.py
--rw-rw-r--   0 root         (0)     1003     2713 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/
--rw-r--r--   0 root         (0)     1003     9269 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      926 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003       75 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-11 18:22:32.000000 google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-11 18:22:32.810615 google-cloud-alloydb-connector-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2519 2023-07-11 18:19:39.000000 google-cloud-alloydb-connector-0.1.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.105536 google-cloud-alloydb-connector-0.1.3/
+-rw-rw-r--   0 root         (0)     1003    11357 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/LICENSE
+-rw-r--r--   0 root         (0)     1003     9269 2023-08-08 18:17:03.105536 google-cloud-alloydb-connector-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     8401 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.101535 google-cloud-alloydb-connector-0.1.3/google/
+-rw-rw-r--   0 root         (0)     1003      746 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.101535 google-cloud-alloydb-connector-0.1.3/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      746 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.101535 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/
+-rw-rw-r--   0 root         (0)     1003      746 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.105536 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/
+-rw-rw-r--   0 root         (0)     1003      803 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6271 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/client.py
+-rw-rw-r--   0 root         (0)     1003     7945 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003      616 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     8388 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1970 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003     2764 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     4328 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/refresh.py
+-rw-rw-r--   0 root         (0)     1003     2713 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-08 18:17:03.105536 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003     9269 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      926 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003       75 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-08 18:17:03.000000 google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-08 18:17:03.105536 google-cloud-alloydb-connector-0.1.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2519 2023-08-08 18:14:22.000000 google-cloud-alloydb-connector-0.1.3/setup.py
```

### Comparing `google-cloud-alloydb-connector-0.1.2/LICENSE` & `google-cloud-alloydb-connector-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/PKG-INFO` & `google-cloud-alloydb-connector-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-connector-0.1.2/README.md` & `google-cloud-alloydb-connector-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/__init__.py` & `google-cloud-alloydb-connector-0.1.3/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/__init__.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/__init__.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/__init__.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/client.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/connector.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/connector.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/exceptions.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/instance.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/instance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/pg8000.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/rate_limiter.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/refresh.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/refresh.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/utils.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/google/cloud/alloydb/connector/version.py` & `google-cloud-alloydb-connector-0.1.3/google/cloud/alloydb/connector/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/PKG-INFO` & `google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-alloydb-connector-0.1.2/google_cloud_alloydb_connector.egg-info/SOURCES.txt` & `google-cloud-alloydb-connector-0.1.3/google_cloud_alloydb_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-0.1.2/setup.py` & `google-cloud-alloydb-connector-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,13 +65,13 @@
         "Programming Language :: Python :: 3.11",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     namespace_packages=namespaces,
     install_requires=core_dependencies,
     extras_require={
-        "pg8000": ["pg8000==1.29.8"],
+        "pg8000": ["pg8000==1.30.1"],
     },
     python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
 )
```


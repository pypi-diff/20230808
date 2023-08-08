# Comparing `tmp/macrometa-source-collection-0.0.57.tar.gz` & `tmp/macrometa-source-collection-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.57.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.58.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.57.tar` & `macrometa-source-collection-0.0.58.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11140 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    11991 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     4101 2023-08-08 03:18:14.647447 macrometa-source-collection-0.0.57/macrometa_source_collection/util.py
--rw-r--r--   0        0        0     1625 2023-08-08 03:18:14.891464 macrometa-source-collection-0.0.57/pyproject.toml
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.57/setup.py
--rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.57/PKG-INFO
+-rw-r--r--   0        0        0    11140 2023-08-08 08:04:02.830066 macrometa-source-collection-0.0.58/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    11991 2023-08-08 08:04:02.830066 macrometa-source-collection-0.0.58/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     4101 2023-08-08 08:04:02.830066 macrometa-source-collection-0.0.58/macrometa_source_collection/util.py
+-rw-r--r--   0        0        0     1625 2023-08-08 08:04:03.074069 macrometa-source-collection-0.0.58/pyproject.toml
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.58/setup.py
+-rw-r--r--   0        0        0     1159 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.58/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.57/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.58/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.57/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.58/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.57/macrometa_source_collection/util.py` & `macrometa-source-collection-0.0.58/macrometa_source_collection/util.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.57/pyproject.toml` & `macrometa-source-collection-0.0.58/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.57'
+version='0.0.58'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -25,15 +25,15 @@
 packages = [
     { include = "macrometa_source_collection" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = ">=0.0.24"
+c8connector = ">=0.0.30"
 chardet = "4.0.0"
 idna = "2.10"
 numpy = "1.21.6"
 pandas = "1.3.5"
 pyC8 = "1.0.1"
 requests = "2.25.1"
 websocket-client = "0.57.0"
```

### Comparing `macrometa-source-collection-0.0.57/setup.py` & `macrometa-source-collection-0.0.58/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 packages = \
 ['macrometa_source_collection']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector>=0.0.24',
+['c8connector>=0.0.30',
  'chardet==4.0.0',
  'idna==2.10',
  'numpy==1.21.6',
  'pandas==1.3.5',
  'pipelinewise-singer-python==1.2.0',
  'prometheus-client==0.16.0',
  'pulsar-client==2.10.1',
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.57',
+    'version': '0.0.58',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.57/PKG-INFO` & `macrometa-source-collection-0.0.58/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.57
+Version: 0.0.58
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: c8connector (>=0.0.24)
+Requires-Dist: c8connector (>=0.0.30)
 Requires-Dist: chardet (==4.0.0)
 Requires-Dist: idna (==2.10)
 Requires-Dist: numpy (==1.21.6)
 Requires-Dist: pandas (==1.3.5)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: prometheus-client (==0.16.0)
 Requires-Dist: pulsar-client (==2.10.1)
```


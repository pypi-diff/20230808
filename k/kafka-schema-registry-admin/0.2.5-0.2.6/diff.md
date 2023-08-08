# Comparing `tmp/kafka_schema_registry_admin-0.2.5.tar.gz` & `tmp/kafka_schema_registry_admin-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_schema_registry_admin-0.2.5.tar", max compression
+gzip compressed data, was "kafka_schema_registry_admin-0.2.6.tar", max compression
```

## Comparing `kafka_schema_registry_admin-0.2.5.tar` & `kafka_schema_registry_admin-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     7652 2022-06-27 09:02:38.500773 kafka_schema_registry_admin-0.2.5/LICENSE
--rw-r--r--   0        0        0      586 2022-06-27 09:02:38.501772 kafka_schema_registry_admin-0.2.5/README.rst
--rw-r--r--   0        0        0      239 2023-06-23 11:22:38.507808 kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/__init__.py
--rw-r--r--   0        0        0    14932 2023-06-23 11:22:39.091815 kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/kafka_schema_registry_admin.py
--rw-r--r--   0        0        0     1560 2023-06-23 11:22:38.507808 kafka_schema_registry_admin-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     7652 2022-06-27 09:02:38.500773 kafka_schema_registry_admin-0.2.6/LICENSE
+-rw-r--r--   0        0        0      586 2022-06-27 09:02:38.501772 kafka_schema_registry_admin-0.2.6/README.rst
+-rw-r--r--   0        0        0      239 2023-08-08 05:04:56.039282 kafka_schema_registry_admin-0.2.6/kafka_schema_registry_admin/__init__.py
+-rw-r--r--   0        0        0    14932 2023-06-23 11:22:39.091815 kafka_schema_registry_admin-0.2.6/kafka_schema_registry_admin/kafka_schema_registry_admin.py
+-rw-r--r--   0        0        0     1560 2023-08-08 05:04:56.039282 kafka_schema_registry_admin-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.2.6/PKG-INFO
```

### Comparing `kafka_schema_registry_admin-0.2.5/LICENSE` & `kafka_schema_registry_admin-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.2.5/README.rst` & `kafka_schema_registry_admin-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.2.5/kafka_schema_registry_admin/kafka_schema_registry_admin.py` & `kafka_schema_registry_admin-0.2.6/kafka_schema_registry_admin/kafka_schema_registry_admin.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.2.5/pyproject.toml` & `kafka_schema_registry_admin-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "kafka-schema-registry-admin"
-version = "0.2.5"
+version = "0.2.6"
 description = "Pure HTTP client to manage schemas in Schema Registry"
 authors = ["John Preston <john@ews-network.net>"]
 license = "LGPL-3.0-only"
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -36,15 +36,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_schema_registry_admin"
 
 [tool.tbump.version]
-current = "0.2.5"
+current = "0.2.6"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka_schema_registry_admin-0.2.5/PKG-INFO` & `kafka_schema_registry_admin-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-schema-registry-admin
-Version: 0.2.5
+Version: 0.2.6
 Summary: Pure HTTP client to manage schemas in Schema Registry
 License: LGPL-3.0-only
 Author: John Preston
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```


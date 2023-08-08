# Comparing `tmp/db_plugins-5.1.1a2.tar.gz` & `tmp/db_plugins-5.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_plugins-5.1.1a2.tar", max compression
+gzip compressed data, was "db_plugins-5.1.1a3.tar", max compression
```

## Comparing `db_plugins-5.1.1a2.tar` & `db_plugins-5.1.1a3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3482 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/README.rst
--rw-r--r--   0        0        0        0 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/cli/__init__.py
--rw-r--r--   0        0        0     2498 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/cli/manage.py
--rw-r--r--   0        0        0       40 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/__init__.py
--rw-r--r--   0        0        0     2012 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/generic.py
--rw-r--r--   0        0        0        0 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/__init__.py
--rw-r--r--   0        0        0     2748 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/_connection.py
--rw-r--r--   0        0        0        0 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/helpers/__init__.py
--rw-r--r--   0        0        0     2534 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/helpers/update_probs.py
--rw-r--r--   0        0        0      234 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/initialization.py
--rw-r--r--   0        0        0     6294 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/models.py
--rw-r--r--   0        0        0     2047 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/mongo/orm.py
--rw-r--r--   0        0        0        0 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/__init__.py
--rw-r--r--   0        0        0     1193 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/_connection.py
--rw-r--r--   0        0        0     2020 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/alembic.ini
--rw-r--r--   0        0        0      930 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/initialization.py
--rw-r--r--   0        0        0       38 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/migrations/README
--rw-r--r--   0        0        0     2472 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/migrations/env.py
--rw-r--r--   0        0        0      494 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/migrations/script.py.mako
--rwxr-xr-x   0        0        0    12920 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/db_plugins/db/sql/models.py
--rw-r--r--   0        0        0      569 2023-08-07 15:54:42.288100 db_plugins-5.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 db_plugins-5.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0     3482 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/README.rst
+-rw-r--r--   0        0        0        0 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/cli/__init__.py
+-rw-r--r--   0        0        0     2498 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/cli/manage.py
+-rw-r--r--   0        0        0       40 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/db/__init__.py
+-rw-r--r--   0        0        0     2012 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/db/generic.py
+-rw-r--r--   0        0        0        0 2023-08-08 16:23:52.809956 db_plugins-5.1.1a3/db_plugins/db/mongo/__init__.py
+-rw-r--r--   0        0        0     2748 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/_connection.py
+-rw-r--r--   0        0        0        0 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/helpers/__init__.py
+-rw-r--r--   0        0        0     2534 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/helpers/update_probs.py
+-rw-r--r--   0        0        0      234 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/initialization.py
+-rw-r--r--   0        0        0     6294 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/models.py
+-rw-r--r--   0        0        0     2047 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/mongo/orm.py
+-rw-r--r--   0        0        0        0 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/__init__.py
+-rw-r--r--   0        0        0     1193 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/_connection.py
+-rw-r--r--   0        0        0     2020 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/alembic.ini
+-rw-r--r--   0        0        0      930 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/initialization.py
+-rw-r--r--   0        0        0       38 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/migrations/README
+-rw-r--r--   0        0        0     2472 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/migrations/script.py.mako
+-rwxr-xr-x   0        0        0    12920 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/db_plugins/db/sql/models.py
+-rw-r--r--   0        0        0      569 2023-08-08 16:23:52.813957 db_plugins-5.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     4074 1970-01-01 00:00:00.000000 db_plugins-5.1.1a3/PKG-INFO
```

### Comparing `db_plugins-5.1.1a2/README.rst` & `db_plugins-5.1.1a3/README.rst`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/cli/manage.py` & `db_plugins-5.1.1a3/db_plugins/cli/manage.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/generic.py` & `db_plugins-5.1.1a3/db_plugins/db/generic.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/mongo/_connection.py` & `db_plugins-5.1.1a3/db_plugins/db/mongo/_connection.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/mongo/helpers/update_probs.py` & `db_plugins-5.1.1a3/db_plugins/db/mongo/helpers/update_probs.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/mongo/models.py` & `db_plugins-5.1.1a3/db_plugins/db/mongo/models.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/mongo/orm.py` & `db_plugins-5.1.1a3/db_plugins/db/mongo/orm.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/sql/_connection.py` & `db_plugins-5.1.1a3/db_plugins/db/sql/_connection.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/sql/alembic.ini` & `db_plugins-5.1.1a3/db_plugins/db/sql/alembic.ini`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/sql/initialization.py` & `db_plugins-5.1.1a3/db_plugins/db/sql/initialization.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/sql/migrations/env.py` & `db_plugins-5.1.1a3/db_plugins/db/sql/migrations/env.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/db_plugins/db/sql/models.py` & `db_plugins-5.1.1a3/db_plugins/db/sql/models.py`

 * *Files identical despite different names*

### Comparing `db_plugins-5.1.1a2/pyproject.toml` & `db_plugins-5.1.1a3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "db-plugins"
-version = "5.1.1a2"
+version = "5.1.1a3"
 description = "ALeRCE database plugins."
 authors = []
 readme = "README.rst"
 packages = [{include = "db_plugins"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7, <3.12"
```

### Comparing `db_plugins-5.1.1a2/PKG-INFO` & `db_plugins-5.1.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-plugins
-Version: 5.1.1a2
+Version: 5.1.1a3
 Summary: ALeRCE database plugins.
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


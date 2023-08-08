# Comparing `tmp/utils-flask-sqlalchemy-0.3.4.tar.gz` & `tmp/utils-flask-sqlalchemy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-flask-sqlalchemy-0.3.4.tar", last modified: Tue Jun  6 08:18:06 2023, max compression
+gzip compressed data, was "utils-flask-sqlalchemy-0.3.5.tar", last modified: Tue Aug  8 09:18:54 2023, max compression
```

## Comparing `utils-flask-sqlalchemy-0.3.4.tar` & `utils-flask-sqlalchemy-0.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.046748 utils-flask-sqlalchemy-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.050748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:18:06.054748 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 08:18:06.000000 utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 08:17:55.000000 utils-flask-sqlalchemy-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.165397 utils-flask-sqlalchemy-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.165397 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.165397 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24910 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:18:54.169396 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 09:18:54.000000 utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 09:18:44.000000 utils-flask-sqlalchemy-0.3.5/tox.ini
```

### Comparing `utils-flask-sqlalchemy-0.3.4/LICENSE` & `utils-flask-sqlalchemy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/PKG-INFO` & `utils-flask-sqlalchemy-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.4/README.md` & `utils-flask-sqlalchemy-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/setup.py` & `utils-flask-sqlalchemy-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/commands.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/commands.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/errors.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/errors.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/generic.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,14 @@
 
     def build_query_filters(self, query, parameters):
         """
         Construction des filtres
         """
         for f in parameters:
             query = self.build_query_filter(query, f, parameters.get(f))
-
         return query
 
     def build_query_filter(self, query, param_name, param_value):
         if param_name in self.view.tableDef.columns.keys():
             query = query.filter(self.view.tableDef.columns[param_name] == param_value)
 
         if param_name.startswith("ilike_"):
@@ -244,21 +243,20 @@
         - process_filter: application des filtres (et du sort)
         """
 
         q = self.DB.session.query(self.view.tableDef)
 
         if not process_filter:
             return q
-
         if self.filters:
             unordered_q = self.build_query_filters(q, self.filters)
             q = self.build_query_order(unordered_q, self.filters)
 
         if self.limit != -1:
-            q.limit(self.limit).offset(self.offset * self.limit)
+            q = q.limit(self.limit).offset(self.offset * self.limit)
 
         return q
 
     def query(self):
         """
         Lance la requete et retourne l'objet sqlalchemy
         """
```

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/utils.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/3842a6d800a0_sql_utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/migrations/versions/ba207b468e31_create_fr_numeric_collation.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/response.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/response.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/schema.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/schema.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/serializers.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/fixtures.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_schema.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/test_serializers.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/tests/utils.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/tests/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqla/utils.py` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqla/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/PKG-INFO` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python lib of tools for Flask and SQLAlchemy
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-0.3.4/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt` & `utils-flask-sqlalchemy-0.3.5/src/utils_flask_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/idbutils-1.0.7.tar.gz` & `tmp/idbutils-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbutils-1.0.7.tar", last modified: Sat Feb 25 12:58:09 2023, max compression
+gzip compressed data, was "idbutils-1.0.8.tar", last modified: Tue Aug  8 10:48:56 2023, max compression
```

## Comparing `idbutils-1.0.7.tar` & `idbutils-1.0.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:58:09.296481 idbutils-1.0.7/
--rw-r--r--   0 tgoetz     (501) staff       (20)    18092 2022-10-21 12:23:17.000000 idbutils-1.0.7/LICENSE
--rw-r--r--   0 tgoetz     (501) staff       (20)       24 2022-10-21 12:23:17.000000 idbutils-1.0.7/MANIFEST.in
--rw-r--r--   0 tgoetz     (501) staff       (20)      516 2023-02-25 12:58:09.296093 idbutils-1.0.7/PKG-INFO
--rw-r--r--   0 tgoetz     (501) staff       (20)       81 2022-10-21 12:23:17.000000 idbutils-1.0.7/README.md
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:58:09.293017 idbutils-1.0.7/idbutils/
--rw-r--r--   0 tgoetz     (501) staff       (20)     1005 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/__init__.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      338 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/conversions.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     3496 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/csv_importer.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     4537 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/db.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2391 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/db_attributes.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      545 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/db_exception.py
--rw-r--r--   0 tgoetz     (501) staff       (20)    40046 2023-02-25 12:44:43.000000 idbutils-1.0.7/idbutils/db_object.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1523 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/derived_enum.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2023 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/file_processor.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      963 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/json_config.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     5154 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/json_file_processor.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     3285 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/key_value.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1362 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/list_and_dict.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2156 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/location.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     1292 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/open_with_app.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     2169 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/plugin.py
--rw-r--r--   0 tgoetz     (501) staff       (20)     7571 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/rest_client.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      984 2022-10-21 12:23:17.000000 idbutils-1.0.7/idbutils/version.py
--rw-r--r--   0 tgoetz     (501) staff       (20)      350 2023-02-25 12:44:43.000000 idbutils-1.0.7/idbutils/version_info.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:58:09.294861 idbutils-1.0.7/idbutils.egg-info/
--rw-r--r--   0 tgoetz     (501) staff       (20)      516 2023-02-25 12:58:09.000000 idbutils-1.0.7/idbutils.egg-info/PKG-INFO
--rw-r--r--   0 tgoetz     (501) staff       (20)      701 2023-02-25 12:58:09.000000 idbutils-1.0.7/idbutils.egg-info/SOURCES.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)        1 2023-02-25 12:58:09.000000 idbutils-1.0.7/idbutils.egg-info/dependency_links.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)       41 2023-02-25 12:58:09.000000 idbutils-1.0.7/idbutils.egg-info/requires.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)        9 2023-02-25 12:58:09.000000 idbutils-1.0.7/idbutils.egg-info/top_level.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)      104 2022-10-21 12:23:17.000000 idbutils-1.0.7/pyproject.toml
--rw-r--r--   0 tgoetz     (501) staff       (20)       41 2022-10-21 12:23:17.000000 idbutils-1.0.7/requirements.txt
--rw-r--r--   0 tgoetz     (501) staff       (20)       38 2023-02-25 12:58:09.296561 idbutils-1.0.7/setup.cfg
--rw-r--r--   0 tgoetz     (501) staff       (20)     1750 2022-10-21 12:23:17.000000 idbutils-1.0.7/setup.py
-drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-02-25 12:58:09.295366 idbutils-1.0.7/test/
--rw-r--r--   0 tgoetz     (501) staff       (20)     2024 2022-10-21 12:23:17.000000 idbutils-1.0.7/test/test_db_object.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 10:48:56.250527 idbutils-1.0.8/
+-rw-r--r--   0 tgoetz     (501) staff       (20)    18092 2022-10-21 12:23:17.000000 idbutils-1.0.8/LICENSE
+-rw-r--r--   0 tgoetz     (501) staff       (20)       24 2022-10-21 12:23:17.000000 idbutils-1.0.8/MANIFEST.in
+-rw-r--r--   0 tgoetz     (501) staff       (20)      516 2023-08-08 10:48:56.250261 idbutils-1.0.8/PKG-INFO
+-rw-r--r--   0 tgoetz     (501) staff       (20)       81 2022-10-21 12:23:17.000000 idbutils-1.0.8/README.md
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 10:48:56.248185 idbutils-1.0.8/idbutils/
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1005 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/__init__.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      338 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/conversions.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     3496 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/csv_importer.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     4537 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/db.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2391 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/db_attributes.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      545 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/db_exception.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)    39861 2023-08-08 10:46:48.000000 idbutils-1.0.8/idbutils/db_object.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1523 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/derived_enum.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2023 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/file_processor.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      963 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/json_config.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     5154 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/json_file_processor.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     3285 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/key_value.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1362 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/list_and_dict.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2156 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/location.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1292 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/open_with_app.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2169 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/plugin.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)     7571 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/rest_client.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      984 2022-10-21 12:23:17.000000 idbutils-1.0.8/idbutils/version.py
+-rw-r--r--   0 tgoetz     (501) staff       (20)      350 2023-08-08 10:46:48.000000 idbutils-1.0.8/idbutils/version_info.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 10:48:56.249602 idbutils-1.0.8/idbutils.egg-info/
+-rw-r--r--   0 tgoetz     (501) staff       (20)      516 2023-08-08 10:48:56.000000 idbutils-1.0.8/idbutils.egg-info/PKG-INFO
+-rw-r--r--   0 tgoetz     (501) staff       (20)      701 2023-08-08 10:48:56.000000 idbutils-1.0.8/idbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)        1 2023-08-08 10:48:56.000000 idbutils-1.0.8/idbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)       41 2023-08-08 10:48:56.000000 idbutils-1.0.8/idbutils.egg-info/requires.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)        9 2023-08-08 10:48:56.000000 idbutils-1.0.8/idbutils.egg-info/top_level.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)      104 2022-10-21 12:23:17.000000 idbutils-1.0.8/pyproject.toml
+-rw-r--r--   0 tgoetz     (501) staff       (20)       41 2022-10-21 12:23:17.000000 idbutils-1.0.8/requirements.txt
+-rw-r--r--   0 tgoetz     (501) staff       (20)       38 2023-08-08 10:48:56.250613 idbutils-1.0.8/setup.cfg
+-rw-r--r--   0 tgoetz     (501) staff       (20)     1750 2022-10-21 12:23:17.000000 idbutils-1.0.8/setup.py
+drwxr-xr-x   0 tgoetz     (501) staff       (20)        0 2023-08-08 10:48:56.249908 idbutils-1.0.8/test/
+-rw-r--r--   0 tgoetz     (501) staff       (20)     2024 2022-10-21 12:23:17.000000 idbutils-1.0.8/test/test_db_object.py
```

### Comparing `idbutils-1.0.7/LICENSE` & `idbutils-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/PKG-INFO` & `idbutils-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utility library for writing database and internet apps.
 Home-page: https://github.com/tcgoetz/Fit
 Author: Tom Goetz
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `idbutils-1.0.7/idbutils/__init__.py` & `idbutils-1.0.8/idbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/csv_importer.py` & `idbutils-1.0.8/idbutils/csv_importer.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/db.py` & `idbutils-1.0.8/idbutils/db.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/db_attributes.py` & `idbutils-1.0.8/idbutils/db_attributes.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/db_exception.py` & `idbutils-1.0.8/idbutils/db_exception.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/db_object.py` & `idbutils-1.0.8/idbutils/db_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,18 +242,15 @@
         """Add values to the table."""
         with db.managed_session() as session:
             return session.add(cls(**values_dict))
 
     @classmethod
     def s_get(cls, session, instance_id, default=None):
         """Return a single instance for the given id."""
-        instance = session.query(cls).get(instance_id)
-        if instance is None:
-            return default
-        return instance
+        return session.get(cls, instance_id) or default
 
     @classmethod
     def get(cls, db, instance_id, default=None):
         """Return a single instance for the given id."""
         with db.managed_session() as session:
             return cls.s_get(session, instance_id, default)
 
@@ -395,33 +392,29 @@
         """Return all DB records in the table."""
         with db.managed_session() as session:
             return session.query(cls).all()
 
     @classmethod
     def s_get_for_period_where(cls, session, start_ts, end_ts, selectable=None, where=None):
         """Return all DB records matching the selection criteria."""
-        if selectable is None:
-            selectable = cls
-        query = cls._s_query(session, selectable, cls.time_col, start_ts, end_ts)
+        query = cls._s_query(session, selectable or cls, cls.time_col, start_ts, end_ts)
         if where is not None:
             query = query.filter(where)
         return query.all()
 
     @classmethod
     def get_for_period_where(cls, db, start_ts, end_ts, selectable=None, where=None):
         """Return all DB records matching the selection criteria."""
         with db.managed_session() as session:
             return cls.s_get_for_period_where(session, start_ts, end_ts, selectable, where)
 
     @classmethod
     def s_get_for_period(cls, session, start_ts, end_ts, selectable=None, not_none_col=None):
         """Return all DB records matching the selection criteria."""
-        if selectable is None:
-            selectable = cls
-        query = cls._s_query(session, selectable, cls.time_col, start_ts, end_ts)
+        query = cls._s_query(session, selectable or cls, cls.time_col, start_ts, end_ts)
         if not_none_col is not None:
             # filter does not use 'is not None'
             query = query.filter(not_none_col != None)  # noqa
         return query.all()
 
     @classmethod
     def get_for_period(cls, db, start_ts, end_ts, selectable=None, not_none_col=None):
```

### Comparing `idbutils-1.0.7/idbutils/derived_enum.py` & `idbutils-1.0.8/idbutils/derived_enum.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/file_processor.py` & `idbutils-1.0.8/idbutils/file_processor.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/json_config.py` & `idbutils-1.0.8/idbutils/json_config.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/json_file_processor.py` & `idbutils-1.0.8/idbutils/json_file_processor.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/key_value.py` & `idbutils-1.0.8/idbutils/key_value.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/list_and_dict.py` & `idbutils-1.0.8/idbutils/list_and_dict.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/location.py` & `idbutils-1.0.8/idbutils/location.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/open_with_app.py` & `idbutils-1.0.8/idbutils/open_with_app.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/plugin.py` & `idbutils-1.0.8/idbutils/plugin.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/rest_client.py` & `idbutils-1.0.8/idbutils/rest_client.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils/version.py` & `idbutils-1.0.8/idbutils/version.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/idbutils.egg-info/PKG-INFO` & `idbutils-1.0.8/idbutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbutils
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utility library for writing database and internet apps.
 Home-page: https://github.com/tcgoetz/Fit
 Author: Tom Goetz
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `idbutils-1.0.7/idbutils.egg-info/SOURCES.txt` & `idbutils-1.0.8/idbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/setup.py` & `idbutils-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `idbutils-1.0.7/test/test_db_object.py` & `idbutils-1.0.8/test/test_db_object.py`

 * *Files identical despite different names*


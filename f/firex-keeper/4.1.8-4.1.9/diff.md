# Comparing `tmp/firex_keeper-4.1.8.tar.gz` & `tmp/firex_keeper-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firex_keeper-4.1.8.tar", last modified: Wed Apr 14 17:45:07 2021, max compression
+gzip compressed data, was "dist/firex_keeper-4.1.9.tar", last modified: Wed Apr 14 19:45:29 2021, max compression
```

## Comparing `firex_keeper-4.1.8.tar` & `firex_keeper-4.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      104 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      560 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2434 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2858 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/db_model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1603 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/keeper_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1200 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/keeper_helper.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2134 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/keeper_launcher.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8157 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/persist.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8483 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/firex_keeper/task_query.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      581 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      160 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       20 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       13 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/firex_keeper.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      279 2021-04-14 17:45:07.000000 firex_keeper-4.1.8/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      928 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-04-14 17:44:53.000000 firex_keeper-4.1.8/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      104 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      560 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/firex_keeper/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2434 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/firex_keeper/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2858 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/db_model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1603 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/keeper_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1200 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/keeper_helper.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2036 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/keeper_launcher.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8157 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/persist.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8483 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/firex_keeper/task_query.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/firex_keeper.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      287 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      581 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      160 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       20 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       13 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2021-04-14 19:45:28.000000 firex_keeper-4.1.9/firex_keeper.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      279 2021-04-14 19:45:29.000000 firex_keeper-4.1.9/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      928 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2021-04-14 19:45:14.000000 firex_keeper-4.1.9/versioneer.py
```

### Comparing `firex_keeper-4.1.8/LICENSE` & `firex_keeper-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/README.md` & `firex_keeper-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/fastentrypoints.py` & `firex_keeper-4.1.9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/__main__.py` & `firex_keeper-4.1.9/firex_keeper/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/db_model.py` & `firex_keeper-4.1.9/firex_keeper/db_model.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/keeper_event_consumer.py` & `firex_keeper-4.1.9/firex_keeper/keeper_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/keeper_helper.py` & `firex_keeper-4.1.9/firex_keeper/keeper_helper.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/keeper_launcher.py` & `firex_keeper-4.1.9/firex_keeper/keeper_launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,13 @@
             logger.error("Failed to start FireXKeeper -- task DB will not be available.")
 
         return {}
 
     def ready_for_tasks(self, **kwargs) -> bool:
         return os.path.isfile(self.broker_recv_ready_file)
 
-    def get_version(self):
-        import firex_keeper
-        return firex_keeper.__version__
 
     def get_pkg_version_info(self) -> PkgVersionInfo:
         import firex_keeper
         return PkgVersionInfo(pkg=firex_keeper.__package__,
                               version=firex_keeper.__version__,
                               commit=firex_keeper._version.get_versions()['full-revisionid'])
```

### Comparing `firex_keeper-4.1.8/firex_keeper/persist.py` & `firex_keeper-4.1.9/firex_keeper/persist.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper/task_query.py` & `firex_keeper-4.1.9/firex_keeper/task_query.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/firex_keeper.egg-info/SOURCES.txt` & `firex_keeper-4.1.9/firex_keeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/setup.py` & `firex_keeper-4.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `firex_keeper-4.1.8/versioneer.py` & `firex_keeper-4.1.9/versioneer.py`

 * *Files identical despite different names*


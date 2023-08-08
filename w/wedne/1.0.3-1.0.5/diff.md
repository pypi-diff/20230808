# Comparing `tmp/wedne-1.0.3.tar.gz` & `tmp/wedne-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedne-1.0.3.tar", max compression
+gzip compressed data, was "wedne-1.0.5.tar", max compression
```

## Comparing `wedne-1.0.3.tar` & `wedne-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1463 2023-08-08 17:39:59.372075 wedne-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     4499 2023-08-08 17:45:10.592681 wedne-1.0.3/README.md
--rw-r--r--   0        0        0     1085 2023-08-08 18:48:09.774644 wedne-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-1.0.3/wedne/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-1.0.3/wedne/client/__init__.py
--rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-1.0.3/wedne/client/__main__.py
--rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-1.0.3/wedne/client/consts.py
--rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-1.0.3/wedne/client/shared_commands.py
--rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-1.0.3/wedne/client/telegram.py
--rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-1.0.3/wedne/client/watcher.py
--rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-1.0.3/wedne/commands.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-1.0.3/wedne/server/__init__.py
--rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-1.0.3/wedne/server/__main__.py
--rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-1.0.3/wedne/server/api/__init__.py
--rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-1.0.3/wedne/server/api/stats.py
--rw-r--r--   0        0        0      999 2023-08-08 14:44:51.556007 wedne-1.0.3/wedne/server/api/visits.py
--rw-r--r--   0        0        0     2259 2023-08-08 13:10:56.432165 wedne-1.0.3/wedne/server/db.py
--rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-1.0.3/wedne/server/settings.py
--rw-r--r--   0        0        0     1546 2023-08-08 18:47:08.190457 wedne-1.0.3/wedne/server/tasks.py
--rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-1.0.3/wedne/utils.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 wedne-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1463 2023-08-08 17:39:59.372075 wedne-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     4499 2023-08-08 17:45:10.592681 wedne-1.0.5/README.md
+-rw-r--r--   0        0        0     1085 2023-08-08 20:23:28.494168 wedne-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-1.0.5/wedne/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-1.0.5/wedne/client/__init__.py
+-rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-1.0.5/wedne/client/__main__.py
+-rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-1.0.5/wedne/client/consts.py
+-rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-1.0.5/wedne/client/shared_commands.py
+-rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-1.0.5/wedne/client/telegram.py
+-rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-1.0.5/wedne/client/watcher.py
+-rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-1.0.5/wedne/commands.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-1.0.5/wedne/server/__init__.py
+-rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-1.0.5/wedne/server/__main__.py
+-rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-1.0.5/wedne/server/api/__init__.py
+-rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-1.0.5/wedne/server/api/stats.py
+-rw-r--r--   0        0        0      999 2023-08-08 20:16:32.538473 wedne-1.0.5/wedne/server/api/visits.py
+-rw-r--r--   0        0        0     2307 2023-08-08 19:53:55.126368 wedne-1.0.5/wedne/server/db.py
+-rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-1.0.5/wedne/server/settings.py
+-rw-r--r--   0        0        0     1546 2023-08-08 20:17:18.076597 wedne-1.0.5/wedne/server/tasks.py
+-rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-1.0.5/wedne/utils.py
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 wedne-1.0.5/PKG-INFO
```

### Comparing `wedne-1.0.3/LICENSE.txt` & `wedne-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/README.md` & `wedne-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/pyproject.toml` & `wedne-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wedne"
-version = "1.0.3"
+version = "1.0.5"
 description = "Координируем строительство башни"
 authors = ["Oskar Sharipov"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/igoose1/wedne"
 
 [tool.poetry.dependencies]
```

### Comparing `wedne-1.0.3/wedne/client/__main__.py` & `wedne-1.0.5/wedne/client/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/client/shared_commands.py` & `wedne-1.0.5/wedne/client/shared_commands.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/client/telegram.py` & `wedne-1.0.5/wedne/client/telegram.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/client/watcher.py` & `wedne-1.0.5/wedne/client/watcher.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/server/__main__.py` & `wedne-1.0.5/wedne/server/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/server/api/stats.py` & `wedne-1.0.5/wedne/server/api/stats.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/wedne/server/api/visits.py` & `wedne-1.0.5/wedne/server/api/visits.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ) -> PreciseCommandSchema | None:
     now = datetime.now(pytz.utc)
     create_new_visit(
         time=now,
         social_media_id=data.social_media_id,
     )
     raw_command = dao.get_command(
-        from_=now - timedelta(seconds=settings.minutes_to_order),
+        from_=now - timedelta(minutes=settings.minutes_to_order),
         social_media_id=data.social_media_id,
     )
     if raw_command is None:
         return None
     command = CommandSchema.parse_obj(raw_command)
     return PreciseCommandSchema(
         expected_in=command.when - now,
```

### Comparing `wedne-1.0.3/wedne/server/db.py` & `wedne-1.0.5/wedne/server/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from typing import Any
 
 import peewee
 from playhouse.sqlite_ext import JSONField
 
 from wedne.server.settings import settings
 
-database = peewee.SqliteDatabase(settings.app_database, autoconnect=False)
+database = peewee.SqliteDatabase(
+    settings.app_database,
+    autoconnect=False,
+    pragmas={"journal_mode": "wal"},
+)
 
 
 class AutoFieldType(int, peewee.AutoField):
     pass
 
 
 class JSONFieldType(dict[Hashable, Any], JSONField):
```

### Comparing `wedne-1.0.3/wedne/server/tasks.py` & `wedne-1.0.5/wedne/server/tasks.py`

 * *Files identical despite different names*

### Comparing `wedne-1.0.3/PKG-INFO` & `wedne-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedne
-Version: 1.0.3
+Version: 1.0.5
 Summary: Координируем строительство башни
 Home-page: https://github.com/igoose1/wedne
 License: BSD-3-Clause
 Author: Oskar Sharipov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```


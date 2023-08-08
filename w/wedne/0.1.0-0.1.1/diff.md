# Comparing `tmp/wedne-0.1.0.tar.gz` & `tmp/wedne-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wedne-0.1.0.tar", max compression
+gzip compressed data, was "wedne-0.1.1.tar", max compression
```

## Comparing `wedne-0.1.0.tar` & `wedne-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        4 2023-08-08 13:10:56.332158 wedne-0.1.0/README.md
--rw-r--r--   0        0        0      950 2023-08-08 13:10:56.352160 wedne-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-0.1.0/wedne/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-0.1.0/wedne/client/__init__.py
--rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-0.1.0/wedne/client/__main__.py
--rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-0.1.0/wedne/client/consts.py
--rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-0.1.0/wedne/client/shared_commands.py
--rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-0.1.0/wedne/client/telegram.py
--rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-0.1.0/wedne/client/watcher.py
--rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-0.1.0/wedne/commands.py
--rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-0.1.0/wedne/server/__init__.py
--rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-0.1.0/wedne/server/__main__.py
--rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-0.1.0/wedne/server/api/__init__.py
--rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-0.1.0/wedne/server/api/stats.py
--rw-r--r--   0        0        0      999 2023-08-08 13:10:56.424164 wedne-0.1.0/wedne/server/api/visits.py
--rw-r--r--   0        0        0     2259 2023-08-08 13:10:56.432165 wedne-0.1.0/wedne/server/db.py
--rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-0.1.0/wedne/server/settings.py
--rw-r--r--   0        0        0     1542 2023-08-08 13:10:56.440165 wedne-0.1.0/wedne/server/tasks.py
--rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-0.1.0/wedne/utils.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 wedne-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2590 2023-08-08 14:45:44.084132 wedne-0.1.1/README.md
+-rw-r--r--   0        0        0      950 2023-08-08 14:45:31.748614 wedne-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.356160 wedne-0.1.1/wedne/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.360160 wedne-0.1.1/wedne/client/__init__.py
+-rw-r--r--   0        0        0     1203 2023-08-08 13:10:56.368161 wedne-0.1.1/wedne/client/__main__.py
+-rw-r--r--   0        0        0      338 2023-08-08 13:10:56.376161 wedne-0.1.1/wedne/client/consts.py
+-rw-r--r--   0        0        0      533 2023-08-08 13:10:56.380161 wedne-0.1.1/wedne/client/shared_commands.py
+-rw-r--r--   0        0        0     2802 2023-08-08 13:10:56.384162 wedne-0.1.1/wedne/client/telegram.py
+-rw-r--r--   0        0        0     1801 2023-08-08 13:10:56.392162 wedne-0.1.1/wedne/client/watcher.py
+-rw-r--r--   0        0        0      399 2023-08-08 13:10:56.396162 wedne-0.1.1/wedne/commands.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:10:56.404163 wedne-0.1.1/wedne/server/__init__.py
+-rw-r--r--   0        0        0     1178 2023-08-08 13:10:56.408163 wedne-0.1.1/wedne/server/__main__.py
+-rw-r--r--   0        0        0      186 2023-08-08 13:10:56.416164 wedne-0.1.1/wedne/server/api/__init__.py
+-rw-r--r--   0        0        0      759 2023-08-08 13:10:56.420164 wedne-0.1.1/wedne/server/api/stats.py
+-rw-r--r--   0        0        0      999 2023-08-08 14:44:51.556007 wedne-0.1.1/wedne/server/api/visits.py
+-rw-r--r--   0        0        0     2259 2023-08-08 13:10:56.432165 wedne-0.1.1/wedne/server/db.py
+-rw-r--r--   0        0        0      428 2023-08-08 13:10:56.436165 wedne-0.1.1/wedne/server/settings.py
+-rw-r--r--   0        0        0     1542 2023-08-08 13:10:56.440165 wedne-0.1.1/wedne/server/tasks.py
+-rw-r--r--   0        0        0      288 2023-08-08 13:10:56.448166 wedne-0.1.1/wedne/utils.py
+-rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 wedne-0.1.1/PKG-INFO
```

### Comparing `wedne-0.1.0/pyproject.toml` & `wedne-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wedne"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Oskar Sharipov"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = {extras = ["dotenv"], version = "^1.10.9"}
```

### Comparing `wedne-0.1.0/wedne/client/__main__.py` & `wedne-0.1.1/wedne/client/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/client/shared_commands.py` & `wedne-0.1.1/wedne/client/shared_commands.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/client/telegram.py` & `wedne-0.1.1/wedne/client/telegram.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/client/watcher.py` & `wedne-0.1.1/wedne/client/watcher.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/server/__main__.py` & `wedne-0.1.1/wedne/server/__main__.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/server/api/stats.py` & `wedne-0.1.1/wedne/server/api/stats.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/server/api/visits.py` & `wedne-0.1.1/wedne/server/api/visits.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ) -> PreciseCommandSchema | None:
     now = datetime.now(pytz.utc)
     create_new_visit(
         time=now,
         social_media_id=data.social_media_id,
     )
     raw_command = dao.get_command(
-        from_=now - timedelta(seconds=settings.seconds_of_delay),
+        from_=now - timedelta(seconds=settings.minutes_to_order),
         social_media_id=data.social_media_id,
     )
     if raw_command is None:
         return None
     command = CommandSchema.parse_obj(raw_command)
     return PreciseCommandSchema(
         expected_in=command.when - now,
```

### Comparing `wedne-0.1.0/wedne/server/db.py` & `wedne-0.1.1/wedne/server/db.py`

 * *Files identical despite different names*

### Comparing `wedne-0.1.0/wedne/server/tasks.py` & `wedne-0.1.1/wedne/server/tasks.py`

 * *Files identical despite different names*


# Comparing `tmp/kingspan_connect_sensor-3.0.0.tar.gz` & `tmp/kingspan_connect_sensor-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingspan_connect_sensor-3.0.0.tar", max compression
+gzip compressed data, was "kingspan_connect_sensor-3.0.1.tar", max compression
```

## Comparing `kingspan_connect_sensor-3.0.0.tar` & `kingspan_connect_sensor-3.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-3.0.0/LICENSE
--rw-r--r--   0        0        0     4033 2023-06-08 09:19:57.908283 kingspan_connect_sensor-3.0.0/README.md
--rw-r--r--   0        0        0     2187 2023-06-08 09:05:24.106065 kingspan_connect_sensor-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-3.0.0/src/connectsensor/__init__.py
--rw-r--r--   0        0        0     3570 2023-06-08 09:08:11.851107 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_export.py
--rw-r--r--   0        0        0     5736 2023-06-08 09:17:59.368334 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_notifier.py
--rw-r--r--   0        0        0     1825 2023-06-08 09:21:14.131699 kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_status.py
--rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-3.0.0/src/connectsensor/client.py
--rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-3.0.0/src/connectsensor/debug.py
--rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-3.0.0/src/connectsensor/exceptions.py
--rw-r--r--   0        0        0     3592 2023-06-08 08:37:38.261232 kingspan_connect_sensor-3.0.0/src/connectsensor/tank.py
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 kingspan_connect_sensor-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4033 2023-06-08 09:19:57.908283 kingspan_connect_sensor-3.0.1/README.md
+-rw-r--r--   0        0        0     2187 2023-08-08 11:42:19.173340 kingspan_connect_sensor-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-3.0.1/src/connectsensor/__init__.py
+-rw-r--r--   0        0        0     3570 2023-06-08 09:08:11.851107 kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_export.py
+-rw-r--r--   0        0        0     5736 2023-06-08 09:17:59.368334 kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_notifier.py
+-rw-r--r--   0        0        0     1825 2023-06-08 09:21:14.131699 kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_status.py
+-rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-3.0.1/src/connectsensor/client.py
+-rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-3.0.1/src/connectsensor/debug.py
+-rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-3.0.1/src/connectsensor/exceptions.py
+-rw-r--r--   0        0        0     3592 2023-06-08 08:37:38.261232 kingspan_connect_sensor-3.0.1/src/connectsensor/tank.py
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 kingspan_connect_sensor-3.0.1/PKG-INFO
```

### Comparing `kingspan_connect_sensor-3.0.0/LICENSE` & `kingspan_connect_sensor-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/README.md` & `kingspan_connect_sensor-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/pyproject.toml` & `kingspan_connect_sensor-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 description = "API to get oil tank from Kingspan SENSiT sensors"
 documentation = "https://github.com/masaccio/kingspan-connect-sensor/blob/main/README.md"
 license = "MIT"
 name = "kingspan-connect-sensor"
 packages = [{include = "connectsensor", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/kingspan-connect-sensor"
-version = "3.0.0"
+version = "3.0.1"
 
 [tool.poetry.dependencies]
 async-property = "^0.2.1"
 asyncio = "^3.4.3"
 datetime = "^4.7"
 httpx = "^0.24"
 python = "^3.9"
```

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_export.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_export.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_notifier.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_notifier.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/_kingspan_status.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/_kingspan_status.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/client.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/client.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/debug.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/debug.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/src/connectsensor/tank.py` & `kingspan_connect_sensor-3.0.1/src/connectsensor/tank.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-3.0.0/PKG-INFO` & `kingspan_connect_sensor-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingspan-connect-sensor
-Version: 3.0.0
+Version: 3.0.1
 Summary: API to get oil tank from Kingspan SENSiT sensors
 Home-page: https://github.com/masaccio/kingspan-connect-sensor
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


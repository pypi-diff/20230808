# Comparing `tmp/pyairstage-1.0.0.tar.gz` & `tmp/pyairstage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyairstage-1.0.0.tar", last modified: Tue Jul 11 08:38:02 2023, max compression
+gzip compressed data, was "pyairstage-1.0.1.tar", last modified: Tue Aug  8 12:00:13 2023, max compression
```

## Comparing `pyairstage-1.0.0.tar` & `pyairstage-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:02.583407 pyairstage-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 08:37:31.000000 pyairstage-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-11 08:38:02.583407 pyairstage-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 08:37:31.000000 pyairstage-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:02.583407 pyairstage-1.0.0/pyairstage/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 08:37:31.000000 pyairstage-1.0.0/pyairstage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-11 08:37:31.000000 pyairstage-1.0.0/pyairstage/airstageAC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-11 08:37:31.000000 pyairstage-1.0.0/pyairstage/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-11 08:37:31.000000 pyairstage-1.0.0/pyairstage/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:38:02.583407 pyairstage-1.0.0/pyairstage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-11 08:38:02.000000 pyairstage-1.0.0/pyairstage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 08:38:02.000000 pyairstage-1.0.0/pyairstage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:38:02.000000 pyairstage-1.0.0/pyairstage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 08:38:02.000000 pyairstage-1.0.0/pyairstage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 08:38:02.000000 pyairstage-1.0.0/pyairstage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 08:38:02.583407 pyairstage-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-11 08:37:31.000000 pyairstage-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:00:13.382130 pyairstage-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 11:59:39.000000 pyairstage-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 12:00:13.382130 pyairstage-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-08 11:59:39.000000 pyairstage-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:00:13.382130 pyairstage-1.0.1/pyairstage/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 11:59:39.000000 pyairstage-1.0.1/pyairstage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-08-08 11:59:39.000000 pyairstage-1.0.1/pyairstage/airstageAC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-08-08 11:59:39.000000 pyairstage-1.0.1/pyairstage/airstageApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-08 11:59:39.000000 pyairstage-1.0.1/pyairstage/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:00:13.382130 pyairstage-1.0.1/pyairstage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-08 12:00:13.000000 pyairstage-1.0.1/pyairstage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 12:00:13.000000 pyairstage-1.0.1/pyairstage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:00:13.000000 pyairstage-1.0.1/pyairstage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 12:00:13.000000 pyairstage-1.0.1/pyairstage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 12:00:13.000000 pyairstage-1.0.1/pyairstage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-08 12:00:13.382130 pyairstage-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-08 11:59:39.000000 pyairstage-1.0.1/setup.py
```

### Comparing `pyairstage-1.0.0/LICENSE` & `pyairstage-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyairstage-1.0.0/PKG-INFO` & `pyairstage-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairstage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to control Fujitsu Airstage Airconditioners
 Home-page: https://github.com/danielkaldheim/pyairstage
 Author: Daniel Rufus Kaldheim
 Author-email: daniel@kaldheim.org
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyairstage-1.0.0/pyairstage/airstageAC.py` & `pyairstage-1.0.1/pyairstage/airstageAC.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from .constants import *
-from .api import Api
+
+from .airstageApi import AirstageApi, ApiCloud, ApiLocal
+
+
+class AirstageACError(Exception):
+    """Airstage AC Error"""
 
 
 class AirstageAC:
-    def __init__(self, dsn: str, api: Api) -> None:
+    def __init__(self, dsn: str, api: AirstageApi | ApiCloud | ApiLocal) -> None:
         if not api:
-            raise Exception("Missing api")
+            raise AirstageACError("Missing api")
 
         if not dsn or not isinstance(dsn, str):
             raise ValueError("dsn must be a non-empty string")
 
         self._dsn = dsn
         self._api = api
         self._cache = {}
         self._min_temp = 18.0
         self._max_temp = 30.0
 
     def refresh_parameters(self, data: dict | None = None):
         if not data:
             devices = self._api.get_devices()
             if not isinstance(self.dsn, devices):
-                raise Exception(f"dsn not found {self.dsn}")
+                raise AirstageACError(f"dsn not found {self.dsn}")
             data = devices[self.dsn]
 
         self._cache = data
 
         for parameter in data["parameters"]:
             try:
                 name = parameter["name"]
@@ -32,17 +37,20 @@
                 parameter_name = ACParameter(name)
 
                 self._cache[parameter_name] = value
             except ValueError:
                 pass
         return self
 
+    def getCache(self):
+        return self._cache
+
     def _get_cached_device_parameter(self, parameterName: ACParameter) -> any:
         if not isinstance(parameterName, ACParameter):
-            raise Exception(f"Invalid parameter name: {parameterName}")
+            raise AirstageACError(f"Invalid parameter name: {parameterName}")
 
         if parameterName in self._cache:
             return self._cache[parameterName]
 
     def get_device_name(self) -> str:
         return str(self._get_cached_device_parameter(ACParameter.DEVICE_NAME))
 
@@ -62,25 +70,25 @@
             return OperationModeDescriptors.OFF
         return VALUE_TO_OPERATION_MODE[
             int(self._get_cached_device_parameter(ACParameter.OPERATION_MODE))
         ]
 
     async def set_operation_mode(self, mode: OperationMode):
         if not isinstance(mode, OperationMode):
-            raise Exception(f"Invalid operationMode value: {mode}")
+            raise AirstageACError(f"Invalid operationMode value: {mode}")
         await self._set_device_parameter(ACParameter.OPERATION_MODE, mode)
 
     def get_fan_speed(self):
         return VALUE_TO_FAN_SPEED[
             int(self._get_cached_device_parameter(ACParameter.FAN_SPEED))
         ]
 
     async def set_fan_speed(self, fan_speed: FanSpeed):
         if not isinstance(fan_speed, FanSpeed):
-            raise Exception(f"Invalid fan speed value: {fan_speed}")
+            raise AirstageACError(f"Invalid fan speed value: {fan_speed}")
         await self._set_device_parameter(ACParameter.FAN_SPEED, fan_speed)
 
     def get_display_temperature(self) -> float | None:
         return (
             int(self._get_cached_device_parameter(ACParameter.INDOOR_TEMPERATURE))
             - 5000
         ) / 100
@@ -88,40 +96,42 @@
     def get_target_temperature(self) -> float | None:
         return (
             int(self._get_cached_device_parameter(ACParameter.TARGET_TEMPERATURE)) / 10
         )
 
     async def set_target_temperature(self, target_temperature: float):
         if target_temperature < self._min_temp or target_temperature > self._max_temp:
-            raise Exception(
+            raise AirstageACError(
                 f"Invalid targetTemperature: {target_temperature}. Value must be {self._min_temp} <= target <= {self._max_temp}"
             )
 
         actual_target = int(target_temperature * 10)
         await self._set_device_parameter(ACParameter.TARGET_TEMPERATURE, actual_target)
 
     def get_vertical_direction(self):
         return VALUE_TO_VERTICAL_POSITION[
             int(self._get_cached_device_parameter(ACParameter.VERTICAL_DIRECTION))
         ]
 
     async def set_vertical_direction(self, direction: VerticalSwingPosition):
         if not isinstance(direction, VerticalSwingPosition):
-            raise Exception(f"Invalid fan direction value: {direction}")
+            raise AirstageACError(f"Invalid fan direction value: {direction}")
         await self._set_device_parameter(ACParameter.VERTICAL_DIRECTION, direction)
 
     def get_vertical_swing(self):
         return VALUE_TO_BOOLEAN[
             int(self._get_cached_device_parameter(ACParameter.VERTICAL_SWING))
         ]
 
     async def set_vertical_swing(self, mode: BooleanProperty):
         if not isinstance(mode, BooleanProperty):
-            raise Exception(f"Invalid mode value: {mode}")
+            raise AirstageACError(f"Invalid mode value: {mode}")
         await self._set_device_parameter(ACParameter.VERTICAL_SWING, mode)
 
     async def _set_device_parameter(self, parameterName: ACParameter, value):
         if not isinstance(parameterName, ACParameter):
-            raise Exception(f"Invalid property name: {parameterName}")
+            raise AirstageACError(f"Invalid property name: {parameterName}")
 
-        await self._api.set_parameter(self._dsn, parameterName, value)
-        self._cache[parameterName] = value
+        updatedValue = await self._api.set_parameter(self._dsn, parameterName, value)
+        if updatedValue is not None:
+            self._cache[parameterName] = value
+            return value
```

### Comparing `pyairstage-1.0.0/pyairstage/constants.py` & `pyairstage-1.0.1/pyairstage/constants.py`

 * *Files identical despite different names*

### Comparing `pyairstage-1.0.0/pyairstage.egg-info/PKG-INFO` & `pyairstage-1.0.1/pyairstage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairstage
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library to control Fujitsu Airstage Airconditioners
 Home-page: https://github.com/danielkaldheim/pyairstage
 Author: Daniel Rufus Kaldheim
 Author-email: daniel@kaldheim.org
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyairstage-1.0.0/setup.py` & `pyairstage-1.0.1/setup.py`

 * *Files identical despite different names*


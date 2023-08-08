# Comparing `tmp/ariston-0.14.0.tar.gz` & `tmp/ariston-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.14.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ariston-0.15.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.14.0.tar` & `ariston-0.15.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-06-12 11:37:25.630295 ariston-0.14.0/LICENSE
--rw-r--r--   0        0        0     3495 2023-06-12 11:37:25.630295 ariston-0.14.0/README.md
--rw-r--r--   0        0        0     5975 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/__init__.py
--rw-r--r--   0        0        0    23657 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/ariston_api.py
--rw-r--r--   0        0        0    13946 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/const.py
--rw-r--r--   0        0        0    12569 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/device.py
--rw-r--r--   0        0        0     3810 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/evo_device.py
--rw-r--r--   0        0        0     1130 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0    30970 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/galevo_device.py
--rw-r--r--   0        0        0     1491 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/lux_device.py
--rw-r--r--   0        0        0     3202 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0     9916 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     7143 2023-06-12 11:37:25.630295 ariston-0.14.0/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2023-06-12 11:37:25.630295 ariston-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-08 21:48:45.558502 ariston-0.15.0/LICENSE
+-rw-r--r--   0        0        0     3515 2023-08-08 21:48:45.558502 ariston-0.15.0/README.md
+-rw-r--r--   0        0        0     6115 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/__init__.py
+-rw-r--r--   0        0        0    27257 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/ariston_api.py
+-rw-r--r--   0        0        0    11325 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/bsb_device.py
+-rw-r--r--   0        0        0    15889 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/const.py
+-rw-r--r--   0        0        0    12583 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/device.py
+-rw-r--r--   0        0        0     3830 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/evo_device.py
+-rw-r--r--   0        0        0     1130 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    31109 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1515 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/lux_device.py
+-rw-r--r--   0        0        0     3202 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9916 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7143 2023-08-08 21:48:45.558502 ariston-0.15.0/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-08-08 21:48:45.558502 ariston-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 ariston-0.15.0/PKG-INFO
```

### Comparing `ariston-0.14.0/LICENSE` & `ariston-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.14.0/README.md` & `ariston-0.15.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 The following devices are currently supported:
 - Ariston Alteas One 24
 - Ariston Velis Evo
 - Ariston Velis Lux
 - Ariston Lydos Hybrid
 - Ariston Genus One
 - Ariston Nuos Split
+- Ariston Thision S
 
 ## Installation
 Use pip3 to install the latest version of this module.
 ```
 pip3 install ariston
 ```
```

### Comparing `ariston-0.14.0/ariston/__init__.py` & `ariston-0.15.0/ariston/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Ariston module"""
 import asyncio
 import logging
 from typing import Any, Optional
 
+from ariston.bsb_device import AristonBsbDevice
+
 from .ariston_api import AristonAPI, ConnectionException
 from .const import (
     DeviceAttribute,
     SystemType,
     VelisDeviceAttribute,
     WheType,
     PlantMode,
@@ -80,15 +82,15 @@
 ) -> Optional[AristonDevice]:
     """Get ariston device"""
     device = next(
         (dev for dev in cloud_devices if dev.get(DeviceAttribute.GW) == gateway),
         None,
     )
     if device is None:
-        _LOGGER.exception(f'No device "{gateway}" found.')
+        _LOGGER.exception("No device %s found.", gateway)
         return None
 
     system_type = device.get(DeviceAttribute.SYS)
     if system_type == SystemType.GALEVO.value:
         return AristonGalevoDevice(
             api,
             device,
@@ -113,18 +115,21 @@
                 device,
             )
         if whe_type == WheType.Lux.value:
             return AristonLuxDevice(
                 api,
                 device,
             )
-        _LOGGER.exception(f"Unsupported whe type {whe_type}")
+        _LOGGER.exception("Unsupported whe type %s", whe_type)
         return None
 
-    _LOGGER.exception(f"Unsupported system type {system_type}")
+    if system_type == SystemType.BSB.value:
+        return AristonBsbDevice(api, device)
+
+    _LOGGER.exception("Unsupported system type %s", system_type)
     return None
 
 
 def _connect(username: str, password: str) -> AristonAPI:
     """Connect to ariston api"""
     api = AristonAPI(username, password)
     api.connect()
```

### Comparing `ariston-0.14.0/ariston/ariston_api.py` & `ariston-0.15.0/ariston/ariston_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Ariston API"""
 from __future__ import annotations
 
 import logging
-import requests
-import aiohttp
-
 from typing import Any, Optional
 
+import aiohttp
+import requests
+
 from .const import (
     ARISTON_API_URL,
+    ARISTON_BSB_ZONES,
     ARISTON_DATA_ITEMS,
     ARISTON_LITE,
     ARISTON_LOGIN,
     ARISTON_PLANT_DATA,
     ARISTON_PLANTS,
     ARISTON_REMOTE,
     ARISTON_REPORTS,
     ARISTON_TIME_PROGS,
     ARISTON_VELIS,
+    BsbOperativeMode,
+    BsbZoneMode,
     DeviceFeatures,
     DeviceProperties,
     LydosPlantMode,
-    WaterHeaterMode,
     NuosSplitOperativeMode,
     PlantData,
     ThermostatProperties,
+    WaterHeaterMode,
     ZoneAttribute,
 )
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class ConnectionException(Exception):
     """When can not connect to Ariston cloud"""
 
 
@@ -171,14 +173,21 @@
                 "culture": culture,
             },
         )
         if properties is not None:
             return properties
         return dict()
 
+    def get_bsb_plant_data(self, gw_id: str) -> dict[str, Any]:
+        """Get BSB plant data."""
+        data = self._get(f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb}/{gw_id}")
+        if data is not None:
+            return data
+        return dict()
+
     def get_velis_plant_data(self, plant_data: PlantData, gw_id: str) -> dict[str, Any]:
         """Get Velis properties"""
         data = self._get(f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}")
         if data is not None:
             return data
         return dict()
 
@@ -242,14 +251,32 @@
         self._post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Slp.value}/{gw_id}/operativeMode",
             {
                 "new": value.value,
             },
         )
 
+    def set_bsb_mode(self, gw_id: str, value: BsbOperativeMode) -> None:
+        """Set Bsb mode"""
+        self._post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb.value}/{gw_id}/dhwMode",
+            {
+                "new": value.value,
+            },
+        )
+
+    def set_bsb_zone_mode(self, gw_id: str, zone: int, value: BsbZoneMode) -> None:
+        """Set Bsb zone mode"""
+        self._post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{ARISTON_BSB_ZONES}/{gw_id}/{zone}/mode",
+            {
+                "new": value.value,
+            },
+        )
+
     def set_evo_temperature(self, gw_id: str, value: float) -> None:
         """Set Velis Evo temperature"""
         self._post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Med.value}/{gw_id}/temperature",
             {
                 "new": value,
             },
@@ -272,14 +299,40 @@
                 "new": {
                     "comfort": comfort,
                     "reduced": reduced,
                 }
             },
         )
 
+    def set_bsb_temperature(self, gw_id: str, comfort: float, reduced: float) -> None:
+        """Set Bsb temperature"""
+        self._post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb.value}/{gw_id}/dhwTemp",
+            {
+                "new": {
+                    "comf": comfort,
+                    "econ": reduced,
+                }
+            },
+        )
+
+    def set_bsb_zone_temperature(
+        self, gw_id: str, zone: int, comfort: float, reduced: float
+    ) -> None:
+        """Set Bsb zone temperature"""
+        self._post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb.value}/{gw_id}/{zone}/temperatures",
+            {
+                "new": {
+                    "comf": comfort,
+                    "econ": reduced,
+                }
+            },
+        )
+
     def set_nous_boost(self, gw_id: str, boost: bool) -> None:
         """ "Set Nous boost"""
         self._post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Slp.value}/{gw_id}/boost",
             boost,
         )
 
@@ -349,15 +402,15 @@
         _LOGGER.debug(
             "Request method %s, path: %s, params: %s",
             method,
             path,
             params,
         )
         response = requests.request(
-            method, path, params=params, json=body, headers=headers
+            method, path, params=params, json=body, headers=headers, timeout=30000
         )
         if not response.ok:
             if response.status_code == 405:
                 if not is_retry:
                     if self.connect():
                         return self.__request(method, path, params, body, True)
                     raise Exception("Login failed (password changed?)")
@@ -491,14 +544,23 @@
                 "culture": culture,
             },
         )
         if properties is not None:
             return properties
         return dict()
 
+    async def async_get_bsb_plant_data(self, gw_id: str) -> dict[str, Any]:
+        """Get BSB plant data."""
+        data = await self._async_get(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb}/{gw_id}"
+        )
+        if data is not None:
+            return data
+        return dict()
+
     async def async_get_velis_plant_data(
         self, plant_data: PlantData, gw_id: str
     ) -> dict[str, Any]:
         """Async get Velis properties"""
         med_plant_data = await self._async_get(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}"
         )
@@ -568,14 +630,34 @@
         await self._async_post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Slp.value}/{gw_id}/operativeMode",
             {
                 "new": value.value,
             },
         )
 
+    async def async_set_bsb_mode(self, gw_id: str, value: BsbOperativeMode) -> None:
+        """Async set Bsb mode"""
+        await self._async_post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb.value}/{gw_id}/dhwMode",
+            {
+                "new": value.value,
+            },
+        )
+
+    async def async_set_bsb_zone_mode(
+        self, gw_id: str, zone: int, value: BsbZoneMode
+    ) -> None:
+        """Async set Bsb zone mode"""
+        await self._async_post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{ARISTON_BSB_ZONES}/{gw_id}/{zone}/mode",
+            {
+                "new": value.value,
+            },
+        )
+
     async def async_set_evo_temperature(self, gw_id: str, value: float) -> None:
         """Async set Velis Evo temperature"""
         await self._async_post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Med.value}/{gw_id}/temperature",
             {
                 "new": value,
             },
@@ -600,14 +682,42 @@
                 "new": {
                     "comfort": comfort,
                     "reduced": reduced,
                 }
             },
         )
 
+    async def async_set_bsb_temperature(
+        self, gw_id: str, comfort: float, reduced: float
+    ) -> None:
+        """Async set Bsb temperature"""
+        await self._async_post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{ARISTON_BSB_ZONES}/{gw_id}/dhwTemp",
+            {
+                "new": {
+                    "comf": comfort,
+                    "econ": reduced,
+                }
+            },
+        )
+
+    async def async_set_bsb_zone_temperature(
+        self, gw_id: str, zone: int, comfort: float, reduced: float
+    ) -> None:
+        """Async set Bsb zone temperature"""
+        await self._async_post(
+            f"{ARISTON_API_URL}{ARISTON_REMOTE}/{PlantData.Bsb.value}/{gw_id}/{zone}/temperatures",
+            {
+                "new": {
+                    "comf": comfort,
+                    "econ": reduced,
+                }
+            },
+        )
+
     async def async_set_nous_boost(self, gw_id: str, boost: bool) -> None:
         """ "Set Nous boost"""
         await self._async_post(
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Slp.value}/{gw_id}/boost",
             boost,
         )
```

### Comparing `ariston-0.14.0/ariston/const.py` & `ariston-0.15.0/ariston/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+"""Constants for ariston module"""
 from enum import Enum, unique
 from typing import Final
 
 ARISTON_API_URL: Final[str] = "https://www.ariston-net.remotethermo.com/api/v2/"
 ARISTON_LOGIN: Final[str] = "accounts/login"
 ARISTON_REMOTE: Final[str] = "remote"
 ARISTON_VELIS: Final[str] = "velis"
 ARISTON_PLANTS: Final[str] = "plants"
 ARISTON_LITE: Final[str] = "lite"
 ARISTON_DATA_ITEMS: Final[str] = "dataItems"
 ARISTON_ZONES: Final[str] = "zones"
+ARISTON_BSB_ZONES: Final[str] = "bsbZones"
 ARISTON_PLANT_DATA: Final[str] = "plantData"
 ARISTON_REPORTS: Final[str] = "reports"
 ARISTON_TIME_PROGS: Final[str] = "timeProgs"
 
 
 @unique
 class PlantData(str, Enum):
     """Plant data enum"""
 
     Med = "medPlantData"
     Se = "sePlantData"
     Slp = "slpPlantData"
+    Bsb = "bsbPlantData"
 
 
 @unique
 class PlantMode(Enum):
     """Plant mode enum"""
 
     UNDEFINED = -1
@@ -43,14 +46,23 @@
 
     UNDEFINED = -1
     OFF = 0
     MANUAL_NIGHT = 1
     MANUAL = 2
     TIME_PROGRAM = 3
 
+@unique
+class BsbZoneMode(Enum):
+    """BSB zone mode enum"""
+
+    UNDEFINED = -1
+    OFF = 0
+    TIME_PROGRAM = 1
+    MANUAL = 2
+    MANUAL_NIGHT = 3
 
 @unique
 class DhwMode(Enum):
     """Dhw mode enum"""
 
     DISABLED = 0
     TIME_BASED = 1
@@ -152,14 +164,21 @@
 
 
 class WaterHeaterMode(Enum):
     """Base class for plant modes"""
 
 
 @unique
+class BsbOperativeMode(WaterHeaterMode):
+    """BSB operative mode enum"""
+
+    OFF = 0
+    ON = 1
+
+@unique
 class LuxPlantMode(WaterHeaterMode):
     """Lux plant mode enum"""
 
     MANUAL = 1
     PROGRAM = 5
     BOOST = 9
 
@@ -387,14 +406,53 @@
 
 
 class LydosDeviceProperties(EvoLydosDeviceProperties):
     """Contants for Velis Lydos device properties"""
 
     BOOST_REQ_TEMP: Final[str] = "boostReqTemp"
 
+class BsbDeviceProperties:
+    """Constants for bsb device properties."""
+
+    DHW_COMF_TEMP: Final[str] = "dhwComfTemp"
+    DHW_ENABLED: Final[str] = "dhwEnabled"
+    DHW_MODE: Final[str] = "dhwMode"
+    DHW_PROG_READ_ONLY: Final[str] = "dhwProgReadOnly"
+    DHW_REDU_TEMP: Final[str] = "dhwReduTemp"
+    DHW_STORAGE_TEMP_ERROR: Final[str] = "dhwStorageTempError"
+    DHW_TEMP: Final[str] = "dhwTemp"
+    FLAME: Final[str] = "flame"
+    GW: Final[str] = "gw"
+    HAS_DHW_TEMP: Final[str] = "hasDhwTemp"
+    HAS_OUT_TEMP: Final[str] = "hasOutTemp"
+    HP_ON: Final[str] = "hpOn"
+    OUTSIDE_TEMP_ERROR: Final[str] = "outsideTempError"
+    OUT_TEMP: Final[str] = "outTemp"
+    ZONES: Final[str] = "zones"
+
+
+class BsbZoneProperties:
+    """Constants for bsb zone properties."""
+
+    CH_COMF_TEMP: Final[str] = "chComfTemp"
+    CH_PROT_TEMP: Final[str] = "chProtTemp"
+    CH_RED_TEMP: Final[str] = "chRedTemp"
+    COOL_COMF_TEMP: Final[str] = "coolComfTemp"
+    COOLING_ON: Final[str] = "coolingOn"
+    COOL_PROT_TEMP: Final[str] = "coolProtTemp"
+    COOL_RED_TEMP: Final[str] = "coolRedTemp"
+    DESIRED_ROOM_TEMP: Final[str] = "desiredRoomTemp"
+    HAS_ROOM_SENS: Final[str] = "hasRoomSens"
+    HEATING_ON: Final[str] = "heatingOn"
+    HEAT_OR_COOL_REQ: Final[str] = "heatOrCoolReq"
+    HOLIDAYS: Final[str] = "holidays"
+    MODE: Final[str] = "mode"
+    ROOM_TEMP: Final[str] = "roomTemp"
+    ROOM_TEMP_ERROR: Final[str] = "roomTempError"
+    USE_REDUCED_OPERATION_MODE_ON_HOLIDAY: Final[str] = "useReducedOperationModeOnHoliday"
 
 class MedDeviceSettings:
     """Constatns for Med device settings"""
 
     MED_ANTILEGIONELLA_ON_OFF: Final[str] = "MedAntilegionellaOnOff"
     MED_HEATING_RATE: Final[str] = "MedHeatingRate"
     MED_MAX_SETPOINT_TEMPERATURE: Final[str] = "MedMaxSetpointTemperature"
@@ -501,7 +559,8 @@
     UNIT: Final[str] = "unit"
     MIN: Final[str] = "min"
     MAX: Final[str] = "max"
     STEP: Final[str] = "step"
     DECIMALS: Final[str] = "decimals"
     ZONE: Final[str] = "zone"
     EXPIRES_ON: Final[str] = "expiresOn"
+    ALLOWED_OPTIONS: Final[str] = "allowedOptions"
```

### Comparing `ariston-0.14.0/ariston/device.py` & `ariston-0.15.0/ariston/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         """Get last value for consumption sequence"""
         for sequence in self.consumptions_sequences:
             if sequence["k"] == consumption_type.value and sequence["p"] == time_interval.value:
                 return sequence["v"][-1]
 
         return None
 
-    def _update_energy(self, old_consumptions_sequences: list[dict[str, Any]]) -> None:
+    def _update_energy(self, old_consumptions_sequences: Optional[list[dict[str, Any]]]) -> None:
         """Update the device energy settings"""
         if (
             self.custom_features.get(
                 ConsumptionType.DOMESTIC_HOT_WATER_ELECTRICITY.name
             )
             is None
         ):
@@ -323,15 +323,15 @@
         for consumption_type in ConsumptionType:
             if consumption_type.name is not None:
                 if (
                     self._get_consumption_sequence_last_value(
                         consumption_type,
                         ConsumptionTimeInterval.LAST_DAY,
                     )
-                    != None
+                    is not None
                 ):
                     self.custom_features[consumption_type.name] = True
                 else:
                     self.custom_features[consumption_type.name] = False
 
     def are_device_features_available(
         self,
```

### Comparing `ariston-0.14.0/ariston/evo_device.py` & `ariston-0.15.0/ariston/evo_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 
 from .const import (
     EvoPlantMode,
     EvoDeviceProperties,
     MedDeviceSettings,
     PlantData,
+    WaterHeaterMode,
 )
 from .evo_lydos_device import AristonEvoLydosDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AristonEvoDevice(AristonEvoLydosDevice):
@@ -31,15 +32,15 @@
 
     @property
     def consumption_type(self) -> str:
         """String to get consumption type"""
         return "Dhw"
 
     @property
-    def water_heater_mode(self) -> type[EvoPlantMode]:
+    def water_heater_mode(self) -> type[WaterHeaterMode]:
         """Return the water heater mode class"""
         return EvoPlantMode
 
     @property
     def max_setpoint_temp(self) -> str:
         return MedDeviceSettings.MED_MAX_SETPOINT_TEMPERATURE
 
@@ -48,15 +49,15 @@
         """Get water heater eco value"""
         return self.data.get(EvoDeviceProperties.ECO, None)
 
     @property
     def rm_tm_value(self) -> Optional[str]:
         """Get remaining time value"""
         return self.data.get(EvoDeviceProperties.RM_TM, None)
-    
+
     @property
     def rm_tm_in_minutes(self) -> int:
         """Get remaining time value in minutes"""
         rm_tm = self.rm_tm_value
         if rm_tm is None:
             return -1
         time = datetime.strptime(rm_tm, "%H:%M:%S")
```

### Comparing `ariston-0.14.0/ariston/evo_lydos_device.py` & `ariston-0.15.0/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.14.0/ariston/galevo_device.py` & `ariston-0.15.0/ariston/galevo_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,19 @@
         self.energy_account: dict[str, Any] = dict()
 
     @property
     def consumption_type(self) -> str:
         """String to get consumption type"""
         return f"Ch{'%2CDhw' if self.custom_features.get(CustomDeviceFeatures.HAS_DHW) else ''}"
 
+    @property
+    def plant_mode_supported(self) -> bool:
+        """Returns is plant mode supported"""
+        return True
+
     def _update_state(self) -> None:
         """Set custom features"""
         if self.custom_features.get(CustomDeviceFeatures.HAS_OUTSIDE_TEMP) is None:
             temp = self._get_item_by_id(
                 DeviceProperties.OUTSIDE_TEMP, PropertyType.VALUE
             )
             max_temp = self._get_item_by_id(
@@ -213,36 +218,36 @@
         """Is zone in time program mode"""
         return self.get_zone_mode(zone) in [
             ZoneMode.TIME_PROGRAM,
         ]
 
     def is_zone_mode_options_contains_manual(self, zone: int) -> bool:
         """Is zone mode options contains manual mode"""
-        return (ZoneMode.MANUAL or ZoneMode.MANUAL_NIGHT) in self.get_zone_mode_options(
+        return (ZoneMode.MANUAL.value or ZoneMode.MANUAL_NIGHT.value) in self.get_zone_mode_options(
             zone
         )
 
     def is_zone_mode_options_contains_time_program(self, zone: int) -> bool:
         """Is zone mode options contains time program mode"""
-        return ZoneMode.TIME_PROGRAM in self.get_zone_mode_options(zone)
+        return ZoneMode.TIME_PROGRAM.value in self.get_zone_mode_options(zone)
 
     def is_zone_mode_options_contains_off(self, zone: int) -> bool:
         """Is zone mode options contains off mode"""
-        return ZoneMode.OFF in self.get_zone_mode_options(zone)
+        return ZoneMode.OFF.value in self.get_zone_mode_options(zone)
 
     @property
     def is_plant_mode_options_contains_off(self) -> bool:
         """Is plant mode options contains off mode"""
-        return PlantMode.OFF in self.plant_mode_options
+        return PlantMode.OFF.value in self.plant_mode_options
 
     @property
     def is_plant_mode_options_contains_cooling(self) -> bool:
         """Is plant mode options contains cooling mode"""
         return (
-            PlantMode.COOLING or PlantMode.COOLING_ONLY
+            PlantMode.COOLING.value or PlantMode.COOLING_ONLY.value
         ) in self.plant_mode_options
 
     @staticmethod
     def get_zone_number(zone_number: int) -> str:
         """Get zone number"""
         return f"{zone_number}"
 
@@ -306,17 +311,17 @@
         """Get central heating flow temperature unit"""
         return self._get_item_by_id(DeviceProperties.CH_FLOW_TEMP, PropertyType.UNIT)
 
     @property
     def is_flame_on_value(self) -> bool:
         """Get is flame on value"""
         return self._get_item_by_id(DeviceProperties.IS_FLAME_ON, PropertyType.VALUE)
-        
+
     @property
-    def is_heating_pump_on_value(self) -> bool:                              
+    def is_heating_pump_on_value(self) -> bool:
         """Get is heating pump on value"""                                           
         return self._get_item_by_id(DeviceProperties.IS_HEATING_PUMP_ON, PropertyType.VALUE)
 
     @property
     def holiday_mode_value(self) -> bool:
         """Get holiday mode on value"""
         return self._get_item_by_id(DeviceProperties.HOLIDAY, PropertyType.VALUE)
@@ -791,15 +796,15 @@
             value,
             current_value,
             self.umsys,
         )
         self._set_item_by_id(item_id, value, zone_number)
 
     @staticmethod
-    def _create_holiday_end_date(holiday_end: date):
+    def _create_holiday_end_date(holiday_end: Optional[date]):
         return (
             None if holiday_end is None else holiday_end.strftime("%Y-%m-%dT00:00:00")
         )
 
     def _set_holiday(self, holiday_end_date: Optional[str]):
         for item in self.data.get("items", dict()):
             if item.get("id") == DeviceProperties.HOLIDAY:
```

### Comparing `ariston-0.14.0/ariston/lux_device.py` & `ariston-0.15.0/ariston/lux_device.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 import logging
 from typing import Optional
 
 from .const import (
     LuxPlantMode,
     EvoDeviceProperties,
-    EvoLydosDeviceProperties
+    EvoLydosDeviceProperties,
+    WaterHeaterMode
 )
 from .evo_device import AristonEvoDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AristonLuxDevice(AristonEvoDevice):
     """Class representing a physical device, it's state and properties."""
 
     @property
-    def water_heater_mode(self) -> type[LuxPlantMode]:
+    def water_heater_mode(self) -> type[WaterHeaterMode]:
         """Return the water heater mode class"""
         return LuxPlantMode
 
     def set_water_heater_operation_mode(self, operation_mode: str):
         """Set water heater operation mode"""
         self.api.set_evo_mode(self.gw, LuxPlantMode[operation_mode])
         self.data[EvoDeviceProperties.MODE] = LuxPlantMode[operation_mode].value
```

### Comparing `ariston-0.14.0/ariston/lydos_hybrid_device.py` & `ariston-0.15.0/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.14.0/ariston/nuos_split_device.py` & `ariston-0.15.0/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.14.0/ariston/velis_device.py` & `ariston-0.15.0/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.14.0/PKG-INFO` & `ariston-0.15.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.14.0
+Version: 0.15.0
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
 
@@ -15,14 +15,15 @@
 The following devices are currently supported:
 - Ariston Alteas One 24
 - Ariston Velis Evo
 - Ariston Velis Lux
 - Ariston Lydos Hybrid
 - Ariston Genus One
 - Ariston Nuos Split
+- Ariston Thision S
 
 ## Installation
 Use pip3 to install the latest version of this module.
 ```
 pip3 install ariston
 ```
```


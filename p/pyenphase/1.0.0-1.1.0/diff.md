# Comparing `tmp/pyenphase-1.0.0.tar.gz` & `tmp/pyenphase-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.0.0.tar", max compression
+gzip compressed data, was "pyenphase-1.1.0.tar", max compression
```

## Comparing `pyenphase-1.0.0.tar` & `pyenphase-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-08-08 18:40:36.891816 pyenphase-1.0.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-08 18:40:36.891816 pyenphase-1.0.0/README.md
--rw-r--r--   0        0        0     2376 2023-08-08 18:40:37.999810 pyenphase-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1041 2023-08-08 18:40:37.971810 pyenphase-1.0.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8051 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/const.py
--rw-r--r--   0        0        0    14257 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     2314 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0        0 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      938 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 18:50:29.201014 pyenphase-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-08 18:50:29.201014 pyenphase-1.1.0/README.md
+-rw-r--r--   0        0        0     2376 2023-08-08 18:50:30.281072 pyenphase-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1041 2023-08-08 18:50:30.241070 pyenphase-1.1.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8051 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      684 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0    15419 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     2314 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2451 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1086 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.0/PKG-INFO
```

### Comparing `pyenphase-1.0.0/LICENSE` & `pyenphase-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/README.md` & `pyenphase-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/pyproject.toml` & `pyenphase-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.0.0"
+version = "1.1.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.0.0/src/pyenphase/__init__.py` & `pyenphase-1.1.0/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/auth.py` & `pyenphase-1.1.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/const.py` & `pyenphase-1.1.0/src/pyenphase/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 URL_PRODUCTION_INVERTERS = "/api/v1/production/inverters"
 URL_PRODUCTION_V1 = "/api/v1/production"
 URL_PRODUCTION_JSON = "/production.json"
 URL_PRODUCTION = "/production"
 
 # Battery and Enpower Status
 URL_DRY_CONTACT_STATUS = "/ivp/ensemble/dry_contacts"
-URL_DRY_CONTACT_SETTINGS = "/ivp/ensemble/dry_contact_settings"
+URL_DRY_CONTACT_SETTINGS = "/ivp/ss/dry_contact_settings"
 URL_ENSEMBLE_INVENTORY = "/ivp/ensemble/inventory"
 URL_ENCHARGE_BATTERY = "/ivp/ensemble/power"
 URL_GRID_RELAY = "/ivp/ensemble/relay"
 URL_POWER_EXPORT = "/uvp/ss/pel_settings"
 URL_TARIFF = "/admin/lib/tariff"
 
 # Generator Configuration
```

### Comparing `pyenphase-1.0.0/src/pyenphase/envoy.py` & `pyenphase-1.1.0/src/pyenphase/envoy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 import orjson
 from awesomeversion import AwesomeVersion
 from envoy_utils.envoy_utils import EnvoyUtils
 from tenacity import retry, retry_if_exception_type, wait_random_exponential
 
 from .auth import EnvoyAuth, EnvoyLegacyAuth, EnvoyTokenAuth
 from .const import (
+    URL_DRY_CONTACT_SETTINGS,
+    URL_DRY_CONTACT_STATUS,
     URL_ENCHARGE_BATTERY,
     URL_ENSEMBLE_INVENTORY,
     URL_PRODUCTION,
     URL_PRODUCTION_INVERTERS,
     URL_PRODUCTION_JSON,
     URL_PRODUCTION_V1,
 )
 from .exceptions import (
     ENDPOINT_PROBE_EXCEPTIONS,
     EnvoyAuthenticationRequired,
     EnvoyProbeFailed,
 )
 from .firmware import EnvoyFirmware, EnvoyFirmwareCheckError
+from .models.dry_contacts import EnvoyDryContactSettings, EnvoyDryContactStatus
 from .models.encharge import EnvoyEncharge, EnvoyEnchargePower
 from .models.enpower import EnvoyEnpower
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 from .ssl import NO_VERIFY_SSL_CONTEXT
@@ -43,17 +46,16 @@
 
 
 class SupportedFeatures(enum.IntFlag):
     INVERTERS = 1
     METERING = 2
     TOTAL_CONSUMPTION = 4
     NET_CONSUMPTION = 8
-    DRY_CONTACTS = 16
-    ENCHARGE = 32
-    ENPOWER = 64
+    ENCHARGE = 16
+    ENPOWER = 32
 
 
 class Envoy:
     """Class for communicating with an envoy."""
 
     def __init__(
         self,
@@ -303,14 +305,16 @@
             }
             raw["inverters"] = inverters_data
 
         # Update Enpower and Encharge data if supported
         encharge_inventory: dict[str, EnvoyEncharge] | None = None
         encharge_power: dict[str, EnvoyEnchargePower] | None = None
         enpower: EnvoyEnpower | None = None
+        dry_contact_settings: dict[str, EnvoyDryContactSettings] = {}
+        dry_contact_status: dict[str, EnvoyDryContactStatus] = {}
 
         if (
             supported_features & SupportedFeatures.ENCHARGE
             or supported_features & SupportedFeatures.ENPOWER
         ):
             ensemble_inventory_data: list[dict[str, Any]] = await self.request(
                 URL_ENSEMBLE_INVENTORY
@@ -339,28 +343,46 @@
                     for serial in inventory
                 }
                 encharge_power = {
                     serial: EnvoyEnchargePower.from_api(power[serial])
                     for serial in power
                 }
             if supported_features & SupportedFeatures.ENPOWER:
+                # Update Enpower data
                 for item in ensemble_inventory_data:
                     if item["type"] != "ENPOWER":
                         continue
                     enpower_data = item["devices"][0]
                 raw["enpower"] = enpower_data
                 enpower = EnvoyEnpower.from_api(enpower_data)
 
+                # Update dry contact data
+                dry_contact_status_data = await self.request(URL_DRY_CONTACT_STATUS)
+                dry_contact_settings_data = await self.request(URL_DRY_CONTACT_SETTINGS)
+                raw["dry_contact_status"] = dry_contact_status_data
+                raw["dry_contact_settings"] = dry_contact_settings_data
+
+                dry_contact_status = {
+                    relay["id"]: EnvoyDryContactStatus.from_api(relay)
+                    for relay in dry_contact_status_data["dry_contacts"]
+                }
+                dry_contact_settings = {
+                    relay["id"]: EnvoyDryContactSettings.from_api(relay)
+                    for relay in dry_contact_settings_data["dry_contacts"]
+                }
+
         data = EnvoyData(
             system_production=system_production,
             system_consumption=system_consumption,
             inverters=inverters,
             encharge_inventory=encharge_inventory,
             encharge_power=encharge_power,
             enpower=enpower,
+            dry_contact_status=dry_contact_status,
+            dry_contact_settings=dry_contact_settings,
             # Raw data is exposed so we can __eq__ the data to see if
             # anything has changed and consumers of the library can
             # avoid dispatching data if nothing has changed.
             raw=raw,
         )
         self.data = data
         return data
```

### Comparing `pyenphase-1.0.0/src/pyenphase/exceptions.py` & `pyenphase-1.1.0/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/firmware.py` & `pyenphase-1.1.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/models/encharge.py` & `pyenphase-1.1.0/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/models/enpower.py` & `pyenphase-1.1.0/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/models/envoy.py` & `pyenphase-1.1.0/src/pyenphase/models/envoy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Model for an envoy."""
 
 from dataclasses import dataclass, field
 from typing import Any
 
-from .dry_contacts import EnvoyDryContact
+from .dry_contacts import EnvoyDryContactSettings, EnvoyDryContactStatus
 from .encharge import EnvoyEncharge, EnvoyEnchargePower
 from .enpower import EnvoyEnpower
 from .inverter import EnvoyInverter
 from .system_consumption import EnvoySystemConsumption
 from .system_production import EnvoySystemProduction
 
 
@@ -16,10 +16,13 @@
     """Model for an envoy."""
 
     encharge_inventory: dict[str, EnvoyEncharge] | None = None
     encharge_power: dict[str, EnvoyEnchargePower] | None = None
     enpower: EnvoyEnpower | None = None
     system_consumption: EnvoySystemConsumption | None = None
     system_production: EnvoySystemProduction | None = None
-    dry_contacts: dict[str, EnvoyDryContact] = field(default_factory=dict)
+    dry_contact_status: dict[str, EnvoyDryContactStatus] = field(default_factory=dict)
+    dry_contact_settings: dict[str, EnvoyDryContactSettings] = field(
+        default_factory=dict
+    )
     inverters: dict[str, EnvoyInverter] = field(default_factory=dict)
     raw: dict[str, dict[str, Any]] = field(default_factory=dict)
```

### Comparing `pyenphase-1.0.0/src/pyenphase/models/inverter.py` & `pyenphase-1.1.0/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/models/system_consumption.py` & `pyenphase-1.1.0/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/models/system_production.py` & `pyenphase-1.1.0/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/src/pyenphase/ssl.py` & `pyenphase-1.1.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.0.0/PKG-INFO` & `pyenphase-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 1.0.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.1.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```


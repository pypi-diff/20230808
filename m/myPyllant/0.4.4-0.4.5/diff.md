# Comparing `tmp/mypyllant-0.4.4.tar.gz` & `tmp/mypyllant-0.4.5.tar.gz`

## Comparing `mypyllant-0.4.4.tar` & `mypyllant-0.4.5.tar`

### file list

```diff
@@ -1,48 +1,57 @@
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.dockerignore
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.4/Dockerfile
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.4/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.4/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.4/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.github/workflows/docker.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/api.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/export.py
--rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/sample.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.4/LICENSE
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.4/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.5/.dockerignore
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.5/Dockerfile
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.5/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.5/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.5/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.5/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.5/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/export.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_models.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0     1567 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/control_identifier.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/current_system.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/firmware_update_required.json
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/system.json
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 mypyllant-0.4.5/src/myPyllant/tests/json/no_system/time_zone.json
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.5/LICENSE
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 mypyllant-0.4.5/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 mypyllant-0.4.5/PKG-INFO
```

### Comparing `mypyllant-0.4.4/.dockerignore` & `mypyllant-0.4.5/.dockerignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/.pre-commit-config.yaml` & `mypyllant-0.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/logo.png` & `mypyllant-0.4.5/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/.github/workflows/build-test.yaml` & `mypyllant-0.4.5/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/.github/workflows/docker.yaml` & `mypyllant-0.4.5/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/api.py` & `mypyllant-0.4.5/src/myPyllant/api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/const.py` & `mypyllant-0.4.5/src/myPyllant/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         "poland": "Poland",
         "portugal": "Portugal",
         "romania": "Romania",
         "slovakia": "Slovakia",
         "spain": "Spain",
     },
 }
+ALL_COUNTRIES = {c: n for d in COUNTRIES.values() for c, n in d.items()}
 MANUAL_SETPOINT_TYPES = {
     "HEATING": "Heating",
     "COOLING": "Cooling",
 }
 DEFAULT_MANUAL_SETPOINT_TYPE = "HEATING"
 DEFAULT_QUICK_VETO_DURATION = 3
 DEFAULT_CONTROL_IDENTIFIER = "tli"
```

### Comparing `mypyllant-0.4.4/src/myPyllant/export.py` & `mypyllant-0.4.5/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/models.py` & `mypyllant-0.4.5/src/myPyllant/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,23 @@
     def water_pressure(self) -> float | None:
         try:
             return self.state["system"]["system_water_pressure"]
         except KeyError:
             logger.info("Could not get water pressure from system control state")
             return None
 
+    @property
+    def system_name(self) -> str:
+        if self.primary_heat_generator:
+            return self.primary_heat_generator.product_name_display
+        elif self.claim:
+            return self.claim.nomenclature
+        else:
+            return "System"
+
 
 class Device(BaseModel):
     system_id: str
     device_uuid: str
     name: str | None
     product_name: str | None
     diagnostic_trouble_codes: list = []
```

### Comparing `mypyllant-0.4.4/src/myPyllant/sample.py` & `mypyllant-0.4.5/src/myPyllant/sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import argparse
 import asyncio
 import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
+from myPyllant.const import ALL_COUNTRIES, BRANDS, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
     "--country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    choices=ALL_COUNTRIES.keys(),
     required=False,
 )
 parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
@@ -36,24 +36,25 @@
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
             print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
-            print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
-            print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
-            print(
-                await api.set_domestic_hot_water_temperature(
-                    system.domestic_hot_water[0], 46
-                )
-            )
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
+            if system.domestic_hot_water:
+                print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
+                print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
+                print(
+                    await api.set_domestic_hot_water_temperature(
+                        system.domestic_hot_water[0], 46
+                    )
+                )
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.brand, args.country))
```

### Comparing `mypyllant-0.4.4/src/myPyllant/utils.py` & `mypyllant-0.4.5/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.5/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.5/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.5/src/myPyllant/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from datetime import datetime, timedelta, tzinfo
+from pathlib import Path
 
 import pytest
 from freezegun import freeze_time
 
 from myPyllant.api import MyPyllantAPI, RealmInvalid
 from myPyllant.models import (
     Device,
@@ -15,24 +16,28 @@
 )
 
 from ..const import DEFAULT_QUICK_VETO_DURATION
 from ..utils import datetime_format
 from .generate_test_data import JSON_DIR
 
 
-def get_test_data():
+def list_test_data():
     test_data = []
     for d in [d for d in JSON_DIR.iterdir() if d.is_dir()]:
-        user_data = {}
-        for f in d.glob("*.json"):
-            user_data[f.stem] = json.loads(f.read_text())
-        test_data.append(user_data)
+        test_data.append(load_test_data(d))
     return test_data
 
 
+def load_test_data(data_dir: Path):
+    user_data = {}
+    for f in data_dir.glob("*.json"):
+        user_data[f.stem] = json.loads(f.read_text())
+    return user_data
+
+
 async def test_login_vaillant(mypyllant_aioresponses) -> None:
     with mypyllant_aioresponses() as _:
         async with MyPyllantAPI(
             "test@example.com", "test", "vaillant", "germany"
         ) as mocked_api:
             assert isinstance(mocked_api.oauth_session_expires, datetime)
             assert mocked_api.oauth_session_expires > datetime.now()
@@ -66,75 +71,75 @@
         with freeze_time(datetime.now() + timedelta(hours=1)):
             await mocked_api.refresh_token()
             session_expires = mocked_api.oauth_session_expires
         assert session_expires - datetime.now() > timedelta(hours=1)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_systems(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
 
         assert isinstance(system, System), "Expected System return type"
         assert isinstance(system.outdoor_temperature, (float | None))
         assert isinstance(system.water_pressure, float)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_meta_info(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
         status = await mocked_api.get_connection_status(system)
         assert isinstance(status, bool)
         time_zone = await mocked_api.get_time_zone(system)
         assert isinstance(time_zone, tzinfo)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_meta_info_system_id(
     mypyllant_aioresponses, mocked_api, test_data
 ) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
         control_identifier = await mocked_api.get_control_identifier(system.id)
         assert isinstance(control_identifier, str)
         status = await mocked_api.get_connection_status(system.id)
         assert isinstance(status, bool)
         time_zone = await mocked_api.get_time_zone(system.id)
         assert isinstance(time_zone, tzinfo)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_devices(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
         if len(system.devices) > 0:
             device = system.devices[0]
             assert isinstance(device, Device)
             assert isinstance(device.name_display, str)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_device_data(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
         if len(system.devices) > 0:
             device = system.devices[0]
             device_data = await anext(mocked_api.get_data_by_device(device))
             assert isinstance(device_data, DeviceData)
             assert isinstance(device_data.data[0], DeviceDataBucket)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_quick_veto(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
         zone: Zone = system.zones[0]
         # Activating quick veto
         zone.current_special_function = ZoneCurrentSpecialFunction.NONE
         await mocked_api.quick_veto_zone_temperature(zone, 20.0)
@@ -147,15 +152,15 @@
         await mocked_api.quick_veto_zone_temperature(zone, 20.0)
         request = list(aio.requests.values())[-1][0]
         assert request.kwargs["json"]["desiredRoomTemperatureSetpoint"] == 20.0
         assert "duration" not in request.kwargs["json"]
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_holiday_without_dates(
     mypyllant_aioresponses, mocked_api, test_data
 ) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
         now = datetime.now()
         with freeze_time(now):
@@ -163,15 +168,15 @@
         request = list(aio.requests.values())[-1][0]
         assert request.kwargs["json"]["holidayStartDateTime"] == datetime_format(
             now, with_microseconds=True
         )
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_holiday_with_dates(
     mypyllant_aioresponses, mocked_api, test_data
 ) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
         now = datetime.now()
         with freeze_time(now):
@@ -184,30 +189,40 @@
         )
         assert request.kwargs["json"]["holidayEndDateTime"] == datetime_format(
             end, with_microseconds=True
         )
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_holiday_wrong_dates(
     mypyllant_aioresponses, mocked_api, test_data
 ) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
         start = datetime.now() + timedelta(days=1)
         end = start - timedelta(days=7)
         with pytest.raises(ValueError):
             await mocked_api.set_holiday(system, start, end)
         await mocked_api.aiohttp_session.close()
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_dhw_setpoint(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
+        if not system.domestic_hot_water:
+            return
         await mocked_api.set_domestic_hot_water_temperature(
             system.domestic_hot_water[0], 60
         )
         request = list(aio.requests.values())[-1][0]
         assert request.kwargs["json"]["setPoint"] == 60
         await mocked_api.aiohttp_session.close()
+
+
+async def test_no_system(mypyllant_aioresponses, mocked_api) -> None:
+    test_data = load_test_data(JSON_DIR / "no_system")
+    with mypyllant_aioresponses(test_data) as _:
+        system = await anext(mocked_api.get_systems())
+        assert system.outdoor_temperature == 15.5625
+        assert system.water_pressure == 1.0
```

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.5/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.5/src/myPyllant/tests/test_export.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 
 import pytest as pytest
 
 from ..export import main as export_main
-from .test_api import get_test_data
+from .test_api import list_test_data
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_export(mypyllant_aioresponses, capsys, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         await export_main("test@example.com", "test", "vaillant", "germany")
         captured = capsys.readouterr()
         assert isinstance(json.loads(captured.out), dict)
 
 
-@pytest.mark.parametrize("test_data", get_test_data())
+@pytest.mark.parametrize("test_data", list_test_data())
 async def test_export_data(mypyllant_aioresponses, capsys, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         await export_main("test@example.com", "test", "vaillant", "germany", data=True)
         captured = capsys.readouterr()
         assert isinstance(json.loads(captured.out), list)
```

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.5/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/utils.py` & `mypyllant-0.4.5/src/myPyllant/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.5/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/.gitignore` & `mypyllant-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/LICENSE` & `mypyllant-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/README.md` & `mypyllant-0.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,29 @@
 
 import argparse
 import asyncio
 import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
+from myPyllant.const import ALL_COUNTRIES, BRANDS, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
     "--country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    choices=ALL_COUNTRIES.keys(),
     required=False,
 )
 parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
@@ -71,24 +71,25 @@
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
             print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
-            print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
-            print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
-            print(
-                await api.set_domestic_hot_water_temperature(
-                    system.domestic_hot_water[0], 46
-                )
-            )
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
+            if system.domestic_hot_water:
+                print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
+                print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
+                print(
+                    await api.set_domestic_hot_water_temperature(
+                        system.domestic_hot_water[0], 46
+                    )
+                )
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.brand, args.country))
```

### Comparing `mypyllant-0.4.4/pyproject.toml` & `mypyllant-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.4/PKG-INFO` & `mypyllant-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,29 +53,29 @@
 
 import argparse
 import asyncio
 import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
+from myPyllant.const import ALL_COUNTRIES, BRANDS, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
 parser.add_argument(
     "--country",
     help="Country your account is registered in, i.e. 'germany'",
-    choices=COUNTRIES[DEFAULT_BRAND].keys(),
+    choices=ALL_COUNTRIES.keys(),
     required=False,
 )
 parser.add_argument(
     "-v", "--verbose", help="increase output verbosity", action="store_true"
 )
 
 
@@ -87,24 +87,25 @@
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
             print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
-            print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
-            print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
-            print(
-                await api.set_domestic_hot_water_temperature(
-                    system.domestic_hot_water[0], 46
-                )
-            )
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
+            if system.domestic_hot_water:
+                print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
+                print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
+                print(
+                    await api.set_domestic_hot_water_temperature(
+                        system.domestic_hot_water[0], 46
+                    )
+                )
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.brand, args.country))
```


# Comparing `tmp/cerc-co2-emission-0.1.0.1.tar.gz` & `tmp/cerc-co2-emission-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-co2-emission-0.1.0.1.tar", last modified: Thu Aug  3 17:48:00 2023, max compression
+gzip compressed data, was "cerc-co2-emission-0.1.0.2.tar", last modified: Tue Aug  8 17:42:50 2023, max compression
```

## Comparing `cerc-co2-emission-0.1.0.1.tar` & `cerc-co2-emission-0.1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 17:48:00.443729 cerc-co2-emission-0.1.0.1/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      423 2023-08-03 17:48:00.443729 cerc-co2-emission-0.1.0.1/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)      523 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 17:48:00.443729 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      423 2023-08-03 17:48:00.000000 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (117)      332 2023-08-03 17:48:00.000000 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-03 17:48:00.000000 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       20 2023-08-03 17:48:00.000000 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       13 2023-08-03 17:48:00.000000 cerc-co2-emission-0.1.0.1/cerc_co2_emission.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-03 17:48:00.443729 cerc-co2-emission-0.1.0.1/co2_emission/
--rw-r--r--   0 jenkins    (109) jenkins    (117)      338 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/co2_emission/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)     3069 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/co2_emission/co2_emission.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      352 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/co2_emission/version.py
--rw-r--r--   0 jenkins    (109) jenkins    (117)      173 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/pyproject.toml
--rw-r--r--   0 jenkins    (109) jenkins    (117)        8 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/requirements.txt
--rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-03 17:48:00.443729 cerc-co2-emission-0.1.0.1/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (117)     1076 2023-08-02 20:23:24.000000 cerc-co2-emission-0.1.0.1/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 17:42:50.106778 cerc-co2-emission-0.1.0.2/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      423 2023-08-08 17:42:50.106778 cerc-co2-emission-0.1.0.2/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      523 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 17:42:50.106778 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      423 2023-08-08 17:42:50.000000 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      332 2023-08-08 17:42:50.000000 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        1 2023-08-08 17:42:50.000000 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       20 2023-08-08 17:42:50.000000 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       13 2023-08-08 17:42:50.000000 cerc-co2-emission-0.1.0.2/cerc_co2_emission.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins    (109) jenkins    (117)        0 2023-08-08 17:42:50.106778 cerc-co2-emission-0.1.0.2/co2_emission/
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      338 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/co2_emission/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     3084 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/co2_emission/co2_emission.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      352 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/co2_emission/version.py
+-rw-r--r--   0 jenkins    (109) jenkins    (117)      173 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/pyproject.toml
+-rw-r--r--   0 jenkins    (109) jenkins    (117)        8 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/requirements.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (117)       38 2023-08-08 17:42:50.106778 cerc-co2-emission-0.1.0.2/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (117)     1076 2023-08-08 17:41:46.000000 cerc-co2-emission-0.1.0.2/setup.py
```

### Comparing `cerc-co2-emission-0.1.0.1/README.md` & `cerc-co2-emission-0.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cerc-co2-emission-0.1.0.1/co2_emission/co2_emission.py` & `cerc-co2-emission-0.1.0.2/co2_emission/co2_emission.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 class Co2Emission:
   """
   Cost class
   """
 
   def __init__(self, building: Building, emissions_factor=None):
     if emissions_factor is None:
-      emissions_factor = {cte.GAS: 0.2025,
-                          cte.ELECTRICITY: 0.00113,
-                          cte.DIESEL: 0.2683,
+      # kgCO2 / J
+      emissions_factor = {cte.GAS: 56.25480769E-9,
+                          cte.ELECTRICITY: 0.313840909E-9,
+                          cte.DIESEL: 74.52882883E-9,
                           cte.RENEWABLE: 0}
     self._emissions_factor = emissions_factor
     self._building = building
 
   @property
   def building(self) -> Building:
     """
@@ -61,21 +62,21 @@
               values.append(value * self._emissions_factor[fuel_type])
             results_by_time_period[time_period] = values
         results[demand_type] = results_by_time_period
 
     results_by_time_period = {}
     for time_period in self._building.lighting_electrical_demand:
       values = []
-      for value in self._building.lighting_electrical_demand[time_period]['insel meb']:
+      for value in self._building.lighting_electrical_demand[time_period]:
         values.append(value * self._emissions_factor[cte.ELECTRICITY])
       results_by_time_period[time_period] = values
     results[cte.LIGHTING] = results_by_time_period
 
     results_by_time_period = {}
     for time_period in self._building.appliances_electrical_demand:
       values = []
-      for value in self._building.appliances_electrical_demand[time_period]['insel meb']:
+      for value in self._building.appliances_electrical_demand[time_period]:
         values.append(value * self._emissions_factor[cte.ELECTRICITY])
       results_by_time_period[time_period] = values
     results[cte.APPLIANCES] = results_by_time_period
 
     return results
```

### Comparing `cerc-co2-emission-0.1.0.1/setup.py` & `cerc-co2-emission-0.1.0.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/MeteoGalicia-API-0.0.7.tar.gz` & `tmp/MeteoGalicia-API-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeteoGalicia-API-0.0.7.tar", last modified: Tue Jun 20 21:13:15 2023, max compression
+gzip compressed data, was "MeteoGalicia-API-0.0.8.tar", last modified: Tue Aug  8 07:54:00 2023, max compression
```

## Comparing `MeteoGalicia-API-0.0.7.tar` & `MeteoGalicia-API-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.171267 MeteoGalicia-API-0.0.7/
--rw-r--r--   0 pi        (1000) pi        (1000)    35149 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/LICENSE.md
--rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/MANIFEST.in
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.163267 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      391 2023-06-20 21:13:15.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/not-zip-safe
--rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       17 2023-06-20 21:13:14.000000 MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-06-20 21:13:15.171267 MeteoGalicia-API-0.0.7/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1145 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 21:13:15.167267 MeteoGalicia-API-0.0.7/meteogalicia_api/
--rw-r--r--   0 pi        (1000) pi        (1000)       29 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)       36 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/const.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1595 2023-06-20 21:10:50.000000 MeteoGalicia-API-0.0.7/meteogalicia_api/interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-06-20 17:56:00.000000 MeteoGalicia-API-0.0.7/requirements.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       54 2023-06-20 21:13:15.175267 MeteoGalicia-API-0.0.7/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1838 2023-06-20 21:12:37.000000 MeteoGalicia-API-0.0.7/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-08 07:54:00.510575 MeteoGalicia-API-0.0.8/
+-rw-r--r--   0 pi        (1000) pi        (1000)    35149 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/LICENSE.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/MANIFEST.in
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-08 07:54:00.506575 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-08-08 07:53:59.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      391 2023-08-08 07:54:00.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-08 07:53:59.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-08 07:53:59.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/not-zip-safe
+-rw-r--r--   0 pi        (1000) pi        (1000)        9 2023-08-08 07:53:59.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       17 2023-08-08 07:53:59.000000 MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     2388 2023-08-08 07:54:00.510575 MeteoGalicia-API-0.0.8/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1145 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-08 07:54:00.510575 MeteoGalicia-API-0.0.8/meteogalicia_api/
+-rw-r--r--   0 pi        (1000) pi        (1000)       29 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/meteogalicia_api/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       36 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/meteogalicia_api/const.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2529 2023-08-08 07:47:41.000000 MeteoGalicia-API-0.0.8/meteogalicia_api/interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-08-08 07:14:14.000000 MeteoGalicia-API-0.0.8/requirements.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       54 2023-08-08 07:54:00.510575 MeteoGalicia-API-0.0.8/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     1838 2023-08-08 07:52:04.000000 MeteoGalicia-API-0.0.8/setup.py
```

### Comparing `MeteoGalicia-API-0.0.7/LICENSE.md` & `MeteoGalicia-API-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MeteoGalicia-API-0.0.7/MeteoGalicia_API.egg-info/PKG-INFO` & `MeteoGalicia-API-0.0.8/MeteoGalicia_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeteoGalicia-API
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python library for get info from MeteoGalicia web service. MeteoGalicia is the meteorological agency for Galicia, Spain
 Home-page: https://github.com/danieldiazi/meteogalicia-api
 Author: danieldiazi
 Author-email: dandiazde@gmail.com
 License: GPLv3
 Description:
```

### Comparing `MeteoGalicia-API-0.0.7/PKG-INFO` & `MeteoGalicia-API-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeteoGalicia-API
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python library for get info from MeteoGalicia web service. MeteoGalicia is the meteorological agency for Galicia, Spain
 Home-page: https://github.com/danieldiazi/meteogalicia-api
 Author: danieldiazi
 Author-email: dandiazde@gmail.com
 License: GPLv3
 Description:
```

### Comparing `MeteoGalicia-API-0.0.7/README.md` & `MeteoGalicia-API-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `MeteoGalicia-API-0.0.7/meteogalicia_api/interface.py` & `MeteoGalicia-API-0.0.8/meteogalicia_api/interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Client for the Meteogalicia REST API."""
 import logging
 from datetime import datetime, timedelta
 import requests
 
 URL_FORECAST = "https://servizos.meteogalicia.gal/mgrss/predicion/jsonPredConcellos.action?idConc={}"
 URL_OBSERVATION = "https://servizos.meteogalicia.gal/mgrss/observacion/observacionConcellos.action?idConcello={}"
-
+URL_OBSERVATION_DAILYDATA_BY_STATION="https://servizos.meteogalicia.gal/mgrss/observacion/datosDiariosEstacionsMeteo.action?idEst={}"
+URL_OBSERVATION_LAST10MINDATA_BY_STATION="https://servizos.meteogalicia.gal/mgrss/observacion/ultimos10minEstacionsMeteo.action?idEst={}"
 
 
 class MeteoGalicia:
     """Class to interact with the MeteoGalicia web service."""
     def __init__( self,  log_level=logging.WARNING):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
@@ -38,8 +39,18 @@
         r = self._do_get(URL_OBSERVATION,id)
         if (r==None):
             self.logger.error(f"No data for code: {id}")
         elif (len(r['listaObservacionConcellos'])==0):
              self.logger.debug(f"No observation data for {id}")
         return r
     
-
+    def get_observation_dailydata_by_station(self,id):
+        r = self._do_get(URL_OBSERVATION_DAILYDATA_BY_STATION,id)
+        if (r==None) or (not('listDatosDiarios1' in r)) or (len(r['listDatosDiarios'])==0):
+             self.logger.debug(f"No observation info (daily data) of station code: {id}")      
+        return r
+    
+    def get_observation_last10mindata_by_station(self,id):
+        r = self._do_get(URL_OBSERVATION_LAST10MINDATA_BY_STATION,id)
+        if (r==None) or (not('listUltimos10min1' in r)) or (len(r['listUltimos10min'])==0):
+             self.logger.debug(f"No observation info (last 10 min data) of station code: {id}")
+        return r
```

### Comparing `MeteoGalicia-API-0.0.7/setup.py` & `MeteoGalicia-API-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 NAME = "MeteoGalicia-API"
 DESCRIPTION = (
     "Python library for get info from MeteoGalicia web service. MeteoGalicia is the meteorological agency for Galicia, Spain"
 )
 URL = "https://github.com/danieldiazi/meteogalicia-api"
 EMAIL = "dandiazde@gmail.com"
 AUTHOR = "danieldiazi"
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 here = lambda *a: os.path.join(os.path.dirname(__file__), *a)
 requirements = [x.strip() for x in open(here('requirements.txt')).readlines()]
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 try:
```


# Comparing `tmp/pyenphase-1.1.0.tar.gz` & `tmp/pyenphase-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.1.0.tar", max compression
+gzip compressed data, was "pyenphase-1.1.1.tar", max compression
```

## Comparing `pyenphase-1.1.0.tar` & `pyenphase-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-08-08 18:50:29.201014 pyenphase-1.1.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-08 18:50:29.201014 pyenphase-1.1.0/README.md
--rw-r--r--   0        0        0     2376 2023-08-08 18:50:30.281072 pyenphase-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1041 2023-08-08 18:50:30.241070 pyenphase-1.1.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8051 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      684 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/const.py
--rw-r--r--   0        0        0    15419 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     2314 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0        0 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2451 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1086 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-08 18:50:29.201014 pyenphase-1.1.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 19:32:10.221692 pyenphase-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-08 19:32:10.221692 pyenphase-1.1.1/README.md
+-rw-r--r--   0        0        0     2376 2023-08-08 19:32:11.461724 pyenphase-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-08-08 19:32:11.421723 pyenphase-1.1.1/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8051 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      684 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/const.py
+-rw-r--r--   0        0        0    15419 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     2314 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2451 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1086 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-08 19:32:10.221692 pyenphase-1.1.1/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.1/PKG-INFO
```

### Comparing `pyenphase-1.1.0/LICENSE` & `pyenphase-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/README.md` & `pyenphase-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/pyproject.toml` & `pyenphase-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.1.0"
+version = "1.1.1"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.1.0/src/pyenphase/__init__.py` & `pyenphase-1.1.1/src/pyenphase/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,17 @@
     EnvoyAuthenticationRequired,
     EnvoyCommunicationError,
     EnvoyError,
     EnvoyFirmwareCheckError,
     EnvoyFirmwareFatalCheckError,
     EnvoyProbeFailed,
 )
+from .models.dry_contacts import EnvoyDryContactSettings, EnvoyDryContactStatus
 from .models.encharge import EnvoyEncharge, EnvoyEnchargePower
+from .models.enpower import EnvoyEnpower
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 
 __all__ = (
     AUTH_TOKEN_MIN_VERSION,
@@ -30,8 +32,11 @@
     "EnvoyAuthenticationRequired",
     "EnvoyProbeFailed",
     "EnvoyInverter",
     "EnvoySystemConsumption",
     "EnvoySystemProduction",
     "EnvoyEncharge",
     "EnvoyEnchargePower",
+    "EnvoyEnpower",
+    "EnvoyDryContactSettings",
+    "EnvoyDryContactStatus",
 )
```

### Comparing `pyenphase-1.1.0/src/pyenphase/auth.py` & `pyenphase-1.1.1/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/const.py` & `pyenphase-1.1.1/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/envoy.py` & `pyenphase-1.1.1/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/exceptions.py` & `pyenphase-1.1.1/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/firmware.py` & `pyenphase-1.1.1/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.1.1/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/encharge.py` & `pyenphase-1.1.1/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/enpower.py` & `pyenphase-1.1.1/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/envoy.py` & `pyenphase-1.1.1/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/inverter.py` & `pyenphase-1.1.1/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/system_consumption.py` & `pyenphase-1.1.1/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/models/system_production.py` & `pyenphase-1.1.1/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/src/pyenphase/ssl.py` & `pyenphase-1.1.1/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.0/PKG-INFO` & `pyenphase-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: pyenphase Version: 1.1.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.1.1 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```


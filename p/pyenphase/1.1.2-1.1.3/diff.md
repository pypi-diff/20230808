# Comparing `tmp/pyenphase-1.1.2.tar.gz` & `tmp/pyenphase-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-1.1.2.tar", max compression
+gzip compressed data, was "pyenphase-1.1.3.tar", max compression
```

## Comparing `pyenphase-1.1.2.tar` & `pyenphase-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-08-08 20:36:25.761374 pyenphase-1.1.2/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-08 20:36:25.761374 pyenphase-1.1.2/README.md
--rw-r--r--   0        0        0     2376 2023-08-08 20:36:26.705377 pyenphase-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-08-08 20:36:26.673377 pyenphase-1.1.2/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     8363 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/auth.py
--rw-r--r--   0        0        0      976 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/const.py
--rw-r--r--   0        0        0    15356 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1272 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     3279 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/firmware.py
--rw-r--r--   0        0        0        0 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2451 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     2673 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     1846 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0     1086 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      873 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1436 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/py.typed
--rw-r--r--   0        0        0     1095 2023-08-08 20:36:25.765374 pyenphase-1.1.2/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 21:28:43.047738 pyenphase-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-08 21:28:43.047738 pyenphase-1.1.3/README.md
+-rw-r--r--   0        0        0     2376 2023-08-08 21:28:44.007747 pyenphase-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1242 2023-08-08 21:28:43.975746 pyenphase-1.1.3/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8363 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      976 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/const.py
+-rw-r--r--   0        0        0    16186 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     3279 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2451 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0     1086 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-08 21:28:43.047738 pyenphase-1.1.3/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.1.3/PKG-INFO
```

### Comparing `pyenphase-1.1.2/LICENSE` & `pyenphase-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/README.md` & `pyenphase-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/pyproject.toml` & `pyenphase-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "1.1.2"
+version = "1.1.3"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-1.1.2/src/pyenphase/__init__.py` & `pyenphase-1.1.3/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/auth.py` & `pyenphase-1.1.3/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/const.py` & `pyenphase-1.1.3/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/envoy.py` & `pyenphase-1.1.3/src/pyenphase/envoy.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,40 @@
 
     @retry(
         retry=retry_if_exception_type(
             (httpx.NetworkError, httpx.TimeoutException, httpx.RemoteProtocolError)
         ),
         wait=wait_random_exponential(multiplier=2, max=3),
     )
+    async def probe_request(self, endpoint: str) -> httpx.Response:
+        """Make a probe request.
+
+        Probe requests are not retried on bad JSON responses.
+        """
+        return await self._request(endpoint)
+
+    @retry(
+        retry=retry_if_exception_type(
+            (
+                httpx.NetworkError,
+                httpx.TimeoutException,
+                httpx.RemoteProtocolError,
+                orjson.JSONDecodeError,
+            )
+        ),
+        wait=wait_random_exponential(multiplier=2, max=3),
+    )
     async def request(self, endpoint: str) -> Any:
+        """Make a request to the Envoy.
+
+        Request retries on bad JSON responses which the Envoy sometimes returns.
+        """
+        return await self._request(endpoint)
+
+    async def _request(self, endpoint: str) -> Any:
         """Make a request to the Envoy."""
         if self.auth is None:
             raise EnvoyAuthenticationRequired(
                 "You must authenticate to the Envoy before making requests."
             )
 
         url = self.auth.get_endpoint_url(endpoint)
@@ -179,15 +204,17 @@
         """Return the Envoy serial number."""
         return self._firmware.serial
 
     async def probe(self) -> None:
         """Probe for model and supported features."""
         for possible_endpoint in (URL_PRODUCTION, URL_PRODUCTION_JSON):
             try:
-                production_json: dict[str, Any] = await self.request(possible_endpoint)
+                production_json: dict[str, Any] = await self.probe_request(
+                    possible_endpoint
+                )
             except ENDPOINT_PROBE_EXCEPTIONS as e:
                 _LOGGER.debug(
                     "Production endpoint not found at %s: %s", possible_endpoint, e
                 )
                 continue
             else:
                 production: list[
@@ -219,37 +246,37 @@
                             if not self._consumption_endpoint:
                                 self._consumption_endpoint = possible_endpoint
 
                 break
 
         if not self._production_endpoint:
             try:
-                await self.request(URL_PRODUCTION_V1)
+                await self.probe_request(URL_PRODUCTION_V1)
             except ENDPOINT_PROBE_EXCEPTIONS as e:
                 _LOGGER.debug(
                     "Production endpoint not found at %s: %s", URL_PRODUCTION_V1, e
                 )
             else:
                 self._production_endpoint = URL_PRODUCTION_V1
 
         if not self._production_endpoint:
             raise EnvoyProbeFailed("Unable to determine production endpoint")
 
         try:
-            await self.request(URL_PRODUCTION_INVERTERS)
+            await self.probe_request(URL_PRODUCTION_INVERTERS)
         except ENDPOINT_PROBE_EXCEPTIONS as e:
             _LOGGER.debug("Inverters endpoint not found: %s", e)
         else:
             self._supported_features |= SupportedFeatures.INVERTERS
 
         # Check for various Ensemble support
         if self._firmware.version >= ENSEMBLE_MIN_VERSION:
             # The Ensemble Inventory endpoint will tell us if we have Enpower or Encharge support
             try:
-                result = await self.request(URL_ENSEMBLE_INVENTORY)
+                result = await self.probe_request(URL_ENSEMBLE_INVENTORY)
             except ENDPOINT_PROBE_EXCEPTIONS as e:
                 _LOGGER.debug("Ensemble Inventory endpoint not found: %s", e)
             else:
                 if not result or "error" in result:
                     # Newer firmware with no Ensemble devices returns an empty list
                     _LOGGER.debug("No Ensemble devices found")
                     return
```

### Comparing `pyenphase-1.1.2/src/pyenphase/exceptions.py` & `pyenphase-1.1.3/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/firmware.py` & `pyenphase-1.1.3/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.1.3/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/encharge.py` & `pyenphase-1.1.3/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/enpower.py` & `pyenphase-1.1.3/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/envoy.py` & `pyenphase-1.1.3/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/inverter.py` & `pyenphase-1.1.3/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/system_consumption.py` & `pyenphase-1.1.3/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/models/system_production.py` & `pyenphase-1.1.3/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/src/pyenphase/ssl.py` & `pyenphase-1.1.3/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-1.1.2/PKG-INFO` & `pyenphase-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 1.1.2
+Version: 1.1.3
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
-Metadata-Version: 2.1 Name: pyenphase Version: 1.1.2 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.1.3 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```


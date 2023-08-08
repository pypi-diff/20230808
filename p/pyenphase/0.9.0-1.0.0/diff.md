# Comparing `tmp/pyenphase-0.9.0.tar.gz` & `tmp/pyenphase-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.9.0.tar", max compression
+gzip compressed data, was "pyenphase-1.0.0.tar", max compression
```

## Comparing `pyenphase-0.9.0.tar` & `pyenphase-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-08-05 22:38:52.350679 pyenphase-0.9.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-05 22:38:52.350679 pyenphase-0.9.0/README.md
--rw-r--r--   0        0        0     2313 2023-08-05 22:38:53.282694 pyenphase-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      931 2023-08-05 22:38:53.250693 pyenphase-0.9.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     7305 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/const.py
--rw-r--r--   0        0        0    10499 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1175 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     4170 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2941 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      833 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      825 2023-08-05 22:38:52.350679 pyenphase-0.9.0/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1388 2023-08-05 22:38:52.354679 pyenphase-0.9.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-05 22:38:52.354679 pyenphase-0.9.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-08-05 22:38:52.354679 pyenphase-0.9.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-08 18:40:36.891816 pyenphase-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-08 18:40:36.891816 pyenphase-1.0.0/README.md
+-rw-r--r--   0        0        0     2376 2023-08-08 18:40:37.999810 pyenphase-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1041 2023-08-08 18:40:37.971810 pyenphase-1.0.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     8051 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0    14257 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1272 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     2314 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     2673 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     1846 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      938 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      873 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1436 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0     1095 2023-08-08 18:40:36.895816 pyenphase-1.0.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-1.0.0/PKG-INFO
```

### Comparing `pyenphase-0.9.0/LICENSE` & `pyenphase-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.9.0/README.md` & `pyenphase-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.9.0/pyproject.toml` & `pyenphase-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.9.0"
+version = "1.0.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
@@ -32,14 +32,17 @@
 envoy-utils = ">=0.0.1"
 orjson = ">=3.9.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 types-orjson = "^3.6.2"
+respx = "^0.20.2"
+pytest-asyncio = "^0.21.1"
+syrupy = "^4.0.8"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `pyenphase-0.9.0/src/pyenphase/__init__.py` & `pyenphase-1.0.0/src/pyenphase/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     EnvoyAuthenticationRequired,
     EnvoyCommunicationError,
     EnvoyError,
     EnvoyFirmwareCheckError,
     EnvoyFirmwareFatalCheckError,
     EnvoyProbeFailed,
 )
+from .models.encharge import EnvoyEncharge, EnvoyEnchargePower
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 
 __all__ = (
     AUTH_TOKEN_MIN_VERSION,
@@ -27,8 +28,10 @@
     "EnvoyFirmwareFatalCheckError",
     "EnvoyAuthenticationError",
     "EnvoyAuthenticationRequired",
     "EnvoyProbeFailed",
     "EnvoyInverter",
     "EnvoySystemConsumption",
     "EnvoySystemProduction",
+    "EnvoyEncharge",
+    "EnvoyEnchargePower",
 )
```

### Comparing `pyenphase-0.9.0/src/pyenphase/auth.py` & `pyenphase-1.0.0/src/pyenphase/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 """Envoy authentication methods."""
 
-import ssl
 from abc import abstractmethod, abstractproperty
-from typing import Any
+from typing import Any, cast
 
 import httpx
+import jwt
 import orjson
 from tenacity import retry, retry_if_exception_type, wait_random_exponential
 
 from .exceptions import EnvoyAuthenticationError
-
-
-def create_default_ssl_context() -> ssl.SSLContext:
-    """Return an default SSL context."""
-    return ssl.create_default_context()
-
-
-_SSL_CONTEXT = create_default_ssl_context()
+from .ssl import SSL_CONTEXT
 
 
 class EnvoyAuth:
     """Base class for Envoy authentication."""
 
     def __init__(self, host: str) -> None:
         """Initialize the EnvoyAuth class."""
@@ -44,14 +37,17 @@
 
     @abstractmethod
     def get_endpoint_url(self, endpoint: str) -> str:
         """Return the URL for the endpoint."""
 
 
 class EnvoyTokenAuth(EnvoyAuth):
+    JSON_LOGIN_URL = "https://enlighten.enphaseenergy.com/login/login.json?"
+    TOKEN_URL = "https://entrez.enphaseenergy.com/tokens"  # nosec
+
     def __init__(
         self,
         host: str,
         cloud_username: str | None = None,
         cloud_password: str | None = None,
         envoy_serial: str | None = None,
         token: str | None = None,
@@ -60,26 +56,15 @@
         self.cloud_username = cloud_username
         self.cloud_password = cloud_password
         self.envoy_serial = envoy_serial
         self._token = token
 
     async def setup(self, client: httpx.AsyncClient) -> None:
         """Obtain the token for Envoy authentication."""
-
         if not self._token:
-            # Raise if we don't have cloud credentials
-            if not self.cloud_username or not self.cloud_password:
-                raise EnvoyAuthenticationError(
-                    "Your firmware requires token authentication, but no cloud credentials were provided to obtain the token."
-                )
-            # Raise if we are missing the envoy serial number
-            if not self.envoy_serial:
-                raise EnvoyAuthenticationError(
-                    "Your firmware requires token authentication, but no envoy serial number was provided to obtain the token."
-                )
             self._token = await self._obtain_token()
 
         # Verify we have adequate credentials
         if not self._token:
             raise EnvoyAuthenticationError(
                 "Unable to obtain token for Envoy authentication."
             )
@@ -95,66 +80,99 @@
                 "Unable to verify token for Envoy authentication."
             )
 
         self._cookies = req.cookies
 
     async def _obtain_token(self) -> None:
         """Obtain the token for Envoy authentication."""
-        # we require a new client that checks SSL certs
-        async with httpx.AsyncClient(verify=_SSL_CONTEXT, timeout=10) as cloud_client:
+        # Raise if we don't have cloud credentials
+        if not self.cloud_username or not self.cloud_password:
+            raise EnvoyAuthenticationError(
+                "Your firmware requires token authentication, "
+                " but no cloud credentials were provided to obtain the token."
+            )
+        # Raise if we are missing the envoy serial number
+        if not self.envoy_serial:
+            raise EnvoyAuthenticationError(
+                "Your firmware requires token authentication, "
+                "but no envoy serial number was provided to obtain the token."
+            )
+        # We require a new client that checks SSL certs
+        async with httpx.AsyncClient(
+            verify=SSL_CONTEXT, timeout=10, follow_redirects=True
+        ) as cloud_client:
             # Login to Enlighten to obtain a session ID
             response = await self._post_json_with_cloud_client(
                 cloud_client,
-                "https://enlighten.enphaseenergy.com/login/login.json?",
+                self.JSON_LOGIN_URL,
                 data={
                     "user[email]": self.cloud_username,
                     "user[password]": self.cloud_password,
                 },
             )
             if response.status_code != 200:
                 raise EnvoyAuthenticationError(
-                    "Unable to login to Enlighten to obtain session ID: "
+                    "Unable to login to Enlighten to obtain session ID from "
+                    f"{self.JSON_LOGIN_URL}: "
                     f"{response.status_code}: {response.text}"
                 )
-            response = orjson.loads(response.text)
+            try:
+                response = orjson.loads(response.text)
+            except orjson.JSONDecodeError as err:
+                raise EnvoyAuthenticationError(
+                    "Unable to decode response from Enlighten: "
+                    f"{response.status_code}: {response.text}"
+                ) from err
+
             self._is_consumer = response["is_consumer"]
             self._manager_token = response["manager_token"]
 
             # Obtain the token
             response = await self._post_json_with_cloud_client(
                 cloud_client,
-                "https://entrez.enphaseenergy.com/tokens",
+                self.TOKEN_URL,
                 json={
                     "session_id": response["session_id"],
                     "serial_num": self.envoy_serial,
                     "username": self.cloud_username,
                 },
             )
             if response.status_code != 200:
                 raise EnvoyAuthenticationError(
-                    "Unable to obtain token for Envoy authentication: "
+                    "Unable to obtain token for Envoy authentication from "
+                    f"{self.TOKEN_URL}: "
                     f"{response.status_code}: {response.text}"
                 )
             return response.text
 
+    async def refresh(self) -> None:
+        """Refresh the token for Envoy authentication."""
+        self._token = await self._obtain_token()
+
+    @property
+    def expire_timestamp(self) -> int:
+        """Return the remaining seconds for the token."""
+        jwt_payload = jwt.decode(self.token, options={"verify_signature": False})
+        return cast(int, jwt_payload["exp"])
+
     @retry(
         retry=retry_if_exception_type(
             (httpx.NetworkError, httpx.TimeoutException, httpx.RemoteProtocolError)
         ),
         wait=wait_random_exponential(multiplier=2, max=3),
     )
     async def _post_json_with_cloud_client(
         self,
-        client: httpx.AsyncClient,
+        cloud_client: httpx.AsyncClient,
         url: str,
         data: dict[str, Any] | None = None,
         json: dict[str, Any] | None = None,
     ) -> httpx.Response:
         """Post to the Envoy API with the cloud client."""
-        return await client.post(url, json=json, data=data)
+        return await cloud_client.post(url, json=json, data=data)
 
     @property
     def token(self) -> str:
         assert self._token is not None  # nosec
         return self._token
 
     @property
```

### Comparing `pyenphase-0.9.0/src/pyenphase/const.py` & `pyenphase-1.0.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.9.0/src/pyenphase/envoy.py` & `pyenphase-1.0.0/src/pyenphase/envoy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,51 @@
-import contextlib
 import enum
-import json
 import logging
-import ssl
 from typing import Any
 
 import httpx
 import orjson
 from awesomeversion import AwesomeVersion
 from envoy_utils.envoy_utils import EnvoyUtils
 from tenacity import retry, retry_if_exception_type, wait_random_exponential
 
 from .auth import EnvoyAuth, EnvoyLegacyAuth, EnvoyTokenAuth
 from .const import (
+    URL_ENCHARGE_BATTERY,
+    URL_ENSEMBLE_INVENTORY,
     URL_PRODUCTION,
     URL_PRODUCTION_INVERTERS,
     URL_PRODUCTION_JSON,
     URL_PRODUCTION_V1,
 )
-from .exceptions import EnvoyAuthenticationRequired, EnvoyProbeFailed
+from .exceptions import (
+    ENDPOINT_PROBE_EXCEPTIONS,
+    EnvoyAuthenticationRequired,
+    EnvoyProbeFailed,
+)
 from .firmware import EnvoyFirmware, EnvoyFirmwareCheckError
+from .models.encharge import EnvoyEncharge, EnvoyEnchargePower
+from .models.enpower import EnvoyEnpower
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
 from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
+from .ssl import NO_VERIFY_SSL_CONTEXT
 
 _LOGGER = logging.getLogger(__name__)
 
 TIMEOUT = 20
 LEGACY_ENVOY_VERSION = AwesomeVersion("3.9.0")
+ENSEMBLE_MIN_VERSION = AwesomeVersion("5.0.0")
 AUTH_TOKEN_MIN_VERSION = AwesomeVersion("7.0.0")
 DEFAULT_HEADERS = {
     "Accept": "application/json",
 }
 
 
-def create_no_verify_ssl_context() -> ssl.SSLContext:
-    """Return an SSL context that does not verify the server certificate.
-    This is a copy of aiohttp's create_default_context() function, with the
-    ssl verify turned off and old SSL versions enabled.
-
-    https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
-    """
-    sslcontext = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-    sslcontext.check_hostname = False
-    sslcontext.verify_mode = ssl.CERT_NONE
-    # Allow all ciphers rather than only Python 3.10 default
-    sslcontext.set_ciphers("DEFAULT")
-    with contextlib.suppress(AttributeError):
-        # This only works for OpenSSL >= 1.0.0
-        sslcontext.options |= ssl.OP_NO_COMPRESSION
-    sslcontext.set_default_verify_paths()
-    return sslcontext
-
-
-_NO_VERIFY_SSL_CONTEXT = create_no_verify_ssl_context()
-
-
 class SupportedFeatures(enum.IntFlag):
     INVERTERS = 1
     METERING = 2
     TOTAL_CONSUMPTION = 4
     NET_CONSUMPTION = 8
     DRY_CONTACTS = 16
     ENCHARGE = 32
@@ -76,21 +61,22 @@
         client: httpx.AsyncClient | None = None,
         timeout: float | None = None,
     ) -> None:
         """Initialize the Envoy class."""
         # We use our own httpx client session so we can disable SSL verification (Envoys use self-signed SSL certs)
         self._timeout = timeout or TIMEOUT
         self._client = client or httpx.AsyncClient(
-            verify=_NO_VERIFY_SSL_CONTEXT
+            verify=NO_VERIFY_SSL_CONTEXT
         )  # nosec
         self.auth: EnvoyAuth | None = None
         self._host = host
         self._firmware = EnvoyFirmware(self._client, self._host)
         self._supported_features: SupportedFeatures = SupportedFeatures(0)
         self._production_endpoint: str | None = None
+        self._consumption_endpoint: str | None = None
         self.data: EnvoyData | None = None
 
     @retry(
         retry=retry_if_exception_type(EnvoyFirmwareCheckError),
         wait=wait_random_exponential(multiplier=2, max=10),
     )
     async def setup(self) -> None:
@@ -111,31 +97,32 @@
             )
             full_serial = self._firmware.serial
             if not username or username == "installer":
                 username = "installer"
                 password = EnvoyUtils.get_password(full_serial, username)
             elif username == "envoy" and not password:
                 # The default password for the envoy user is the first 6 digits of the serial number
+                assert full_serial is not None, "Serial must be set"  # nosec
                 password = full_serial[:6]
 
             if username and password:
                 self.auth = EnvoyLegacyAuth(self.host, username, password)
 
         else:
             # Envoy firmware using new token authentication
             _LOGGER.debug("Authenticating to Envoy using token authentication")
-            if token is not None:
-                self.auth = EnvoyTokenAuth(self.host, token=token)
-            elif (
-                username is not None
-                and password is not None
-                and self._firmware.serial is not None
-            ):
+            if token or (username and password):
+                # Always pass all the data to the token auth class, even if some of it is None
+                # so that we can refresh the token if needed
                 self.auth = EnvoyTokenAuth(
-                    self.host, username, password, self._firmware.serial
+                    self.host,
+                    cloud_username=username,
+                    cloud_password=password,
+                    envoy_serial=self._firmware.serial,
+                    token=token,
                 )
 
         if not self.auth:
             _LOGGER.error(
                 "You must include username/password or token to authenticate to the Envoy."
             )
             raise EnvoyAuthenticationRequired("Could not setup authentication object.")
@@ -151,127 +138,229 @@
     async def request(self, endpoint: str) -> Any:
         """Make a request to the Envoy."""
         if self.auth is None:
             raise EnvoyAuthenticationRequired(
                 "You must authenticate to the Envoy before making requests."
             )
 
+        url = self.auth.get_endpoint_url(endpoint)
         response = await self._client.get(
-            self.auth.get_endpoint_url(endpoint),
+            url,
             headers={**DEFAULT_HEADERS, **self.auth.headers},
             cookies=self.auth.cookies,
             follow_redirects=True,
             auth=self.auth.auth,
             timeout=self._timeout,
         )
-        return orjson.loads(response.text)
+        try:
+            return orjson.loads(response.text)
+        except orjson.JSONDecodeError as e:
+            _LOGGER.debug(
+                "Unable to decode response from Envoy endpoint %s: %s", url, e
+            )
+            raise
 
     @property
     def host(self) -> str:
         """Return the Envoy host."""
         return self._host
 
     @property
     def firmware(self) -> AwesomeVersion:
         """Return the Envoy firmware version."""
         return self._firmware.version
 
     @property
+    def part_number(self) -> str | None:
+        """Return the Envoy part number."""
+        return self._firmware.part_number
+
+    @property
     def serial_number(self) -> str | None:
         """Return the Envoy serial number."""
         return self._firmware.serial
 
     async def probe(self) -> None:
         """Probe for model and supported features."""
-        try:
-            production_json: dict[str, Any] = await self.request(URL_PRODUCTION)
-        except (json.JSONDecodeError, httpx.HTTPError) as e:
-            _LOGGER.debug("Production endpoint not found at %s: %s", URL_PRODUCTION, e)
-        else:
-            production: list[dict[str, str | float | int]] | None = production_json.get(
-                "production"
-            )
-            if production:
-                for type_ in production:
-                    if type_["type"] == "eim" and type_["activeCount"]:
-                        self._supported_features |= SupportedFeatures.METERING
-                        break
-            consumption: list[
-                dict[str, str | float | int]
-            ] | None = production_json.get("consumption")
-            if consumption:
-                for meter in consumption:
-                    meter_type = meter["measurementType"]
-                    if meter_type == "total-consumption" and meter["activeCount"]:
-                        self._supported_features |= SupportedFeatures.TOTAL_CONSUMPTION
-                    elif meter_type == "net-consumption" and meter["activeCount"]:
-                        self._supported_features |= SupportedFeatures.NET_CONSUMPTION
-            self._production_endpoint = URL_PRODUCTION
+        for possible_endpoint in (URL_PRODUCTION, URL_PRODUCTION_JSON):
+            try:
+                production_json: dict[str, Any] = await self.request(possible_endpoint)
+            except ENDPOINT_PROBE_EXCEPTIONS as e:
+                _LOGGER.debug(
+                    "Production endpoint not found at %s: %s", possible_endpoint, e
+                )
+                continue
+            else:
+                production: list[
+                    dict[str, str | float | int]
+                ] | None = production_json.get("production")
+                if production:
+                    for type_ in production:
+                        if type_["type"] == "eim" and type_["activeCount"]:
+                            self._supported_features |= SupportedFeatures.METERING
+                            self._production_endpoint = possible_endpoint
+                            break
+
+                consumption: list[
+                    dict[str, str | float | int]
+                ] | None = production_json.get("consumption")
+                if consumption:
+                    for meter in consumption:
+                        meter_type = meter["measurementType"]
+                        if meter_type == "total-consumption":
+                            self._supported_features |= (
+                                SupportedFeatures.TOTAL_CONSUMPTION
+                            )
+                            if not self._consumption_endpoint:
+                                self._consumption_endpoint = possible_endpoint
+                        elif meter_type == "net-consumption":
+                            self._supported_features |= (
+                                SupportedFeatures.NET_CONSUMPTION
+                            )
+                            if not self._consumption_endpoint:
+                                self._consumption_endpoint = possible_endpoint
 
-        if not self._production_endpoint:
-            for endpoint in (URL_PRODUCTION_V1, URL_PRODUCTION_JSON):
-                try:
-                    await self.request(endpoint)
-                except (json.JSONDecodeError, httpx.HTTPError) as e:
-                    _LOGGER.debug(
-                        "Production endpoint not found at %s: %s", endpoint, e
-                    )
-                    continue
-                self._production_endpoint = endpoint
                 break
 
+        if not self._production_endpoint:
+            try:
+                await self.request(URL_PRODUCTION_V1)
+            except ENDPOINT_PROBE_EXCEPTIONS as e:
+                _LOGGER.debug(
+                    "Production endpoint not found at %s: %s", URL_PRODUCTION_V1, e
+                )
+            else:
+                self._production_endpoint = URL_PRODUCTION_V1
+
+        if not self._production_endpoint:
+            raise EnvoyProbeFailed("Unable to determine production endpoint")
+
         try:
             await self.request(URL_PRODUCTION_INVERTERS)
-        except (json.JSONDecodeError, httpx.HTTPError) as e:
+        except ENDPOINT_PROBE_EXCEPTIONS as e:
             _LOGGER.debug("Inverters endpoint not found: %s", e)
         else:
             self._supported_features |= SupportedFeatures.INVERTERS
 
+        # Check for various Ensemble support
+        if self._firmware.version >= ENSEMBLE_MIN_VERSION:
+            # The Ensemble Inventory endpoint will tell us if we have Enpower or Encharge support
+            try:
+                result = await self.request(URL_ENSEMBLE_INVENTORY)
+            except ENDPOINT_PROBE_EXCEPTIONS as e:
+                _LOGGER.debug("Ensemble Inventory endpoint not found: %s", e)
+            else:
+                if not result or "error" in result:
+                    # Newer firmware with no Ensemble devices returns an empty list
+                    _LOGGER.debug("No Ensemble devices found")
+                    return
+
+                for item in result:
+                    if item["type"] == "ENPOWER":
+                        self._supported_features |= SupportedFeatures.ENPOWER
+                    if item["type"] == "ENCHARGE":
+                        self._supported_features |= SupportedFeatures.ENCHARGE
+        else:
+            _LOGGER.debug("Firmware too old for Ensemble support")
+
     async def update(self) -> EnvoyData:
         """Update data."""
         if not self._production_endpoint:
             await self.probe()
 
-        if not self._production_endpoint:
-            raise EnvoyProbeFailed("Unable to determine production endpoint")
-
         production_endpoint = self._production_endpoint
+        consumption_endpoint = self._consumption_endpoint
         supported_features = self._supported_features
-        system_consumption: EnvoySystemConsumption | None = None
+
         production_data = await self.request(production_endpoint)
-        inverters: dict[str, EnvoyInverter] = {}
         raw = {"production": production_data}
+        if consumption_endpoint == production_endpoint:
+            consumption_data = production_data
+        elif consumption_endpoint:
+            consumption_data = await self.request(consumption_endpoint)
+            raw["consumption"] = consumption_data
 
-        if production_endpoint == URL_PRODUCTION:
-            if (
-                supported_features & SupportedFeatures.TOTAL_CONSUMPTION
-                or supported_features & SupportedFeatures.NET_CONSUMPTION
-            ):
-                system_consumption = EnvoySystemConsumption.from_production(
-                    production_data
-                )
+        inverters: dict[str, EnvoyInverter] = {}
+
+        if production_endpoint in (URL_PRODUCTION, URL_PRODUCTION_JSON):
             system_production = EnvoySystemProduction.from_production(production_data)
         else:
-            # Production endpoint is either URL_PRODUCTION_V1 or URL_PRODUCTION_JSON
+            # Production endpoint is URL_PRODUCTION_V1
             system_production = EnvoySystemProduction.from_v1_api(production_data)
 
+        system_consumption: EnvoySystemConsumption | None = None
+        if consumption_endpoint:
+            system_consumption = EnvoySystemConsumption.from_production(
+                consumption_data
+            )
+
         if supported_features & SupportedFeatures.INVERTERS:
             inverters_data: list[dict[str, Any]] = await self.request(
                 URL_PRODUCTION_INVERTERS
             )
             inverters = {
                 inverter["serialNumber"]: EnvoyInverter.from_v1_api(inverter)
                 for inverter in inverters_data
             }
             raw["inverters"] = inverters_data
 
+        # Update Enpower and Encharge data if supported
+        encharge_inventory: dict[str, EnvoyEncharge] | None = None
+        encharge_power: dict[str, EnvoyEnchargePower] | None = None
+        enpower: EnvoyEnpower | None = None
+
+        if (
+            supported_features & SupportedFeatures.ENCHARGE
+            or supported_features & SupportedFeatures.ENPOWER
+        ):
+            ensemble_inventory_data: list[dict[str, Any]] = await self.request(
+                URL_ENSEMBLE_INVENTORY
+            )
+            raw["ensemble"] = ensemble_inventory_data
+
+            if supported_features & SupportedFeatures.ENCHARGE:
+                encharge_power_data: dict[str, Any] = await self.request(
+                    URL_ENCHARGE_BATTERY
+                )
+                raw["encharge_power"] = encharge_power_data
+                power: dict[str, Any] = {
+                    power["serial_num"]: power
+                    for power in encharge_power_data["devices:"]
+                }
+                inventory: dict[str, Any] = {}
+                for item in ensemble_inventory_data:
+                    if item["type"] != "ENCHARGE":
+                        continue
+                    inventory = {
+                        device["serial_num"]: device for device in item["devices"]
+                    }
+
+                encharge_inventory = {
+                    serial: EnvoyEncharge.from_api(inventory[serial])
+                    for serial in inventory
+                }
+                encharge_power = {
+                    serial: EnvoyEnchargePower.from_api(power[serial])
+                    for serial in power
+                }
+            if supported_features & SupportedFeatures.ENPOWER:
+                for item in ensemble_inventory_data:
+                    if item["type"] != "ENPOWER":
+                        continue
+                    enpower_data = item["devices"][0]
+                raw["enpower"] = enpower_data
+                enpower = EnvoyEnpower.from_api(enpower_data)
+
         data = EnvoyData(
             system_production=system_production,
             system_consumption=system_consumption,
             inverters=inverters,
+            encharge_inventory=encharge_inventory,
+            encharge_power=encharge_power,
+            enpower=enpower,
             # Raw data is exposed so we can __eq__ the data to see if
             # anything has changed and consumers of the library can
             # avoid dispatching data if nothing has changed.
             raw=raw,
         )
         self.data = data
         return data
```

### Comparing `pyenphase-0.9.0/src/pyenphase/exceptions.py` & `pyenphase-1.0.0/src/pyenphase/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+import json
+
+import httpx
+
+ENDPOINT_PROBE_EXCEPTIONS = (json.JSONDecodeError, httpx.HTTPError)
+
+
 class EnvoyError(Exception):
     """Base class for Envoy exceptions."""
 
 
 class EnvoyFirmwareCheckError(EnvoyError):
     """Exception raised when unable to query the Envoy firmware version."""
```

### Comparing `pyenphase-0.9.0/src/pyenphase/firmware.py` & `pyenphase-1.0.0/src/pyenphase/firmware.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,29 @@
 
 from .exceptions import EnvoyFirmwareCheckError, EnvoyFirmwareFatalCheckError
 
 
 class EnvoyFirmware:
     """Class for querying and determining the Envoy firmware version."""
 
+    __slots__ = (
+        "_client",
+        "_host",
+        "_firmware_version",
+        "_serial_number",
+        "_part_number",
+    )
+
     def __init__(self, _client: httpx.AsyncClient, host: str) -> None:
+        """Initialize the Envoy firmware version."""
         self._client = _client
         self._host = host
+        self._firmware_version: str | None = None
+        self._serial_number: str | None = None
+        self._part_number: str | None = None
 
     async def setup(self) -> None:
         """Obtain the firmware version for Envoy authentication."""
         # <envoy>/info will return XML with the firmware version
         try:
             result = await self._client.get(f"http://{self._host}/info")
         except httpx.ConnectError:
@@ -27,20 +39,26 @@
             if (device_tag := xml.find("device")) is not None:
                 if (software_tag := device_tag.find("software")) is not None:
                     self._firmware_version = AwesomeVersion(
                         software_tag.text[1:]
                     )  # need to strip off the leading 'R' or 'D'
                 if (sn_tag := device_tag.find("sn")) is not None:
                     self._serial_number = sn_tag.text
+                if (pn_tag := device_tag.find("pn")) is not None:
+                    self._part_number = pn_tag.text
                 return
 
         else:
             # If we get a different status code, raise an exception
             raise EnvoyFirmwareCheckError(result.status_code, result.text)
 
     @property
     def version(self) -> AwesomeVersion:
         return self._firmware_version
 
     @property
-    def serial(self) -> str:
+    def serial(self) -> str | None:
         return self._serial_number
+
+    @property
+    def part_number(self) -> str | None:
+        return self._part_number
```

### Comparing `pyenphase-0.9.0/src/pyenphase/models/dry_contacts.py` & `pyenphase-1.0.0/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.9.0/src/pyenphase/models/envoy.py` & `pyenphase-1.0.0/src/pyenphase/models/envoy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Model for an envoy."""
 
 from dataclasses import dataclass, field
 from typing import Any
 
 from .dry_contacts import EnvoyDryContact
-from .encharge import EnvoyEncharge
+from .encharge import EnvoyEncharge, EnvoyEnchargePower
 from .enpower import EnvoyEnpower
 from .inverter import EnvoyInverter
 from .system_consumption import EnvoySystemConsumption
 from .system_production import EnvoySystemProduction
 
 
 @dataclass(slots=True)
 class EnvoyData:
     """Model for an envoy."""
 
-    encharge: EnvoyEncharge | None = None
+    encharge_inventory: dict[str, EnvoyEncharge] | None = None
+    encharge_power: dict[str, EnvoyEnchargePower] | None = None
     enpower: EnvoyEnpower | None = None
     system_consumption: EnvoySystemConsumption | None = None
     system_production: EnvoySystemProduction | None = None
     dry_contacts: dict[str, EnvoyDryContact] = field(default_factory=dict)
     inverters: dict[str, EnvoyInverter] = field(default_factory=dict)
     raw: dict[str, dict[str, Any]] = field(default_factory=dict)
```

### Comparing `pyenphase-0.9.0/src/pyenphase/models/inverter.py` & `pyenphase-1.0.0/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.9.0/src/pyenphase/models/system_consumption.py` & `pyenphase-1.0.0/src/pyenphase/models/system_consumption.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     watts_now: int
 
     @classmethod
     def from_production(cls, data: dict[str, Any]) -> EnvoySystemConsumption:
         """Initialize from the production API."""
         consumption = data["consumption"][0]
         return cls(
-            watt_hours_lifetime=consumption["whLifetime"],
-            watt_hours_last_7_days=consumption["whLastSevenDays"],
-            watt_hours_today=consumption["whToday"],
-            watts_now=consumption["wNow"],
+            watt_hours_lifetime=int(round(consumption["whLifetime"])),
+            watt_hours_last_7_days=int(round(consumption["whLastSevenDays"])),
+            watt_hours_today=int(round(consumption["whToday"])),
+            watts_now=int(round(consumption["wNow"])),
         )
```

### Comparing `pyenphase-0.9.0/src/pyenphase/ssl.py` & `pyenphase-1.0.0/src/pyenphase/ssl.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,7 +18,15 @@
         # This only works for OpenSSL >= 1.0.0
         sslcontext.options |= ssl.OP_NO_COMPRESSION
     sslcontext.set_default_verify_paths()
     return sslcontext
 
 
 NO_VERIFY_SSL_CONTEXT = create_no_verify_ssl_context()
+
+
+def create_default_ssl_context() -> ssl.SSLContext:
+    """Return an default SSL context."""
+    return ssl.create_default_context()
+
+
+SSL_CONTEXT = create_default_ssl_context()
```

### Comparing `pyenphase-0.9.0/PKG-INFO` & `pyenphase-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.9.0
+Version: 1.0.0
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
-Metadata-Version: 2.1 Name: pyenphase Version: 0.9.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 1.0.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```


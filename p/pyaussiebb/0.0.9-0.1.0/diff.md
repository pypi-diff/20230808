# Comparing `tmp/pyaussiebb-0.0.9.tar.gz` & `tmp/pyaussiebb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaussiebb-0.0.9.tar", last modified: Sat Aug 28 06:57:56 2021, max compression
+gzip compressed data, was "pyaussiebb-0.1.0.tar", max compression
```

## Comparing `pyaussiebb-0.0.9.tar` & `pyaussiebb-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.181794 pyaussiebb-0.0.9/
--rw-r--r--   0 yaleman    (501) staff       (20)     7787 2021-08-28 06:57:56.181672 pyaussiebb-0.0.9/PKG-INFO
--rw-r--r--   0 yaleman    (501) staff       (20)     7250 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/README.md
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.180518 pyaussiebb-0.0.9/aussiebb/
--rw-r--r--   0 yaleman    (501) staff       (20)    16560 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/aussiebb/__init__.py
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.180743 pyaussiebb-0.0.9/aussiebb/asyncio/
--rw-r--r--   0 yaleman    (501) staff       (20)    22219 2021-08-28 06:32:04.000000 pyaussiebb-0.0.9/aussiebb/asyncio/__init__.py
--rw-r--r--   0 yaleman    (501) staff       (20)     1733 2021-08-28 06:55:58.000000 pyaussiebb-0.0.9/aussiebb/const.py
--rw-r--r--   0 yaleman    (501) staff       (20)      399 2021-08-21 07:50:56.000000 pyaussiebb-0.0.9/aussiebb/exceptions.py
--rw-r--r--   0 yaleman    (501) staff       (20)      364 2021-08-27 05:11:41.000000 pyaussiebb-0.0.9/aussiebb/utils.py
-drwxr-xr-x   0 yaleman    (501) staff       (20)        0 2021-08-28 06:57:56.181513 pyaussiebb-0.0.9/pyaussiebb.egg-info/
--rw-r--r--   0 yaleman    (501) staff       (20)     7787 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/PKG-INFO
--rw-r--r--   0 yaleman    (501) staff       (20)      296 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/SOURCES.txt
--rw-r--r--   0 yaleman    (501) staff       (20)        1 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/dependency_links.txt
--rw-r--r--   0 yaleman    (501) staff       (20)       24 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/requires.txt
--rw-r--r--   0 yaleman    (501) staff       (20)        9 2021-08-28 06:57:56.000000 pyaussiebb-0.0.9/pyaussiebb.egg-info/top_level.txt
--rw-r--r--   0 yaleman    (501) staff       (20)       38 2021-08-28 06:57:56.181828 pyaussiebb-0.0.9/setup.cfg
--rw-r--r--   0 yaleman    (501) staff       (20)      837 2021-08-28 06:56:41.000000 pyaussiebb-0.0.9/setup.py
+-rw-r--r--   0        0        0     1073 2022-03-15 10:47:57.690327 pyaussiebb-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6463 2023-03-28 21:37:40.458981 pyaussiebb-0.1.0/README.md
+-rw-r--r--   0        0        0    18979 2023-08-08 02:29:37.717512 pyaussiebb-0.1.0/aussiebb/__init__.py
+-rw-r--r--   0        0        0    25465 2023-08-08 01:57:31.039610 pyaussiebb-0.1.0/aussiebb/asyncio/__init__.py
+-rw-r--r--   0        0        0     5566 2023-04-30 12:03:33.835084 pyaussiebb-0.1.0/aussiebb/baseclass.py
+-rw-r--r--   0        0        0     4406 2023-08-08 01:56:12.370181 pyaussiebb-0.1.0/aussiebb/const.py
+-rw-r--r--   0        0        0      574 2023-04-30 12:03:33.835596 pyaussiebb-0.1.0/aussiebb/exceptions.py
+-rw-r--r--   0        0        0    10721 2023-08-08 02:30:23.793498 pyaussiebb-0.1.0/aussiebb/types.py
+-rw-r--r--   0        0        0       33 2022-02-04 11:18:19.130969 pyaussiebb-0.1.0/aussiebb/utils.py
+-rw-r--r--   0        0        0     1770 2023-08-08 02:04:48.066296 pyaussiebb-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 pyaussiebb-0.1.0/PKG-INFO
```

### Comparing `pyaussiebb-0.0.9/PKG-INFO` & `pyaussiebb-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: pyaussiebb
-Version: 0.0.9
+Version: 0.1.0
 Summary: Aussie Broadband API module
-Home-page: https://github.com/yaleman/aussiebb
+Home-page: https://github.com/yaleman/pyaussiebb
+License: MIT
+Keywords: api,aussie,broadband,internet
 Author: James Hodgkinson
-Author-email: yaleman@ricetek.net
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: james@terminaloutcomes.com
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: pydantic (>=1.9,<3.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Documentation, https://yaleman.github.io/pyaussiebb/
+Project-URL: Issues, https://github.com/yaleman/pyaussiebb/issues/
+Project-URL: Repository, https://github.com/yaleman/pyaussiebb
 Description-Content-Type: text/markdown
 
 # pyAussieBB
 
-[![Build Status](https://droneio.yaleman.org/api/badges/yaleman/aussiebb/status.svg)](https://droneio.yaleman.org/yaleman/aussiebb)
-
 This is a very simple module for interacting with the Aussie Broadband APIs.
 
-I wrote this so I can pull a line test periodically and show the NBN how garbage they are.
+![ruff](https://github.com/yaleman/aussiebb/actions/workflows/pylint.yml/badge.svg)
+![mypy](https://github.com/yaleman/aussiebb/actions/workflows/mypy.yml/badge.svg)
+![pytest](https://github.com/yaleman/aussiebb/actions/workflows/pytest.yml/badge.svg)
+![Shellcheck](https://github.com/yaleman/aussiebb/actions/workflows/shellcheck.yml/badge.svg)
 
 # Usage
 
 ```
 pip install --user pyaussiebb
 python
 >>> from aussiebb import AussieBB
@@ -43,15 +52,15 @@
 If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
 
 # Development
 
 
 ## Example service tests I've seen
 
-All the "endpoints" below should be tacked onto `aussiebb.BASEURL['api']`.
+All the "endpoints" below should be tacked onto `aussiebb.const.BASEURL['api']`.
 
 **Warning:** `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.
 
 These can be run by using `AussieBB.run_test()` with the string after the last forward-slash as the "test" - ie, `connection` or `linestate`.
 
 ### HFC 
 
@@ -98,24 +107,9 @@
 | `/nbn/{service_id}/connection` | Probably POST | Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/loopback` | Probably POST | Loopback Test | This will test the connectivity between the point NBN’s network transitions to ours and to the closest point to your property. Usually either the Network Termination Device or Node. |
 | `/tests/{service_id}/portreset` | Probably POST | Port Reset | This will reset the connection from the Node and also clear errors that may be causing issues with gaining sync. |
 | `/tests/{service_id}/unidstatus` | Probably POST | UNI-D Status | UNI-D Status will show if the UNI-D port you are currently using has a router connected to it. This will also provide the Link speed your router and UNI-D port are connected at Eg, 100mbit or 1gbit. You will also see the MAC address of the currently connected router. |
 
 # Changelog
 
- * 0.0.3 - Added `get_service_plans` so the gigabit-desperate crowd can check for their new hotness.
- * 0.0.4 - Added `asyncio` submodule, split constants and exceptions out into their own files/modules.
- * 0.0.5/6 - Fixing rate limiting
- * 0.0.7 
-    - Added the following new functions: `account_transactions`, `billing_invoice`, `service_outages`, `service_boltons`, `service_datablocks`, `support_tickets`, `account contacts`. Renamed `get_service_plans` to `service_plans`
- * 0.0.8
-    - renamed serviceid to service_id to match the api
-    - added request_get_json to the sync class
-    - added telephony_usage
-    - added get_appointment which gets service appointments
-    - updated get_usage so it checks the service list and will return telephony data if it's a PhoneMobile service
-    - abstracted how URLS are generated so I don't have to keep adding them twice
-    - added a filter on get_services which allows you to filter by type
-
-
-
+See [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `pyaussiebb-0.0.9/README.md` & `pyaussiebb-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pyAussieBB
 
-[![Build Status](https://droneio.yaleman.org/api/badges/yaleman/aussiebb/status.svg)](https://droneio.yaleman.org/yaleman/aussiebb)
-
 This is a very simple module for interacting with the Aussie Broadband APIs.
 
-I wrote this so I can pull a line test periodically and show the NBN how garbage they are.
+![ruff](https://github.com/yaleman/aussiebb/actions/workflows/pylint.yml/badge.svg)
+![mypy](https://github.com/yaleman/aussiebb/actions/workflows/mypy.yml/badge.svg)
+![pytest](https://github.com/yaleman/aussiebb/actions/workflows/pytest.yml/badge.svg)
+![Shellcheck](https://github.com/yaleman/aussiebb/actions/workflows/shellcheck.yml/badge.svg)
 
 # Usage
 
 ```
 pip install --user pyaussiebb
 python
 >>> from aussiebb import AussieBB
@@ -26,15 +27,15 @@
 If you hit the rate limit it'll raise a `RateLimit` exception. I haven't put that functionality into the blocking version yet, since ... that tends not to hit it. 🤣
 
 # Development
 
 
 ## Example service tests I've seen
 
-All the "endpoints" below should be tacked onto `aussiebb.BASEURL['api']`.
+All the "endpoints" below should be tacked onto `aussiebb.const.BASEURL['api']`.
 
 **Warning:** `/nbn/{service_id}/connection` seems to have both a GET and POST method endpoint - tests on other endpoints may be similar.
 
 These can be run by using `AussieBB.run_test()` with the string after the last forward-slash as the "test" - ie, `connection` or `linestate`.
 
 ### HFC 
 
@@ -81,22 +82,8 @@
 | `/nbn/{service_id}/connection` | Probably POST | Kick Connection | Kick your current session and force your device to reauthenticate |
 | `/tests/{service_id}/loopback` | Probably POST | Loopback Test | This will test the connectivity between the point NBN’s network transitions to ours and to the closest point to your property. Usually either the Network Termination Device or Node. |
 | `/tests/{service_id}/portreset` | Probably POST | Port Reset | This will reset the connection from the Node and also clear errors that may be causing issues with gaining sync. |
 | `/tests/{service_id}/unidstatus` | Probably POST | UNI-D Status | UNI-D Status will show if the UNI-D port you are currently using has a router connected to it. This will also provide the Link speed your router and UNI-D port are connected at Eg, 100mbit or 1gbit. You will also see the MAC address of the currently connected router. |
 
 # Changelog
 
- * 0.0.3 - Added `get_service_plans` so the gigabit-desperate crowd can check for their new hotness.
- * 0.0.4 - Added `asyncio` submodule, split constants and exceptions out into their own files/modules.
- * 0.0.5/6 - Fixing rate limiting
- * 0.0.7 
-    - Added the following new functions: `account_transactions`, `billing_invoice`, `service_outages`, `service_boltons`, `service_datablocks`, `support_tickets`, `account contacts`. Renamed `get_service_plans` to `service_plans`
- * 0.0.8
-    - renamed serviceid to service_id to match the api
-    - added request_get_json to the sync class
-    - added telephony_usage
-    - added get_appointment which gets service appointments
-    - updated get_usage so it checks the service list and will return telephony data if it's a PhoneMobile service
-    - abstracted how URLS are generated so I don't have to keep adding them twice
-    - added a filter on get_services which allows you to filter by type
-
-
+See [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `pyaussiebb-0.0.9/aussiebb/__init__.py` & `pyaussiebb-0.1.0/aussiebb/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,438 +1,534 @@
 """ A class for interacting with Aussie Broadband APIs """
 
-import inspect
-
-import json
-from time import time
+# import json
 import sys
+from time import time
+from typing import Any, Dict, List, Optional, cast
 
-from loguru import logger
 import requests
+import requests.sessions
+
+from .baseclass import BaseClass
+from .const import BASEURL, default_headers, PHONE_TYPES
+from .exceptions import RecursiveDepth
+from .types import (
+    FetchService,
+    MFAMethod,
+    ServiceTest,
+    AccountContact,
+    AccountTransaction,
+    AussieBBOutage,
+    OrderResponse,
+    OrderDetailResponse,
+    OrderDetailResponseModel,
+    GetServicesResponse,
+    VOIPDevice,
+    VOIPDetails,
+)
+
+
+class AussieBB(BaseClass):
+    """A class for interacting with Aussie Broadband APIs"""
+
+    def __init__(
+        self,
+        username: str,
+        password: str,
+        debug: bool = False,
+        services_cache_time: int = 28800,
+        session: Optional[requests.sessions.Session] = None,
+    ):
+        """Setup function
+
+        ```
+        @param username: str - username for Aussie Broadband account
+        @param password: str - password for Aussie Broadband account
+        @param debug: bool - debug mode
+        @param services_cache_time: int
+            - seconds between caching get_services()
+            - defaults to 8 hours
+        @param session : requests.session - session object
+        ```
+        """
+        super().__init__(username, password, debug, services_cache_time)
+        if session is None:
+            self.session = requests.Session()
+        else:
+            self.session = session
 
-from .const import BASEURL, API_ENDPOINTS, default_headers
-from .exceptions import AuthenticationException, RateLimitException, RecursiveDepth
-from .utils import get_url
-
-#pylint: disable=too-many-public-methods,too-many-instance-attributes
-class AussieBB():
-    """ A class for interacting with Aussie Broadband APIs """
-    def __init__(self, username: str, password: str, debug: bool=False, **kwargs):
-        """ Setup function
-
-            ```
-            @param username: str - username for Aussie Broadband account
-            @param password: str - password for Aussie Broadband account
-            @param debug: bool - debug mode
-            @param services_cache_time: int
-                - seconds between caching get_services()
-                - defaults to 8 hours
-            ```
-        """
-        self.username = username
-        self.password = password
-
-        self.debug = debug
-        # TODO: set the debug level in loguru when this is set to False
-
-        if not (username and password):
-            raise AuthenticationException("You need to supply both username and password")
-        self.session = requests.Session()
-
-        self.myaussie_cookie = ""
-        self.token_expires = -1
-
-        self.services_cache_time = kwargs.get('services_cache_time', 28800) # defaults to 8 hours
-        self.services_last_update = -1
-        self.services = None
-
-    def login(self, depth=0):
-        """ Logs into the account and caches the cookie.  """
-        if depth>2:
+    def login(self, depth: int = 0) -> bool:
+        """Logs into the account and caches the cookie."""
+        if depth > 2:
             raise RecursiveDepth("Login recursion depth > 2")
-        logger.debug("Logging in...")
+        self.logger.debug("Logging in...")
 
-        url = BASEURL.get('login')
+        url = BASEURL["login"]
 
         payload = {
-            'username' : self.username,
-            'password' : self.password,
-            }
-        headers = default_headers()
+            "username": self.username,
+            "password": self.password,
+        }
+        headers: Dict[str, Any] = dict(default_headers())
+
+        response = self.session.post(
+            url,
+            headers=headers,
+            json=payload,
+        )
 
-        response = self.session.post(url,
-                                     headers=headers,
-                                     data=json.dumps(payload),
-                                     )
-        if response.status_code == 422:
-            raise AuthenticationException(response.json())
-        if response.status_code == 429:
-            raise RateLimitException(response.json())
         response.raise_for_status()
-
         jsondata = response.json()
 
-        # we expire a little early just because
-        self.token_expires = time() + jsondata.get('expiresIn') - 50
-
-        self.myaussie_cookie = response.cookies.get('myaussie_cookie')
-        if self.myaussie_cookie:
-            logger.debug(f"Login Cookie: {self.myaussie_cookie}")
-        return True
-
-    def _has_token_expired(self):
-        """ Returns bool of if the token has expired """
-        if time() > self.token_expires:
-            return True
-        return False
-
-    def request_get(self, skip_login_check: bool = False, **kwargs):
-        """ Performs a GET request and logs in first if needed.
+        return self._handle_login_response(
+            response.status_code, jsondata, response.cookies
+        )
 
-        Returns the `requests.Response` object."""
+    def do_login_check(self, skip_login_check: bool) -> None:
+        """checks if we're skipping the login check and logs in if necessary"""
         if not skip_login_check:
-            logger.debug("skip_login_check false")
+            self.logger.debug("skip_login_check false")
             if self._has_token_expired():
-                logger.debug("token has expired, logging in...")
+                self.logger.debug("token has expired, logging in...")
                 self.login()
-        if 'cookies' not in kwargs:
-            kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        response = self.session.get(**kwargs)
+
+    def request_get(  # type: ignore
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ):
+        """Performs a GET request and logs in first if needed.
+
+        Returns the `requests.Response` object."""
+        self.do_login_check(skip_login_check)
+        if cookies is None:
+            cookies = {"myaussie_cookie": self.myaussie_cookie}
+
+        response = self.session.get(url=url, cookies=cookies, params=params)
         response.raise_for_status()
         return response
 
-    def request_get_json(self, skip_login_check: bool = False, **kwargs):
-        """ Performs a GET request and logs in first if needed.
+    def request_get_list(
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> List[Any]:
+        """Performs a GET request and logs in first if needed.
+
+        Returns a list from the response.
+        """
+        self.do_login_check(skip_login_check)
+        response = self.session.get(url=url, cookies=cookies, params=params)
+        response.raise_for_status()
+        result: List[Any] = response.json()
+        return result
+
+    def request_get_json(
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Performs a GET request and logs in first if needed.
 
         Returns a dict of the JSON response.
         """
-        if not skip_login_check:
-            logger.debug("skip_login_check false")
-            if self._has_token_expired():
-                logger.debug("token has expired, logging in...")
-                self.login()
-        if 'cookies' not in kwargs:
-            kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        response = self.session.get(**kwargs)
+        self.do_login_check(skip_login_check)
+        response = self.session.get(url=url, cookies=cookies, params=params)
         response.raise_for_status()
-        return response.json()
+        result: Dict[str, Any] = response.json()
+        return result
 
-    def request_post(self, skip_login_check: bool = False, **kwargs):
-        """ Performs a POST request and logs in first if needed."""
-        if not skip_login_check:
-            logger.debug("skip_login_check false")
-            if self._has_token_expired():
-                logger.debug("token has expired, logging in...")
-                self.login()
-        if 'cookies' not in kwargs:
-            kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        if 'headers' not in kwargs:
-            kwargs['headers'] = default_headers()
-        response = self.session.post(**kwargs)
+    def request_post(
+        self, url: str, skip_login_check: bool = False, **kwargs: Dict[str, Any]
+    ) -> requests.Response:
+        """Performs a POST request and logs in first if needed."""
+        self.do_login_check(skip_login_check)
+        if "cookies" not in kwargs:
+            kwargs["cookies"] = {"myaussie_cookie": self.myaussie_cookie}
+
+        if "headers" in kwargs:
+            headers: Dict[str, Any] = kwargs["headers"]
+        else:
+            headers = dict(default_headers())
+
+        response = self.session.post(
+            url=url,
+            headers=headers,
+            **kwargs,  # type: ignore
+        )
         response.raise_for_status()
         return response
 
-    def get_customer_details(self):
-        """ Grabs the customer details.
+    def get_customer_details(self) -> Dict[str, Any]:
+        """Grabs the customer details.
 
-        Returns a dict """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        querystring = {"v":"2"}
-        responsedata = self.request_get_json(url=url,
-                                    params=querystring,
-                                    )
+        Returns a dict"""
+        url = self.get_url("get_customer_details")
+        querystring = {"v": "2"}
+        responsedata = self.request_get_json(
+            url=url,
+            params=querystring,
+        )
         return responsedata
 
+    @property
+    def referral_code(self) -> int:
+        """returns the referral code, which is just the customer number"""
+        response = self.get_customer_details()
+        if "customer_number" not in response:
+            raise ValueError("Couldn't get customer_number from customer_details call.")
+        return int(response["customer_number"])
 
-    def _check_reload_cached_services(self):
-        """ If the age of the service data caching is too old, clear it and re-poll.
+    def _check_reload_cached_services(self) -> bool:
+        """If the age of the service data caching is too old, clear it and re-poll.
 
         Returns bool - if it reloaded the cache.
         """
         if not self.services:
             self.get_services(use_cached=False)
             return True
 
         cache_expiry = self.services_last_update + self.services_cache_time
         if time() >= cache_expiry:
             self.get_services(use_cached=False)
             return True
         return False
 
+    def get_services(
+        self,
+        page: int = 1,
+        use_cached: bool = False,
+        servicetypes: Optional[List[str]] = None,
+        drop_types: Optional[List[str]] = None,
+    ) -> Optional[List[Dict[str, Any]]]:
+        """Returns a `list` of `dicts` of services associated with the account.
 
-    def get_services(self, page: int = 1, servicetypes: list=None, use_cached: bool=False):
-        """ Returns a `list` of `dicts` of services associated with the account.
+        If you want a specific kind of service, or services,
+        provide a list of matching strings in servicetypes.
 
-            If you want a specific kind of service, or services,
-            provide a list of matching strings in servicetypes.
-
-            If you want to use cached data, call it with `use_cached=True`
+        If you want to use cached data, call it with `use_cached=True`
         """
         if use_cached:
-            logger.debug("Using cached data for get_services.")
+            self.logger.debug("Using cached data for get_services.")
             self._check_reload_cached_services()
         else:
-            frame = inspect.currentframe()
-            url = get_url(inspect.getframeinfo(frame).function)
-            querystring = {'page' : page}
-
-            responsedata = self.request_get_json(url=url, params=querystring)
-            # cache the data
-            self.services_last_update = time()
-            self.services = responsedata.get('data')
-
-        # only filter if we need to
-        if servicetypes:
-            logger.debug("Filtering services based on provided list: {}", servicetypes)
-            filtered_responsedata = []
-            for service in self.services:
-                if service.get('type') in servicetypes:
-                    filtered_responsedata.append(service)
-                else:
-                    logger.debug("Skipping as type=={} - {}", service.get('type'), service)
-            return filtered_responsedata
+            url = self.get_url("get_services")
+            services_list: List[Dict[str, Any]] = []
+            while True:
+                params = {"page": page}
+                responsedata = self.request_get_json(url=url, params=params)
+                servicedata = GetServicesResponse.model_validate(responsedata)
+
+                for service in servicedata.data:
+                    services_list.append(service)
+
+                if servicedata.links.next is None:
+                    break
+                url = servicedata.links.next
+                page = servicedata.meta["current_page"]
+
+            self.services = services_list
+            self.services_last_update = int(time())
+
+        self.services = self.filter_services(
+            service_types=servicetypes,
+            drop_types=drop_types,
+        )
 
         return self.services
 
+    def account_transactions(self) -> Dict[str, AccountTransaction]:
+        """Pulls the data for transactions on your account.
 
-    def account_transactions(self):
-        """ Pulls the data for transactions on your account.
+        Returns a dict where the key is the month and year of the transaction.
 
-            Returns a dict where the key is the month and year of the transaction.
+        Keys: `['id', 'type', 'time', 'description', 'amountCents', 'runningBalanceCents']`
 
-            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+        Example output:
 
-            Example output:
-
-            ``` json
-            "August 2021": [
-              {
-                    "id": 12345,
-                    "type": "receipt",
-                    "time": "2021-08-06",
-                    "description": "Payment #12345",
-                    "amountCents": -8400,
-                    "runningBalanceCents": 0
-                }
-            ],
-            ```
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        return self.request_get_json(url=url)
+        ``` json
+        "August 2021": [
+          {
+                "id": 12345,
+                "type": "receipt",
+                "time": "2021-08-06",
+                "description": "Payment #12345",
+                "amountCents": -8400,
+                "runningBalanceCents": 0
+            }
+        ],
+        ```
+        """
+        url = self.get_url("account_transactions")
+        responsedata = self.request_get_json(url=url)
 
+        result: Dict[str, AccountTransaction] = responsedata
+        return result
 
-    def billing_invoice(self, invoice_id):
-        """ Downloads an invoice
+    def billing_invoice(self, invoice_id: int) -> Dict[str, Any]:
+        """Downloads an invoice
 
-            This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
+        This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'invoice_id' : invoice_id})
-        return self.request_get_json(url=url)
+        url = self.get_url("billing_invoice", {"invoice_id": invoice_id})
+        result = self.request_get_json(url=url)
+
+        return result
 
-    def account_paymentplans(self):
-        """ Returns a dict of payment plans for an account """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
+    def account_paymentplans(self) -> Dict[str, Any]:
+        """Returns a dict of payment plans for an account"""
+        url = self.get_url("account_paymentplans")
         return self.request_get_json(url=url)
 
-    def get_usage(self, service_id: int):
+    def get_usage(self, service_id: int, use_cached: bool = True) -> Dict[str, Any]:
         """
         Returns a dict of usage for a service.
 
         If it's a telephony service (`type=PhoneMobile`) it'll pull from the telephony endpoint.
 
         """
+        if self.services is None:
+            self.get_services(use_cached=use_cached)
 
-        if not self.services:
-            self.get_services(use_cached=True)
-        for service in self.services:
-            if service_id == service.get('service_id'):
-                if service.get('type') in ['PhoneMobile']:
-                    return self.telephony_usage(service_id)
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
-        return self.request_get_json(url=url)
+        if self.services is not None:
+            for service in self.services:
+                if service_id == service["service_id"]:
+                    # throw an error if we're trying to parse something we can't
+                    self.validate_service_type(service)
+                    if service["type"] in PHONE_TYPES:
+                        return self.telephony_usage(service_id)
+            url = self.get_url("get_usage", {"service_id": service_id})
+            result = self.request_get_json(url=url)
+
+            return result
+        return {}
 
-    def get_service_tests(self, service_id: int):
-        """ Gets the available tests for a given service ID
+    def get_service_tests(self, service_id: int) -> List[ServiceTest]:
+        """Gets the available tests for a given service ID
         Returns list of dicts
 
         Example data:
 
         ```
         [{
             'name' : str(),
             'description' : str',
             'link' : str(a url to the test)
         },]
         ```
 
         This has a habit of throwing 400 errors if you query a VOIP service...
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
-        return self.request_get_json(url=url)
+        url = self.get_url("get_service_tests", {"service_id": service_id})
+        results: List[ServiceTest] = [
+            ServiceTest.model_validate(test) for test in self.request_get_list(url=url)
+        ]
+        return results
 
-    def get_test_history(self, service_id: int):
-        """ Gets the available tests for a given service ID
+    def get_test_history(self, service_id: int) -> Dict[str, Any]:
+        """Gets the available tests for a given service ID
 
         Returns a list of dicts with tests which have been run
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("get_test_history", {"service_id": service_id})
         return self.request_get_json(url=url)
 
-    def test_line_state(self, service_id: int):
-        """ Tests the line state for a given service ID """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
-        logger.debug("Testing line state, can take a few seconds...")
+    def test_line_state(self, service_id: int) -> Dict[str, Any]:
+        """Tests the line state for a given service ID"""
+        tests = self.get_service_tests(service_id)
+        url = self.get_url("test_line_state", {"service_id": service_id})
+
+        self.is_valid_test(url, tests)
+
+        self.logger.debug("Testing line state, can take a few seconds...")
         response = self.request_post(url=url)
-        return response.json()
+        result: Dict[str, Any] = response.json()
+        return result
 
-    def run_test(self, service_id: int, test_name: str, test_method: str = 'post'):
-        """ Run a test, but it checks it's valid first
+    def run_test(
+        self, service_id: int, test_name: str, test_method: str = "post"
+    ) -> Optional[Dict[str, Any]]:
+        """Run a test, but it checks it's valid first
 
-            There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
+        There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
 
-            See the README for more analysis
+        See the README for more analysis
 
-            - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
-            - 'status' of 'Completed' means you've got the full response
+        - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
+        - 'status' of 'Completed' means you've got the full response
         """
 
-        test_links = [test for test in self.get_service_tests(service_id) if test.get('link', '').endswith(f'/{test_name}')] #pylint: disable=line-too-long
+        test_links = [
+            test
+            for test in self.get_service_tests(service_id)
+            if test.link.endswith(f"/{test_name}")
+        ]
 
         if not test_links:
-            return False
+            return None
         if len(test_links) != 1:
-            logger.debug(f"Too many tests? {test_links}")
+            self.logger.debug("Too many tests? %s", test_links)
 
-        test_name = test_links[0].get('name')
-        logger.debug(f"Running {test_name}")
-        if test_method == 'get':
-            return self.request_get_json(url=test_links[0].get('link'))
-        return self.request_post(url=test_links[0].get('link')).json()
+        test_name = test_links[0].name
+        self.logger.debug("Running %s", test_name)
+        if test_method == "get":
+            return self.request_get_json(url=test_links[0].link)
+        result: Dict[str, Any] = self.request_post(url=test_links[0].link).json()
+        return result
 
-    def service_plans(self, service_id: int):
-        """ Pulls the plan data for a given service.
+    def service_plans(self, service_id: int) -> Dict[str, Any]:
+        """
+        Pulls the plan data for a given service. You MUST MFA-verify first.
 
-            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+        Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
 
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("service_plans", {"service_id": service_id})
         return self.request_get_json(url=url)
 
-    def service_outages(self, service_id: int):
-        """ Pulls outages associated with a service.
+    def service_outages(self, service_id: int) -> Dict[str, Any]:
+        """Pulls outages associated with a service.
 
-            Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
+        Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
 
-            Example data:
-            ```
-            {
-                "networkEvents": [],
-                "aussieOutages": [],
-                "currentNbnOutages": [],
-                "scheduledNbnOutages": [],
-                "resolvedScheduledNbnOutages": [
-                    {
-                        "start_date": "2021-08-17T14:00:00Z",
-                        "end_date": "2021-08-17T20:00:00Z",
-                        "duration": "6.0"
-                    }
-                ],
-                "resolvedNbnOutages": []
-            }
-            ```
+        ```
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
-        return self.request_get_json(url=url)
+        url = self.get_url("service_outages", {"service_id": service_id})
+        data = self.request_get_json(url=url)
+        result = AussieBBOutage.model_validate(data)
+        return result.model_dump()
 
-    def service_boltons(self, service_id: int):
-        """ Pulls addons associated with the service.
+    def service_boltons(self, service_id: int) -> Dict[str, Any]:
+        """Pulls addons associated with the service.
 
-            Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
+        Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
 
-            Example data:
+        Example data:
 
-            ```
-            [{
-                "id": 4,
-                "name": "Small Change Big Change Donation",
-                "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
-                "costCents": 100,
-                "additionalNote": null,
-                "active": false
-            }]
-            ```
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        ```
+        [{
+            "id": 4,
+            "name": "Small Change Big Change Donation",
+            "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
+            "costCents": 100,
+            "additionalNote": null,
+            "active": false
+        }]
+        ```
+        """
+        url = self.get_url("service_boltons", {"service_id": service_id})
         return self.request_get_json(url=url)
 
-    def service_datablocks(self, service_id: int):
-        """ Pulls datablocks associated with the service.
+    def service_datablocks(self, service_id: int) -> Dict[str, Any]:
+        """Pulls datablocks associated with the service.
 
-            Keys: `['current', 'available']`
+        Keys: `['current', 'available']`
 
-            Example data:
+        Example data:
 
-            ```
-            {
-                "current": [],
-                "available": []
-            }
-            ```
+        ```
+        {
+            "current": [],
+            "available": []
+        }
+        ```
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("service_datablocks", {"service_id": service_id})
         return self.request_get_json(url=url)
 
-    def telephony_usage(self, service_id: int):
-        """ Pulls the telephony usage associated with the service.
+    def telephony_usage(self, service_id: int) -> Dict[str, Any]:
+        """Pulls the telephony usage associated with the service.
 
-            Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
+        Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
 
-            Example data:
+        Example data:
 
-            ```
-            {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},"international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},"internet":{"kbytes":0,"cost":0},"voicemail":{"calls":0,"cost":0},"other":{"calls":0,"cost":0},"daysTotal":31,"daysRemaining":2,"historical":[]}
-            ```
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        ```
+        {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},
+        "international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},
+        "internet":{"kbytes":0,"cost":0},
+        "voicemail":{"calls":0,"cost":0},"other":{"calls":0,"cost":0},
+        "daysTotal":31,"daysRemaining":2,"historical":[]}
+        ```
+        """
+        url = self.get_url("telephony_usage", {"service_id": service_id})
         return self.request_get_json(url=url)
 
-    def support_tickets(self):
-        """ Pulls the support tickets associated with the account, returns a list of dicts.
+    def support_tickets(self) -> Dict[str, Any]:
+        """Pulls the support tickets associated with the account, returns a list of dicts.
 
-            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
+        Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
 
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
+        """
+        url = self.get_url("support_tickets")
         return self.request_get_json(url=url)
 
-    def get_appointment(self, ticketid: int):
-        """ Pulls the support tickets associated with the account, returns a list of dicts.
+    def get_appointment(self, ticketid: int) -> Dict[str, Any]:
+        """Pulls the support tickets associated with the account, returns a list of dicts.
 
-            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'ticketid' : ticketid})
+        Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
+        """
+        url = self.get_url("get_appointment", {"ticketid": ticketid})
         return self.request_get_json(url=url)
 
+    def account_contacts(self) -> List[AccountContact]:
+        """Pulls the contacts with the account, returns a list of dicts
 
-    def account_contacts(self):
-        """ Pulls the contacts with the account, returns a list of dicts
+        Dict keys: `['id', 'first_name', 'last_name', 'email', 'dob', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
+        """
+        url = self.get_url("account_contacts")
+        response = self.request_get_json(url=url)
+        return [AccountContact.model_validate(contact) for contact in response]
 
-            Dict keys: `['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        return self.request_get_json(url=url)
+    # TODO: type get_orders
+    def get_orders(self) -> Dict[str, Any]:
+        """pulls the outstanding orders for an account"""
+        url = self.get_url("get_orders")
+        responsedata = self.request_get_json(url=url)
+
+        result = OrderResponse(**responsedata)
+        return result.model_dump()
+
+    def get_order(self, order_id: int) -> OrderDetailResponse:
+        """gets a specific order"""
+        url = self.get_url("get_order", {"order_id": order_id})
+        responsedata = self.request_get_json(url=url)
+        result = cast(
+            OrderDetailResponse,
+            OrderDetailResponseModel.model_validate(responsedata).model_dump(),
+        )
+        return result
+
+    def get_voip_devices(self, service_id: int) -> List[VOIPDevice]:
+        """gets the devices associatd with a VOIP service"""
+        url = self.get_url("voip_devices", {"service_id": service_id})
+        service_list: List[VOIPDevice] = []
+        for service in self.request_get_json(url=url):
+            service_list.append(VOIPDevice.model_validate(service))
+        return service_list
+
+    def get_voip_service(self, service_id: int) -> VOIPDetails:
+        """gets the details of a VOIP service"""
+        url = self.get_url("voip_service", {"service_id": service_id})
+        return VOIPDetails.model_validate(self.request_get_json(url=url))
+
+    def get_fetch_service(self, service_id: int) -> FetchService:
+        """gets the details of a Fetch service"""
+        url = self.get_url("fetch_service", {"service_id": service_id})
+        return FetchService.model_validate(self.request_get_json(url=url))
+
+    async def mfa_send(self, method: MFAMethod) -> None:
+        """sends an MFA code to the user"""
+        url = self.get_url("mfa_send")
+        print(method.model_dump(), file=sys.stderr)
+        self.request_post(url=url, data=method.model_dump())
+
+    async def mfa_verify(self, token: str) -> None:
+        """got the token from send_mfa? send it back to validate it"""
+        url = self.get_url("mfa_verify")
+        self.request_post(url=url, data={"token": token})
```

### Comparing `pyaussiebb-0.0.9/aussiebb/asyncio/__init__.py` & `pyaussiebb-0.1.0/aussiebb/asyncio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,357 +1,446 @@
 """ aiohttp support for AussieBB """
 
 
 import asyncio
 
-import inspect
 import json
 from time import time
-
 import sys
+from typing import Any, Dict, List, Optional
+
 try:
     import aiohttp
+    from aiohttp.client import ClientResponse
 except ImportError as error_message:
     print(f"Failed to import aiohttp, bailing: {error_message}", file=sys.stderr)
     sys.exit(1)
 
-from ..const import BASEURL, default_headers, DEFAULT_BACKOFF_DELAY
-from ..exceptions import AuthenticationException, RateLimitException, RecursiveDepth
-from ..utils import get_url
-
-
-class AussieBB(): #pylint: disable=too-many-public-methods,too-many-instance-attributes
-    """ aiohttp class for interacting with Aussie Broadband APIs """
-    def __init__(self, username: str, password: str, session: aiohttp.client.ClientSession=None, debug: bool=False, **kwargs):
-        """ Setup function
-
-            ```
-            @param username: str - username for Aussie Broadband account
-            @param password: str - password for Aussie Broadband account
-            @param debug: bool - debug mode
-            @param services_cache_time: int
-                - seconds between caching get_services()
-                - defaults to 8 hours
-            ```
-        """
-        self.username = username
-        self.password = password
-        if not (username and password):
-            raise AuthenticationException("You need to supply both username and password")
+from ..baseclass import BaseClass
+from ..const import BASEURL, default_headers, DEFAULT_BACKOFF_DELAY, PHONE_TYPES
+from ..exceptions import (
+    AuthenticationException,
+    RateLimitException,
+    RecursiveDepth,
+)
+
+from ..types import (
+    MFAMethod,
+    ServiceTest,
+    AccountContact,
+    AccountTransaction,
+    FetchService,
+    OrderDetailResponseModel,
+    GetServicesResponse,
+    VOIPDevice,
+    VOIPDetails,
+)
+
+
+class AussieBB(BaseClass):
+    """aiohttp class for interacting with Aussie Broadband APIs"""
+
+    def __init__(
+        self,
+        username: str,
+        password: str,
+        session: Optional[aiohttp.client.ClientSession] = None,
+        debug: bool = False,
+        services_cache_time: int = 28800,
+    ):
+        """Setup function
+
+        ```
+        @param username: str - username for Aussie Broadband account
+        @param password: str - password for Aussie Broadband account
+        @param debug: bool - debug mode
+        @param services_cache_time: int
+            - seconds between caching get_services()
+            - defaults to 8 hours
+        ```
+        """
+        super().__init__(username, password, debug, services_cache_time)
 
         if not session:
             self.session = aiohttp.ClientSession()
         else:
             self.session = session
 
-        self.myaussie_cookie = ""
-        self.token_expires = -1
-        self.debug = debug
-
-        self.services_cache_time = kwargs.get('services_cache_time', 28800) # defaults to 8 hours
-        self.services_last_update = -1
-        self.services = None
-
-
-    def _debug_print(self, message: str):
-        """ Prints a debug message to stderr if the class is in debug mode. """
-        if self.debug:
-            print(message, file=sys.stderr)
-
-    async def login(self, depth=0):
-        """ Logs into the account and caches the cookie.  """
-        if depth>2:
+    async def login(self, depth: int = 0) -> bool:
+        """Logs into the account and caches the cookie."""
+        if depth > 2:
             raise RecursiveDepth("Login recursion depth > 2")
-        self._debug_print("Logging in...")
+        self.logger.debug("Logging in...")
 
-        url = BASEURL.get('login')
+        url = BASEURL["login"]
 
         if not self._has_token_expired():
             return True
 
         payload = {
-            'username' : self.username,
-            'password' : self.password,
-            }
+            "username": self.username,
+            "password": self.password,
+        }
         headers = default_headers()
 
-        async with self.session.post(url=url, headers=headers, json=payload) as response:
+        async with self.session.post(
+            url=url,
+            headers=headers,
+            json=payload,
+        ) as response:
             try:
                 await self.handle_response_fail(response)
                 jsondata = await response.json()
             except RateLimitException:
-                return await self.login(depth+1)
-            self._debug_print(f"Login response status: {response.status}")
-        self._debug_print(f"Dumping login response: {json.dumps(jsondata)}")
-
-        # we expire a little early just because
-        self.token_expires = time() + jsondata.get('expiresIn') - 50
-        self.myaussie_cookie = response.cookies.get('myaussie_cookie')
-        if self.myaussie_cookie:
-            self._debug_print(f"Login Cookie: {self.myaussie_cookie}")
-        return True
-
-    async def handle_response_fail(self, response, wait_on_rate_limit: bool=True):
-        """ Handles response status codes. Tries to gracefully handle the rate limiting.
+                return await self.login(depth + 1)
+            self.logger.debug("Login response status: %s", response.status)
+        self.logger.debug("Dumping login response: %s", json.dumps(jsondata))
+
+        return self._handle_login_response(response.status, jsondata, response.cookies)
+
+    async def handle_response_fail(
+        self,
+        response: ClientResponse,
+        wait_on_rate_limit: bool = True,
+    ) -> None:
+        """Handles response status codes. Tries to gracefully handle the rate limiting.
 
         ```
         @param response - aiohttp.Response - the full response object
         @param wait_on_rate_limit - bool - if hitting a rate limit, async wait on the time limit
         ```
         """
-        ratelimit_remaining = int(response.headers.get('x-ratelimit-remaining', -1))
-        self._debug_print(f"Rate limit header: {response.headers.get('x-ratelimit-remaining', -1)}")
+        ratelimit_remaining = int(response.headers.get("X-RateLimit-Remaining", -1))
+        self.logger.debug(
+            "Rate limit header: %s", response.headers.get("X-RateLimit-Remaining", -1)
+        )
         if ratelimit_remaining < 5 and wait_on_rate_limit:
-            print("Rate limit below 5, sleeping for 1 second.", file=sys.stderr)
+            self.logger.info("Rate limit below 5, sleeping for 1 second.")
             await asyncio.sleep(1)
 
         if response.status == 422:
             raise AuthenticationException(await response.json())
         if response.status == 429:
             jsondata = await response.json()
-            self._debug_print(f"Dumping headers: {response.headers}")
-            self._debug_print(f"Dumping response: {jsondata}")
+            self.logger.debug("Dumping headers: %s", response.headers)
+            self.logger.debug("Dumping response: %s", json.dumps(jsondata, default=str))
             delay = DEFAULT_BACKOFF_DELAY
-            if 'Please try again in ' in str(jsondata.get('errors')):
+            if "Please try again in " in str(jsondata.get("errors")):
                 fallback_value = [f"default {DEFAULT_BACKOFF_DELAY} seconds"]
-                delay = jsondata.get('errors', {}).get('username', fallback_value)[0].split()[-2]
+                delay = (
+                    jsondata.get("errors", {})
+                    .get("username", fallback_value)[0]
+                    .split()[-2]
+                )
                 # give it some extra time to cool off
-                delay = int(delay)+5
+                delay = int(delay) + 5
 
                 if 0 < delay < 1000:
-                    self._debug_print(f"Found delay: {delay}")
+                    self.logger.debug("Found required rate limit delay: %s", delay)
                     delay = int(delay)
                 else:
-                    self._debug_print(f"Couldn't parse delay, using default: {delay}")
+                    self.logger.debug(
+                        "Couldn't parse rate limit delay, using default: %s", delay
+                    )
             else:
                 delay = DEFAULT_BACKOFF_DELAY
-                if self.debug:
-                    print(f"Couldn't parse delay, using default: {delay}", file=sys.stderr)
+                self.logger.debug("Couldn't parse delay, using default: %s", delay)
             if wait_on_rate_limit:
-                print(f"Rate limit on Aussie API calls raised, sleeping for {delay} seconds.", file=sys.stderr)
+                self.logger.debug(
+                    "Rate limit on Aussie API calls raised, sleeping for %s seconds.",
+                    delay,
+                )
                 await asyncio.sleep(delay)
             raise RateLimitException(jsondata)
+        if response.status == 500:
+            self.logger.error("AussieBB API returned 500, dumping headers.")
+            self.logger.error(response.headers)
+            self.logger.error("body: %s", await response.content.read())
         response.raise_for_status()
 
-    def _has_token_expired(self):
-        """ Returns bool of if the token has expired """
-        if time() > self.token_expires:
-            return True
-        return False
+    async def do_login_check(self, skip_login_check: bool) -> None:
+        """checks if we're skipping the login check and logs in if necessary"""
+        if not skip_login_check:
+            self.logger.debug("skip_login_check false")
+            if self._has_token_expired():
+                self.logger.debug("token has expired, logging in...")
+                await self.login()
 
-    async def request_get(self, skip_login_check: bool = False, **kwargs) -> dict:
-        """ Performs a GET request and logs in first if needed. """
-        depth = kwargs.get('depth', 0)
+    async def request_get(
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        depth: int = 0,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> ClientResponse:
+        """Performs a GET request and logs in first if needed."""
         if depth > 2:
             raise RecursiveDepth(f"depth: {depth}")
 
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
-        if not skip_login_check:
-            if self._has_token_expired():
-                if self.debug:
-                    print("token has expired, logging in...", file=sys.stderr)
-                await self.login()
+        await self.do_login_check(skip_login_check)
 
-        if 'cookies' not in kwargs:
-            kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        async with self.session.get(**kwargs) as response:
-            try:
-                await self.handle_response_fail(response)
-                await response.read()
-            except RateLimitException:
-                response = await self.request_get(skip_login_check, **kwargs)
-            return response
+        if cookies is None:
+            cookies = {"myaussie_cookie": self.myaussie_cookie}
 
-    async def request_get_json(self, skip_login_check: bool = False, **kwargs) -> dict:
-        """ Performs a GET request and logs in first if needed.
+        # telling it where we're coming from
+        headers = {
+            "referer": "https://my.aussiebroadband.com.au/",
+            "x-two-factor-auth-capable-client": "false",  # this might need to be a thing...
+        }
+        response: ClientResponse = await self.session.get(
+            url=url, cookies=cookies, params=params, headers=headers
+        )
+        try:
+            await self.handle_response_fail(response)
+            await response.read()
+        except RateLimitException:
+            response = await self.request_get(
+                url=url,
+                skip_login_check=skip_login_check,
+                depth=depth,
+                cookies=cookies,
+                params=params,
+            )
+        return response
 
-        Returns a dict of the JSON response.
-        """
-        depth = kwargs.get('depth', 0)
-        if depth > 2:
-            raise RecursiveDepth(f"depth: {depth}")
+    async def request_get_list(
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        depth: int = 0,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> List[Any]:
+        """Performs a GET request and logs in first if needed.
 
-        if self.session is None:
-            self.session = aiohttp.ClientSession()
+        Returns a list from the JSON response.
+        """
+        response = await self.request_get(url, skip_login_check, depth, cookies, params)
+        result: List[Any] = await response.json()
+        return result
 
-        if not skip_login_check:
-            if self.debug:
-                print("skip_login_check false", file=sys.stderr)
-            if self._has_token_expired():
-                if self.debug:
-                    print("token has expired, logging in...", file=sys.stderr)
-                await self.login()
+    async def request_get_json(
+        self,
+        url: str,
+        skip_login_check: bool = False,
+        depth: int = 0,
+        cookies: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Performs a GET request and logs in first if needed.
 
-        if 'cookies' not in kwargs:
-            kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        async with self.session.get(**kwargs) as response:
-            try:
-                await self.handle_response_fail(response)
-                jsondata = await response.json()
-            except RateLimitException:
-                jsondata = await self.request_get_json(skip_login_check, **kwargs)
-        return jsondata
+        Returns a dict of the JSON response.
+        """
+        response = await self.request_get(url, skip_login_check, depth, cookies, params)
+        result: Dict[str, Any] = await response.json()
+        return result
 
-    async def request_post_json(self, url, **kwargs):
-        """ Performs a POST request and logs in first if needed.
+    async def request_post_json(
+        self,
+        url: str,
+        depth: int = 0,
+        skip_login_check: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> Dict[str, Any]:
+        """Performs a POST request and logs in first if needed.
 
         Returns a dict of the response data.
         """
-        depth = kwargs.get('depth', 0)
         if depth > 2:
             raise RecursiveDepth(f"depth: {depth}")
 
         if self.session is None:
             self.session = aiohttp.ClientSession()
 
-        if not kwargs.get('skip_login_check', False):
-            if self.debug:
-                print("skip_login_check false", file=sys.stderr)
-            if self._has_token_expired():
-                if self.debug:
-                    print("token has expired, logging in...", file=sys.stderr)
-                await self.login()
+        await self.do_login_check(skip_login_check)
 
-        #if 'cookies' not in kwargs:
-        #    kwargs['cookies'] = {'myaussie_cookie' : self.myaussie_cookie}
-        cookies = kwargs.get('cookies', {'myaussie_cookie' : self.myaussie_cookie})
-        headers = kwargs.get('headers', default_headers())
-        async with self.session.post(url=url, cookies=cookies, headers=headers) as response:
+        cookies = kwargs.get("cookies", {"myaussie_cookie": self.myaussie_cookie})
+        headers = kwargs.get("headers", default_headers())
+        async with self.session.post(
+            url=url, cookies=cookies, headers=headers, json=kwargs.get("data")
+        ) as response:
             try:
                 await self.handle_response_fail(response)
-                jsondata = await response.json()
+                jsondata: Dict[str, Any] = await response.json()
             except RateLimitException:
-                jsondata = await self.request_post_json(url=url, depth=depth+1, **kwargs)
+                jsondata = await self.request_post_json(
+                    url=url,
+                    depth=depth + 1,
+                    skip_login_check=skip_login_check,
+                    **kwargs,
+                )
         return jsondata
 
-    async def get_customer_details(self) -> dict:
-        """ Grabs the customer details.
+    async def get_customer_details(self) -> Dict[str, Any]:
+        """Grabs the customer details.
 
-        Returns a dict """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        params = {"v":"2"}
-        return await self.request_get_json(url=url,
-                                    params=params,
-                                    )
+        Returns a dict"""
 
-    async def _check_reload_cached_services(self):
-        """ If the age of the service data caching is too old, clear it and re-poll.
+        url = self.get_url("get_customer_details")
+        result: Dict[str, Any] = await self.request_get_json(
+            url=url,
+            params={"v": "2"},
+        )
+        return result
+
+    @property
+    async def referral_code(self) -> int:
+        """returns the referral code, which is just the customer number"""
+        response = await self.get_customer_details()
+        if "customer_number" not in response:
+            raise ValueError("Couldn't get customer_number from customer_details call.")
+        return int(response["customer_number"])
+
+    async def _check_reload_cached_services(self) -> bool:
+        """If the age of the service data caching is too old, clear it and re-poll.
 
         Returns bool - if it reloaded the cache.
         """
         if not self.services:
             await self.get_services(use_cached=False)
             return True
         cache_expiry = self.services_last_update + self.services_cache_time
         if time() >= cache_expiry:
             await self.get_services(use_cached=False)
             return True
         return False
 
-    async def get_services(self, page: int=1, servicetypes: list=None, use_cached: bool=False):
-        """ Returns a `list` of `dicts` of services associated with the account.
+    async def get_services(
+        self,
+        page: int = 1,
+        use_cached: bool = False,
+        servicetypes: Optional[List[str]] = None,
+        drop_types: Optional[List[str]] = None,
+    ) -> List[Dict[str, Any]]:
+        """Returns a `list` of `dicts` of services associated with the account.
+
+        If you want a specific kind of service, or services,
+        provide a list of matching strings in servicetypes.
 
-            If you want a specific kind of service, or services,
-            provide a list of matching strings in servicetypes.
+        If you want to use cached data, call it with `use_cached=True`
 
-            If you want to use cached data, call it with `use_cached=True`
+        If you want to drop service types, then pass a list of strings to drop_types
         """
         if use_cached:
-            self._debug_print("Using cached data for get_services.")
+            self.logger.debug("Using cached data for get_services.")
             await self._check_reload_cached_services()
         else:
-            frame = inspect.currentframe()
-            url = get_url(inspect.getframeinfo(frame).function)
-            params = {'page' : page}
-
-            responsedata = await self.request_get_json(url=url, params=params)
-            # cache the data
-            self.services_last_update = time()
-            self.services = responsedata.get('data')
-
-        # only filter if we need to
-        if servicetypes:
-            self._debug_print(f"Filtering services based on provided list: {servicetypes}")
-            filtered_responsedata = []
-            for service in self.services:
-                if service.get('type') in servicetypes:
-                    filtered_responsedata.append(service)
-                else:
-                    self._debug_print(f"Skipping as type=={service.get('type')} - {service}")
-            return filtered_responsedata
+            url = self.get_url("get_services")
+            services_list: List[Dict[str, Any]] = []
+            while True:
+                params = {"page": page}
+                responsedata = await self.request_get_json(url=url, params=params)
+                servicedata = GetServicesResponse.model_validate(responsedata)
+
+                for service in servicedata.data:
+                    services_list.append(service)
+
+                if servicedata.links.next is None:
+                    break
+                url = servicedata.links.next
+                page = servicedata.meta["current_page"]
+
+            self.services = services_list
+            self.services_last_update = int(time())
+
+        # TODO: validate the expected fields in the service (type, name, plan, description, service_id at a minimum)
+
+        self.services = self.filter_services(
+            service_types=servicetypes,
+            drop_types=drop_types,
+        )
 
         return self.services
 
-    async def account_transactions(self):
-        """ Pulls the data for transactions on your account.
+    async def account_transactions(self) -> Dict[str, AccountTransaction]:
+        """Pulls the data for transactions on your account.
 
-            Returns a dict where the key is the month and year of the transaction.
+        Returns a dict where the key is the month and year of the transaction.
 
-            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+        Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
 
-            Example output:
+        Example output:
 
-            ``` json
-            "August 2021": [
-              {
-                    "id": 12345,
-                    "type": "receipt",
-                    "time": "2021-08-06",
-                    "description": "Payment #12345",
-                    "amountCents": -8400,
-                    "runningBalanceCents": 0
-                }
-            ],
-            ```
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        responsedata = await self.request_get_json(url=url)
+        ``` json
+        "August 2021": [
+          {
+                "id": 12345,
+                "type": "receipt",
+                "time": "2021-08-06",
+                "description": "Payment #12345",
+                "amountCents": -8400,
+                "runningBalanceCents": 0
+            }
+        ],
+        ```
+        """
+        url = self.get_url("account_transactions")
+        responsedata: Dict[str, AccountTransaction] = await self.request_get_json(
+            url=url
+        )
         return responsedata
 
-    async def billing_invoice(self, invoice_id):
-        """ Downloads an invoice
+    async def billing_receipt(self, receipt_id: int) -> ClientResponse:
+        """Downloads a receipt
 
-            This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
+        This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'invoice_id', invoice_id})
-        responsedata = await self.request_get_json(url=url)
+        return await self.billing_download("receipt", receipt_id)
+
+    async def billing_invoice(self, invoice_id: int) -> ClientResponse:
+        """Downloads an invoice
+
+        This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
+        """
+        return await self.billing_download("invoice", invoice_id)
+
+    async def billing_download(
+        self, download_type: str, item_id: int
+    ) -> ClientResponse:
+        """Downloads a billing file
+
+        This returns the bare response object, parsing the result is an exercise for the consumer. It's a PDF file.
+        """
+        url = f"{self.BASEURL.get('api')}/billing/{download_type}s/{item_id}"
+
+        responsedata = await self.request_get(url=url)
         return responsedata
 
-    async def account_paymentplans(self):
-        """ Returns a dict of payment plans for an account """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
+    async def account_paymentplans(self) -> Dict[str, Any]:
+        """Returns a dict of payment plans for an account"""
+        url = self.get_url("account_paymentplans")
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
-    async def get_usage(self, service_id: int):
+    async def get_usage(
+        self, service_id: int, use_cached: bool = True
+    ) -> Dict[str, Any]:
         """
         Returns a dict of usage for a service.
 
-        If it's a telephony service (`type=PhoneMobile`) it'll pull from the telephony endpoint.
+        If it's a telephony service (`type in aussiebb.const.PHONE_TYPES`) it'll pull from the telephony endpoint.
 
         """
-        services = await self.get_services(use_cached=True)
+        services = await self.get_services(use_cached=use_cached)
         for service in services:
-            if service_id == service.get('service_id'):
-                if service.get('type') in ['PhoneMobile']:
+            if service_id == service["service_id"]:
+                # throw an error if we're trying to parse something we can't
+                self.validate_service_type(service)
+                if service["type"] in PHONE_TYPES:
                     return await self.telephony_usage(service_id)
-
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("get_usage", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
-    async def get_service_tests(self, service_id: int):
-        """ Gets the available tests for a given service ID
+    async def get_service_tests(self, service_id: int) -> List[ServiceTest]:
+        """Gets the available tests for a given service ID
         Returns list of dicts
 
         Example data:
 
         ```
         [{
             'name' : str(),
@@ -360,209 +449,244 @@
         },]
         ```
 
         This has a habit of throwing 400 errors if you query a VOIP service...
         """
         if self.debug:
             print(f"Getting service tests for {service_id}", file=sys.stderr)
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        responsedata = await self.request_get_json(url=url)
-        return responsedata
 
-    async def get_test_history(self, service_id: int):
-        """ Gets the available tests for a given service ID
+        url = self.get_url("get_service_tests", {"service_id": service_id})
+        responsedata: List[Any] = await self.request_get_list(url=url)
+        return [ServiceTest.model_validate(test) for test in responsedata]
+
+    async def get_test_history(self, service_id: int) -> Dict[str, Any]:
+        """Gets the available tests for a given service ID
 
         Returns a list of dicts with tests which have been run
         """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+
+        url = self.get_url("get_test_history", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
         return responsedata
 
-    async def test_line_state(self, service_id: int):
-        """ Tests the line state for a given service ID """
+    async def test_line_state(self, service_id: int) -> Dict[str, Any]:
+        """Tests the line state for a given service ID"""
+        tests = await self.get_service_tests(service_id)
+        url = self.get_url("test_line_state", {"service_id": service_id})
 
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        self.is_valid_test(url, tests)
 
-        if self.debug:
-            print("Testing line state, can take a few seconds...")
+        # if self.debug:
+        # print("Testing line state, can take a few seconds...")
         response = await self.request_post_json(url=url)
-        if self.debug:
-            print(f"Response: {response}", file=sys.stderr)
+        # if self.debug:
+        # print(f"Response: {response}", file=sys.stderr)
         return response
 
-    async def run_test(self, service_id: int, test_name: str, test_method: str = 'post'):
-        """ Run a test, but it checks it's valid first
+    async def run_test(
+        self, service_id: int, test_name: str, test_method: str = "post"
+    ) -> Optional[Dict[str, Any]]:
+        """Run a test, but it checks it's valid first
 
-            There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
+        There doesn't seem to be a valid way to identify what method you're supposed to use on each test.
 
-            See the README for more analysis
+        See the README for more analysis
 
-            - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
-            - 'status' of 'Completed' means you've got the full response
+        - 'status' of 'InProgress' use 'AussieBB.get_test_history()' and look for the 'id'
+        - 'status' of 'Completed' means you've got the full response
         """
 
         service_tests = await self.get_service_tests(service_id)
-        test_links = [test for test in service_tests if test.get('link', '').endswith(f'/{test_name}')] #pylint: disable=line-too-long
+        test_links = [
+            test for test in service_tests if test.link.endswith(f"/{test_name}")
+        ]
 
         if not test_links:
-            return False
+            return None
         if len(test_links) != 1:
             if self.debug:
                 print(f"Too many tests? {test_links}", file=sys.stderr)
 
-        test_name = test_links[0].get('name')
+        test_name = test_links[0].name
         if self.debug:
             print(f"Running {test_name}", file=sys.stderr)
-        if test_method == 'get':
-            result = await self.request_get_json(url=test_links[0].get('link'))
+        if test_method == "get":
+            result = await self.request_get_json(url=test_links[0].link)
         else:
-            result = await self.request_post_json(url=test_links[0].get('link'))
+            result = await self.request_post_json(url=test_links[0].link)
         return result
 
-    async def service_plans(self, service_id: int):
-        """ Pulls the plan data for a given service.
+    async def service_plans(self, service_id: int) -> Dict[str, Any]:
+        """
+        Pulls the plan data for a given service. You MUST MFA-verify first.
 
-            Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
+        Keys: `['current', 'pending', 'available', 'filters', 'typicalEveningSpeeds']`
 
         """
 
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("service_plans", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def service_outages(self, service_id: int):
-        """ Pulls outages associated with a service.
+    async def service_outages(self, service_id: int) -> Dict[str, Any]:
+        """Pulls outages associated with a service.
 
-            Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
+        Keys: `['networkEvents', 'aussieOutages', 'currentNbnOutages', 'scheduledNbnOutages', 'resolvedScheduledNbnOutages', 'resolvedNbnOutages']`
 
-            Example data:
-            ```
-            {
-                "networkEvents": [],
-                "aussieOutages": [],
-                "currentNbnOutages": [],
-                "scheduledNbnOutages": [],
-                "resolvedScheduledNbnOutages": [
-                    {
-                        "start_date": "2021-08-17T14:00:00Z",
-                        "end_date": "2021-08-17T20:00:00Z",
-                        "duration": "6.0"
-                    }
-                ],
-                "resolvedNbnOutages": []
-            }
-            ```
+        Example data:
+        ```
+        {
+            "networkEvents": [],
+            "aussieOutages": [],
+            "currentNbnOutages": [],
+            "scheduledNbnOutages": [],
+            "resolvedScheduledNbnOutages": [
+                {
+                    "start_date": "2021-08-17T14:00:00Z",
+                    "end_date": "2021-08-17T20:00:00Z",
+                    "duration": "6.0"
+                }
+            ],
+            "resolvedNbnOutages": []
+        }
+        ```
         """
-
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("service_outages", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def service_boltons(self, service_id: int):
-        """ Pulls addons associated with the service.
-
-            Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
+    async def service_boltons(self, service_id: int) -> Dict[str, Any]:
+        """Pulls addons associated with the service.
 
-            Example data:
+        Keys: `['id', 'name', 'description', 'costCents', 'additionalNote', 'active']`
 
-            ```
-            [{
-                "id": 4,
-                "name": "Small Change Big Change Donation",
-                "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
-                "costCents": 100,
-                "additionalNote": null,
-                "active": false
-            }]
-            ```
-            """
+        Example data:
 
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        ```
+        [{
+            "id": 4,
+            "name": "Small Change Big Change Donation",
+            "description": "Charitable donation to the Small Change Big Change program, part of the Telco Together Foundation, which helps build resilient young Australians",
+            "costCents": 100,
+            "additionalNote": null,
+            "active": false
+        }]
+        ```
+        """
+        url = self.get_url("service_boltons", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
         if self.debug:
             print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def service_datablocks(self, service_id: int):
-        """ Pulls datablocks associated with the service.
+    async def service_datablocks(self, service_id: int) -> Dict[str, Any]:
+        """Pulls datablocks associated with the service.
 
-            Keys: `['current', 'available']`
+        Keys: `['current', 'available']`
 
-            Example data:
+        Example data:
 
-            ```
-            {
-                "current": [],
-                "available": []
-            }
-            ```
+        ```
+        {
+            "current": [],
+            "available": []
+        }
+        ```
         """
-
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        url = self.get_url("service_datablocks", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
-        if self.debug:
-            print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def telephony_usage(self, service_id: int):
-        """ Pulls the telephony usage associated with the service.
+    async def telephony_usage(self, service_id: int) -> Dict[str, Any]:
+        """Pulls the telephony usage associated with the service.
 
-            Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
+        Keys: `['national', 'mobile', 'international', 'sms', 'internet', 'voicemail', 'other', 'daysTotal', 'daysRemaining', 'historical']`
 
-            Example data:
+        Example data:
 
-            ```
-            {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},"international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},"internet":{"kbytes":0,"cost":0},"voicemail":{"calls":0,"cost":0},"other":{"calls":0,"cost":0},"daysTotal":31,"daysRemaining":2,"historical":[]}
-            ```
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'service_id' : service_id})
+        ```
+        {"national":{"calls":0,"cost":0},"mobile":{"calls":0,"cost":0},
+        "international":{"calls":0,"cost":0},"sms":{"calls":0,"cost":0},
+        "internet":{"kbytes":0,"cost":0},"voicemail":{"calls":0,"cost":0},
+        "other":{"calls":0,"cost":0},"daysTotal":31,"daysRemaining":2,"historical":[]}
+        ```
+        """
+        url = self.get_url("telephony_usage", {"service_id": service_id})
         responsedata = await self.request_get_json(url=url)
-        if self.debug:
-            print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def support_tickets(self):
-        """ Pulls the support tickets associated with the account, returns a list of dicts.
+    async def support_tickets(self) -> Dict[str, Any]:
+        """Pulls the support tickets associated with the account, returns a list of dicts.
 
-            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
+        Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
 
-            """
-
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
+        """
+        url = self.get_url("support_tickets")
         responsedata = await self.request_get_json(url=url)
-        if self.debug:
-            print(responsedata, file=sys.stderr)
         return responsedata
 
-    async def get_appointment(self, ticketid: int):
-        """ Pulls the support tickets associated with the account, returns a list of dicts.
+    async def get_appointment(self, ticketid: int) -> Dict[str, Any]:
+        """Pulls the support tickets associated with the account, returns a list of dicts.
 
-            Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function, {'ticketid' : ticketid})
+        Dict keys: `['ref', 'create', 'updated', 'service_id', 'type', 'subject', 'status', 'closed', 'awaiting_customer_reply', 'expected_response_minutes']`
+        """
+        url = self.get_url("get_appointment", {"ticketid": ticketid})
         return await self.request_get_json(url=url)
 
-    async def account_contacts(self):
-        """ Pulls the contacts with the account, returns a list of dicts
+    async def account_contacts(self) -> List[AccountContact]:
+        """Pulls the contacts with the account, returns a list of dicts
 
-            Dict keys: `['id', 'first_name', 'last_name', 'email', 'dog', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
-            """
-        frame = inspect.currentframe()
-        url = get_url(inspect.getframeinfo(frame).function)
-        responsedata = await self.request_get_json(url=url)
-        if self.debug:
-            print(responsedata, file=sys.stderr)
-        return responsedata
+        Dict keys: `['id', 'first_name', 'last_name', 'email', 'dob', 'home_phone', 'work_phone', 'mobile_phone', 'work_mobile', 'primary_contact']`
+        """
+        url = self.get_url("account_contacts")
+        response = await self.request_get_json(url=url)
+        return [AccountContact.model_validate(contact) for contact in response]
+
+    async def get_orders(self) -> Dict[str, Any]:
+        """pulls the outstanding orders for an account"""
+        url = self.get_url("get_orders")
+        responsedata = await self.request_get_json(url=url)
+        result = OrderDetailResponseModel(**responsedata)
+        return result.dict()
+
+    async def get_order(self, order_id: int) -> Dict[str, Any]:
+        """gets a specific order"""
+        url = self.get_url("get_order", {"order_id": order_id})
+        responsedata = await self.request_get_json(url=url)
+        result = OrderDetailResponseModel(**responsedata)
+        return result.dict()
+
+    async def get_voip_devices(self, service_id: int) -> List[VOIPDevice]:
+        """gets the devices associatd with a VOIP service"""
+        url = self.get_url("voip_devices", {"service_id": service_id})
+        service_list: List[VOIPDevice] = []
+        data = await self.request_get_json(url=url)
+        for service in data:
+            service_list.append(VOIPDevice.model_validate(service))
+        return service_list
+
+    async def get_voip_service(self, service_id: int) -> VOIPDetails:
+        """gets the details of a VOIP service"""
+        url = self.get_url("voip_service", {"service_id": service_id})
+        data = await self.request_get_json(url=url)
+        return VOIPDetails.model_validate(data)
+
+    async def get_fetch_service(self, service_id: int) -> FetchService:
+        """gets the details of a Fetch service"""
+        url = self.get_url("fetch_service", {"service_id": service_id})
+        data = await self.request_get_json(url=url)
+        return FetchService.model_validate(data)
+
+    async def mfa_send(self, method: MFAMethod) -> None:
+        """sends an MFA code to the user"""
+        url = self.get_url("mfa_send")
+        print(method.dict())
+        await self.request_post_json(url=url, data=method.dict())
+
+    async def mfa_verify(self, token: str) -> None:
+        """got the token from send_mfa? send it back to validate it"""
+        url = self.get_url("mfa_verify")
+        await self.request_post_json(url=url, data={"token": token})
```


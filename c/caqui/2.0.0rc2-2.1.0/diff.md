# Comparing `tmp/caqui-2.0.0rc2.tar.gz` & `tmp/caqui-2.1.0.tar.gz`

## Comparing `caqui-2.0.0rc2.tar` & `caqui-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,51 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-appium.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-win-app-driver.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample-winium.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/sample.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/test-requirements.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tox.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/__init__.py
--rw-r--r--   0        0        0    27242 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/asynchronous.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/by.py
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/caqui.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/exceptions.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/helper.py
--rw-r--r--   0        0        0    26490 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/constants.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/fake_responses.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/test_sniffer.py
--rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/apk/app-debug.apk
--rw-r--r--   0        0        0    33962 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/html/iframe.html
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/html/playground.html
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/__initi__.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_by.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_helper.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_objects.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/utils/coverage.sh
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/LICENSE
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 caqui-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-2.1.0/sample-appium.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-2.1.0/sample-win-app-driver.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-2.1.0/sample-winium.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 caqui-2.1.0/sample.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-2.1.0/test-requirements.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-2.1.0/tox.ini
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-2.1.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-2.1.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-2.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-2.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/__init__.py
+-rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/asynchronous.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/by.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/exceptions.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/helper.py
+-rw-r--r--   0        0        0    26203 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/synchronous.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/action_chains.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/alert.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/driver.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/element.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/switch_to.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 caqui-2.1.0/caqui/easy/window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/constants.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/fake_responses.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/test_sniffer.py
+-rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/apk/app-debug.apk
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/feature/test_objects.py
+-rw-r--r--   0        0        0    33982 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/html/iframe.html
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/html/playground.html
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     7721 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/integration/test_object_scenarios.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/unit/test_by.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 caqui-2.1.0/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-2.1.0/utils/coverage.sh
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-2.1.0/LICENSE
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 caqui-2.1.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 caqui-2.1.0/PKG-INFO
```

### Comparing `caqui-2.0.0rc2/CODE_OF_CONDUCT.md` & `caqui-2.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/sample-appium.py` & `caqui-2.1.0/sample-appium.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/sample-win-app-driver.py` & `caqui-2.1.0/sample-win-app-driver.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/sample-winium.py` & `caqui-2.1.0/sample-winium.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/sample.py` & `caqui-2.1.0/sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # It opens the WebDriver, navigate to a page and get all links
 import asyncio
 import time
 from caqui import synchronous, asynchronous
 from os import getcwd
 from tests.constants import PAGE_URL
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 BASE_DIR = getcwd()
 
 MAX_CONCURRENCY = 5  # number of webdriver instances running
 all_anchors = []
 semaphore = asyncio.Semaphore(MAX_CONCURRENCY)
 
 
 async def get_all_links():
     async with semaphore:
         driver_url = "http://127.0.0.1:9999"
-        capabilities = {
-            "desiredCapabilities": {
-                "browserName": "chrome",
-                "marionette": True,
-                "acceptInsecureCerts": True,
-                "pageLoadStrategy": "normal",
-                "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-            }
-        }
-
+        capabilities = (
+            CapabilitiesBuilder()
+            .browser_name("webdriver")
+            .accept_insecure_certs(True)
+            .page_load_strategy("normal")
+            .additional_capability(
+                {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+            )
+        ).build()
         session = await asynchronous.get_session(driver_url, capabilities)
         await asynchronous.go_to_page(
             driver_url,
             session,
             PAGE_URL,
         )
```

### Comparing `caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-2.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/.github/workflows/python-app.yml` & `caqui-2.1.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/.github/workflows/python-publish.yml` & `caqui-2.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/caqui/asynchronous.py` & `caqui-2.1.0/caqui/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import aiohttp
-import json
-from caqui.constants import HEADERS
-from caqui.exceptions import WebDriverError
-from caqui import helper
+import aiohttp as __aiohttp
+import json as __json
+from caqui.constants import HEADERS as __HEADERS
+from caqui.exceptions import WebDriverError as __WebDriverError
+from caqui import helper as __helper
 
 
 async def __handle_response(resp):
     result = None
     if resp.status in range(200, 399):
         result = await resp.json()
     else:
-        raise WebDriverError(f"Status code: {resp.status}, Body: {resp.text}")
+        raise __WebDriverError(f"Status code: {resp.status}, Body: {resp.text}")
 
     if int(result.get("status", 0)) > 0:
-        raise WebDriverError(f"Status code: {resp.status}, Body: {resp.text}")
+        raise __WebDriverError(f"Status code: {resp.status}, Body: {resp.text}")
 
     return result
 
 
 async def __delete(url):
     try:
-        async with aiohttp.ClientSession() as session:
-            async with session.delete(url, headers=HEADERS) as resp:
+        async with __aiohttp.ClientSession() as session:
+            async with session.delete(url, headers=__HEADERS) as resp:
                 return await __handle_response(resp)
     except Exception as error:
-        raise WebDriverError("'DELETE' request failed.") from error
+        raise __WebDriverError("'DELETE' request failed.") from error
 
 
 async def __post(url, payload):
     try:
-        async with aiohttp.ClientSession() as session:
+        async with __aiohttp.ClientSession() as session:
             async with session.post(
-                url, data=json.dumps(payload), headers=HEADERS
+                url, data=__json.dumps(payload), headers=__HEADERS
             ) as resp:
                 return await __handle_response(resp)
     except Exception as error:
-        raise WebDriverError("'POST' request failed.") from error
+        raise __WebDriverError("'POST' request failed.") from error
 
 
 async def __get(url):
     try:
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=HEADERS) as resp:
+        async with __aiohttp.ClientSession() as session:
+            async with session.get(url, headers=__HEADERS) as resp:
                 return await __handle_response(resp)
     except Exception as error:
-        raise WebDriverError("'GET' request failed.") from error
+        raise __WebDriverError("'GET' request failed.") from error
 
 
 async def __handle_alert(driver_url, session, command):
     url = f"{driver_url}/session/{session}/alert/{command}"
     payload = {
         "value": command,
     }
@@ -60,263 +60,263 @@
     url = f"{driver_url}/session/{session}/window/{command}"
     payload = {}
     await __post(url, payload)
     return True
 
 
 async def add_cookie(driver_url, session, cookie):
-    """Refresh page"""
+    """Add cookie"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         payload = {"cookie": cookie}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to add cookie.") from error
+        raise __WebDriverError("Failed to add cookie.") from error
 
 
 async def delete_cookie(driver_url, session, name):
     """Delete cookie by name"""
     try:
         url = f"{driver_url}/session/{session}/cookie/{name}"
         await __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to delete cookie '{name}'.") from error
+        raise __WebDriverError(f"Failed to delete cookie '{name}'.") from error
 
 
 async def refresh_page(driver_url, session):
     """Refresh page"""
     try:
         url = f"{driver_url}/session/{session}/refresh"
         payload = {}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to refresh page.") from error
+        raise __WebDriverError("Failed to refresh page.") from error
 
 
 async def go_forward(driver_url, session):
     """Go to page forward"""
     try:
         url = f"{driver_url}/session/{session}/forward"
         payload = {}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to go to page forward.") from error
+        raise __WebDriverError("Failed to go to page forward.") from error
 
 
 async def set_window_rectangle(driver_url, session, width, height, x, y):
     """Set window rectangle"""
     try:
         url = f"{driver_url}/session/{session}/window/rect"
         payload = {"width": width, "height": height, "x": x, "y": y}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to set window rectangle.") from error
+        raise __WebDriverError("Failed to set window rectangle.") from error
 
 
 async def fullscreen_window(driver_url, session):
     """Fullscreen window"""
     try:
         return await __handle_window(driver_url, session, command="fullscreen")
     except Exception as error:
-        raise WebDriverError(f"Failed to fullscreen window.") from error
+        raise __WebDriverError("Failed to fullscreen window.") from error
 
 
 async def minimize_window(driver_url, session):
     """Minimize window"""
     try:
         return await __handle_window(driver_url, session, command="minimize")
     except Exception as error:
-        raise WebDriverError(f"Failed to minimize window.") from error
+        raise __WebDriverError("Failed to minimize window.") from error
 
 
 async def maximize_window(driver_url, session):
     """Maximize window"""
     try:
         return await __handle_window(driver_url, session, command="maximize")
     except Exception as error:
-        raise WebDriverError(f"Failed to maximize window.") from error
+        raise __WebDriverError("Failed to maximize window.") from error
 
 
 async def switch_to_window(driver_url, session, handle):
     """Switch to window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         payload = {"name": handle}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to window.") from error
+        raise __WebDriverError("Failed to switch to window.") from error
 
 
 async def new_window(driver_url, session, window_type="tab"):
     """Open a new window
     :param window_type (str): tab or window
 
     return (str): window handle
     """
     try:
         url = f"{driver_url}/session/{session}/window/new"
         payload = {"type": window_type}
         result = await __post(url, payload)
         return result.get("value", {}).get("handle")
     except Exception as error:
-        raise WebDriverError(f"Failed to open window.") from error
+        raise __WebDriverError("Failed to open window.") from error
 
 
 async def switch_to_parent_frame(driver_url, session, element_frame):
     """Switch to parent frame of 'element_frame'"""
     try:
         url = f"{driver_url}/session/{session}/frame/parent"
         payload = {"id": {"ELEMENT": element_frame}}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to parent frame.") from error
+        raise __WebDriverError("Failed to switch to parent frame.") from error
 
 
 async def switch_to_frame(driver_url, session, element_frame):
     """Switch to frame 'element_frame'"""
     try:
         url = f"{driver_url}/session/{session}/frame"
         payload = {"id": {"ELEMENT": element_frame}}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to frame.") from error
+        raise __WebDriverError("Failed to switch to frame.") from error
 
 
 async def delete_all_cookies(driver_url, session):
     """Delete all cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         await __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to delete cookies.") from error
+        raise __WebDriverError("Failed to delete cookies.") from error
 
 
 async def send_alert_text(driver_url, session, text):
     """Fill the alert text area and send the text"""
     try:
         url = f"{driver_url}/session/{session}/alert/text"
         payload = {
             "text": text,
         }
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to sent text to alert.") from error
+        raise __WebDriverError("Failed to sent text to alert.") from error
 
 
 async def accept_alert(driver_url, session):
     """Accept alert"""
     try:
         return await __handle_alert(driver_url, session, "accept")
     except Exception as error:
-        raise WebDriverError(f"Failed to accept alert.") from error
+        raise __WebDriverError("Failed to accept alert.") from error
 
 
 async def dismiss_alert(driver_url, session):
     """Dismiss alert"""
     try:
         return await __handle_alert(driver_url, session, "dismiss")
     except Exception as error:
-        raise WebDriverError(f"Failed to dismiss alert.") from error
+        raise __WebDriverError("Failed to dismiss alert.") from error
 
 
 async def take_screenshot_element(
     driver_url, session, element, path="/tmp", file_name="caqui"
 ):
     """Take screenshot of element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/screenshot"
         response = await __get(url)
         picture = response.get("value")
-        helper.save_picture(session, path, file_name, picture)
+        __helper.save_picture(session, path, file_name, picture)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to take screenshot.") from error
+        raise __WebDriverError("Failed to take screenshot from element.") from error
 
 
 async def take_screenshot(driver_url, session, path="/tmp", file_name="caqui"):
     """Take screenshot"""
     try:
         url = f"{driver_url}/session/{session}/screenshot"
         response = await __get(url)
         picture = response.get("value")
-        helper.save_picture(session, path, file_name, picture)
+        __helper.save_picture(session, path, file_name, picture)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to take screenshot.") from error
+        raise __WebDriverError("Failed to take screenshot.") from error
 
 
 async def get_named_cookie(driver_url, session, name):
     """Get cookie by name"""
     try:
         url = f"{driver_url}/session/{session}/cookie/{name}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get cookie '{name}'.") from error
+        raise __WebDriverError(f"Failed to get cookie '{name}'.") from error
 
 
 async def get_computed_label(driver_url, session, element):
     """Get the element tag computed label. Get the accessibility name"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/computedlabel"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get element computed label.") from error
+        raise __WebDriverError("Failed to get element computed label.") from error
 
 
 async def get_computed_role(driver_url, session, element):
     """Get the element tag computed role (the element role)"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/computedrole"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get element computed role.") from error
+        raise __WebDriverError("Failed to get element computed role.") from error
 
 
 async def get_tag_name(driver_url, session, element):
     """Get the element tag name"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/name"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get element name.") from error
+        raise __WebDriverError("Failed to get element name.") from error
 
 
 async def get_shadow_root(driver_url, session, element):
     """Get the shadow root element"""
     try:
         root_element = "shadow-6066-11e4-a52e-4f735466cecf"
         url = f"{driver_url}/session/{session}/element/{element}/shadow"
         response = await __get(url)
         return response.get("value", {}).get(root_element)
     except Exception as error:
-        raise WebDriverError("Failed to get element shadow.") from error
+        raise __WebDriverError("Failed to get element shadow.") from error
 
 
 async def get_rect(driver_url, session, element):
     """Get the element rectangle"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/rect"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get element rect.") from error
+        raise __WebDriverError("Failed to get element rect.") from error
 
 
 async def actions(driver_url, session, payload):
     url = f"{driver_url}/session/{session}/actions"
     await __post(url, payload)
     return True
 
@@ -345,15 +345,15 @@
                     "id": "key",
                     "actions": [{"type": "pause", "duration": 0}],
                 },
             ]
         }
         return await actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to move to element.") from error
+        raise __WebDriverError("Failed to move to element.") from error
 
 
 async def actions_scroll_to_element(driver_url, session, element):
     """Scroll to an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
@@ -372,15 +372,15 @@
                         }
                     ],
                 }
             ]
         }
         return await actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to scroll to element.") from error
+        raise __WebDriverError("Failed to scroll to element.") from error
 
 
 async def submit(driver_url, session, element):
     """Submit a form. It is similar to 'submit' funtion in Seleniu
     It is not part of W3C WebDriver. Just added for convenience
     """
     try:
@@ -389,15 +389,15 @@
             session,
             element,
             locator_type="xpath",
             locator_value="*[@type='submit']",
         )
         return await click(driver_url, session, submit_element)
     except Exception as error:
-        raise WebDriverError(f"Failed to submit form.") from error
+        raise __WebDriverError("Failed to submit form.") from error
 
 
 async def actions_click(driver_url, session, element):
     """Click an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
@@ -426,220 +426,220 @@
                         {"type": "pause", "duration": 0},
                     ],
                 },
             ]
         }
         return await actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to click the element.") from error
+        raise __WebDriverError("Failed to click the element.") from error
 
 
 async def set_timeouts(driver_url, session, timeouts):
     """Set timeouts"""
     try:
         url = f"{driver_url}/session/{session}/timeouts"
         payload = {
             "implicit": timeouts,
         }
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to set timeouts.") from error
+        raise __WebDriverError("Failed to set timeouts.") from error
 
 
 async def find_children_elements(
     driver_url, session, parent_element, locator_type, locator_value
 ):
     """Find the children elements by 'locator_type'
 
     If the 'parent_element' is a shadow element, set the 'locator_type' as 'id' or
     'css selector'
     """
     try:
         url = f"{driver_url}/session/{session}/element/{parent_element}/elements"
         payload = {"using": locator_type, "value": locator_value, "id": parent_element}
         response = await __post(url, payload)
-        return helper.get_elements(response)
+        return __helper.get_elements(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find the children elements from '{parent_element}'."
         ) from error
 
 
 async def find_child_element(
     driver_url, session, parent_element, locator_type, locator_value
 ):
     """Find the child element by 'locator_type'"""
     try:
         url = f"{driver_url}/session/{session}/element/{parent_element}/element"
         payload = {"using": locator_type, "value": locator_value, "id": parent_element}
         response = await __post(url, payload)
-        return helper.get_element(response)
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find the child element from '{parent_element}'."
         ) from error
 
 
 async def get_page_source(driver_url, session):
     """Get the page source (all content)"""
     try:
         url = f"{driver_url}/session/{session}/source"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get the page source.") from error
+        raise __WebDriverError("Failed to get the page source.") from error
 
 
 async def execute_script(driver_url, session, script, args=[]):
     """Executes a script, like 'alert('something')' to open an alert window"""
     try:
         url = f"{driver_url}/session/{session}/execute/sync"
         payload = {"script": script, "args": args}
         response = await __post(url, payload)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to open session.") from error
+        raise __WebDriverError("Failed to execute script.") from error
 
 
 async def get_alert_text(driver_url, session):
     """Get the text from an alert"""
     try:
         url = f"{driver_url}/session/{session}/alert/text"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get the alert text.") from error
+        raise __WebDriverError("Failed to get the alert text.") from error
 
 
 async def get_active_element(driver_url, session):
     """Get the active element"""
     try:
         url = f"{driver_url}/session/{session}/element/active"
         response = await __get(url)
-        return helper.get_element(response)
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError("Failed to check if element is selected.") from error
+        raise __WebDriverError("Failed to check if element is selected.") from error
 
 
 async def clear_element(driver_url, session, element):
     """Clear the element text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/clear"
         payload = {"id": element}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to clear the element text.") from error
+        raise __WebDriverError("Failed to clear the element text.") from error
 
 
 async def is_element_enabled(driver_url, session, element):
     """Check if element is enabled"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/enabled"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to check if element is enabled.") from error
+        raise __WebDriverError("Failed to check if element is enabled.") from error
 
 
 async def get_css_value(driver_url, session, element, property_name):
     """Check if element is selected"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/css/{property_name}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to check if element is selected.") from error
+        raise __WebDriverError("Failed to check if element is selected.") from error
 
 
 async def is_element_selected(driver_url, session, element):
     """Check if element is selected"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/selected"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to check if element is selected.") from error
+        raise __WebDriverError("Failed to check if element is selected.") from error
 
 
 async def get_window_rectangle(driver_url, session):
     """Get window rectangle"""
     try:
         url = f"{driver_url}/session/{session}/window/rect"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get window rectangle.") from error
+        raise __WebDriverError("Failed to get window rectangle.") from error
 
 
 async def get_window_handles(driver_url, session):
     """Get window handles"""
     try:
         url = f"{driver_url}/session/{session}/window/handles"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get window handles.") from error
+        raise __WebDriverError("Failed to get window handles.") from error
 
 
 async def close_window(driver_url, session):
     """Close active window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         response = await __delete(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to close active window.") from error
+        raise __WebDriverError("Failed to close active window.") from error
 
 
 async def get_window(driver_url, session):
     """Get window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get window.") from error
+        raise __WebDriverError("Failed to get window.") from error
 
 
 async def go_back(driver_url, session):
     """
     This command causes the browser to traverse one step backward in the joint session history of the
     current browse. This is equivalent to pressing the back button in the browser.
     """
     try:
         url = f"{driver_url}/session/{session}/back"
         await __post(url, {})
         return True
     except Exception as error:
-        raise WebDriverError("Failed to go back to page.") from error
+        raise __WebDriverError("Failed to go back to page.") from error
 
 
 async def get_url(driver_url, session):
     """Return the URL from web page:"""
     try:
         url = f"{driver_url}/session/{session}/url"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get page url.") from error
+        raise __WebDriverError("Failed to get page url.") from error
 
 
 async def get_timeouts(driver_url, session):
     """
     Return the configured timeouts:
         {"implicit": 0, "pageLoad": 300000, "script": 30000}
     """
     try:
         url = f"{driver_url}/session/{session}/timeouts"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get timeouts.") from error
+        raise __WebDriverError("Failed to get timeouts.") from error
 
 
 async def get_status(driver_url):
     """
     Return the status and details of the WebDriver:
         "build": {
                 "version": "113.0.5672.63 (0e1a4471d5ae5bf128b1bd8f4d627c8cbd55f70c-refs/branch-heads/5672@{#912})"
@@ -650,88 +650,88 @@
         }
     """
     try:
         url = f"{driver_url}/status"
         response = await __get(url)
         return response
     except Exception as error:
-        raise WebDriverError("Failed to get status.") from error
+        raise __WebDriverError("Failed to get status.") from error
 
 
 async def get_title(driver_url, session):
     """Get the page title"""
     try:
         url = f"{driver_url}/session/{session}/title"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get page title.") from error
+        raise __WebDriverError("Failed to get page title.") from error
 
 
 async def find_elements(driver_url, session, locator_type, locator_value):
     """Search the DOM elements by 'locator', for example, 'xpath'"""
     try:
         payload = {"using": locator_type, "value": locator_value}
         url = f"{driver_url}/session/{session}/elements"
         response = await __post(url, payload)
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
 async def get_property(driver_url, session, element, property):
     """Get the given HTML property of an element, for example, 'href'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get value from element.") from error
+        raise __WebDriverError("Failed to get value from element.") from error
 
 
 async def get_attribute(driver_url, session, element, attribute):
     """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get value from element.") from error
+        raise __WebDriverError("Failed to get value from element.") from error
 
 
 async def get_text(driver_url, session, element):
     """Get the text of an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/text"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get text from element.") from error
+        raise __WebDriverError("Failed to get text from element.") from error
 
 
 async def get_cookies(driver_url, session):
     """Get the page cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         response = await __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get page cookies.") from error
+        raise __WebDriverError("Failed to get page cookies.") from error
 
 
 async def close_session(driver_url, session):
     """Close an opened session and close the browser"""
     try:
         url = f"{driver_url}/session/{session}"
         await __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to close session.") from error
+        raise __WebDriverError("Failed to close session.") from error
 
 
 async def get(driver_url, session, page_url):
     """Does the same of 'go_to_page'. Added to be compatible with selenium method name'"""
     return go_to_page(driver_url, session, page_url)
 
 
@@ -739,60 +739,60 @@
     """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
         payload = {"url": page_url}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to navigate to page '{page_url}'.") from error
+        raise __WebDriverError(f"Failed to navigate to page '{page_url}'.") from error
 
 
 async def send_keys(driver_url, session, element, text):
     """Fill an editable element, for example a textarea, with a given text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/value"
         payload = {"text": text, "value": [*text], "id": element}
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to send key '{text}'.") from error
+        raise __WebDriverError(f"Failed to send key '{text}'.") from error
 
 
 async def click(driver_url, session, element):
     """Click on an element"""
     try:
         payload = {"id": element}
         url = f"{driver_url}/session/{session}/element/{element}/click"
         await __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to click on element.") from error
+        raise __WebDriverError("Failed to click on element.") from error
 
 
 async def find_element(driver_url, session, locator_type, locator_value):
     """Find an element by a 'locator', for example 'xpath'"""
 
     try:
         payload = {"using": locator_type, "value": locator_value}
         url = f"{driver_url}/session/{session}/element"
         response = await __post(url, payload)
 
         # Firefox does not support id locator, so it prints the error message to the user
         # It helps on debug
         if response.get("value").get("error"):
-            raise WebDriverError(f"Failed to find element. {response}")
-        return helper.get_element(response)
+            raise __WebDriverError(f"Failed to find element. {response}")
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
 async def get_session(driver_url, capabilities):
     """Opens a browser and a session. This session is used for all functions to perform events in the page"""
     try:
         payload = capabilities
         url = f"{driver_url}/session"
         response = await __post(url, payload)
         return response.get("sessionId")
     except Exception as error:
-        raise WebDriverError("Failed to open session.") from error
+        raise __WebDriverError("Failed to open session.") from error
```

### Comparing `caqui-2.0.0rc2/caqui/synchronous.py` & `caqui-2.1.0/caqui/synchronous.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,59 @@
-import requests
-import json
-from caqui.exceptions import WebDriverError
-from caqui import helper
-
-HEADERS = {
-    "Accept-Encoding": "identity",
-    "Accept": "application/json",
-    "Content-Type": "application/json;charset=UTF-8",
-    "Connection": "keep-alive",
-}
+import requests as __requests
+import json as __json
+from caqui.exceptions import WebDriverError as __WebDriverError
+from caqui import helper as __helper
+from caqui.constants import HEADERS as __HEADERS
 
 
 def __handle_response(response):
     result = None
     if response.status_code in range(200, 399):
         result = response.json()
     else:
-        raise WebDriverError(f"Status: {response.status_code}, {response.text}")
+        raise __WebDriverError(f"Status: {response.status_code}, {response.text}")
 
     if int(result.get("status", 0)) > 0:
-        raise WebDriverError(f"Status: {response.status_code}, {response.text}")
+        raise __WebDriverError(f"Status: {response.status_code}, {response.text}")
     return result
 
 
 def __get(url):
     try:
-        response = requests.request("GET", url, headers=HEADERS, data={})
+        response = __requests.request("GET", url, headers=__HEADERS, data={})
         return __handle_response(response)
     except Exception as error:
-        raise WebDriverError("'GET' request failed.") from error
+        raise __WebDriverError("'GET' request failed.") from error
 
 
 def __post(url, payload):
-    response = requests.request("POST", url, headers=HEADERS, data=json.dumps(payload))
+    response = __requests.request(
+        "POST", url, headers=__HEADERS, data=__json.dumps(payload)
+    )
     try:
         return __handle_response(response)
     except Exception as error:
-        raise WebDriverError("'POST' request failed.") from error
+        raise __WebDriverError("'POST' request failed.") from error
 
 
 def __delete(url):
     try:
-        response = requests.request("DELETE", url, headers={}, data={})
+        response = __requests.request("DELETE", url, headers={}, data={})
         return __handle_response(response)
     except Exception as error:
-        raise WebDriverError("'DELETE' request failed.") from error
+        raise __WebDriverError("'DELETE' request failed.") from error
 
 
 def __handle_alerts(driver_url, session, command):
     url = f"{driver_url}/session/{session}/alert/{command}"
     payload = {"value": command}
     __post(url, payload)
     return True
 
 
-# def add_cookie(driver_url, session, name, value):
-#     """Add cookie by name"""
-#     try:
-#         url = f"{driver_url}/session/{session}/cookie"
-#         payload = {"cookie": {"name": name, "value": value}}
-#         __post(url, payload)
-#         return True
-#     except Exception as error:
-#         raise WebDriverError(f"Failed to add cookie '{name}'.") from error
-
-
 def __handle_window(driver_url, session, command):
     url = f"{driver_url}/session/{session}/window/{command}"
     payload = {}
     __post(url, payload)
     return True
 
 
@@ -76,245 +61,245 @@
     """Add cookie"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         payload = {"cookie": cookie}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to add cookie.") from error
+        raise __WebDriverError("Failed to add cookie.") from error
 
 
 def delete_cookie(driver_url, session, name):
     """Delete cookie by name"""
     try:
         url = f"{driver_url}/session/{session}/cookie/{name}"
         __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to delete cookie '{name}'.") from error
+        raise __WebDriverError("Failed to delete cookie '{name}'.") from error
 
 
 def refresh_page(driver_url, session):
     """Refresh page"""
     try:
         url = f"{driver_url}/session/{session}/refresh"
         payload = {}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to refresh page.") from error
+        raise __WebDriverError("Failed to refresh page.") from error
 
 
 def go_forward(driver_url, session):
     """Go to page forward"""
     try:
         url = f"{driver_url}/session/{session}/forward"
         payload = {}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to go page forward.") from error
+        raise __WebDriverError("Failed to go page forward.") from error
 
 
 def set_window_rectangle(driver_url, session, width, height, x, y):
     """Set window rectangle"""
     try:
         url = f"{driver_url}/session/{session}/window/rect"
         payload = {"width": width, "height": height, "x": x, "y": y}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to set window rectangle.") from error
+        raise __WebDriverError("Failed to set window rectangle.") from error
 
 
 def fullscreen_window(driver_url, session):
     """Fullscreen window"""
     try:
         return __handle_window(driver_url, session, command="fullscreen")
     except Exception as error:
-        raise WebDriverError(f"Failed to fullscreen window.") from error
+        raise __WebDriverError("Failed to fullscreen window.") from error
 
 
 def minimize_window(driver_url, session):
     """Minimize window"""
     try:
         return __handle_window(driver_url, session, command="minimize")
     except Exception as error:
-        raise WebDriverError(f"Failed to minimize window.") from error
+        raise __WebDriverError("Failed to minimize window.") from error
 
 
 def maximize_window(driver_url, session):
     """Maximize window"""
     try:
         return __handle_window(driver_url, session, command="maximize")
     except Exception as error:
-        raise WebDriverError(f"Failed to maximize window.") from error
+        raise __WebDriverError("Failed to maximize window.") from error
 
 
 def switch_to_window(driver_url, session, handle):
     """Switch to window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         payload = {"name": handle}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to window.") from error
+        raise __WebDriverError("Failed to switch to window.") from error
 
 
 def new_window(driver_url, session, window_type="tab"):
     """Open a new window
     :param window_type (str): tab or window
 
     return (str): window handle
     """
     try:
         url = f"{driver_url}/session/{session}/window/new"
         payload = {"type": window_type}
         return __post(url, payload).get("value", {}).get("handle")
     except Exception as error:
-        raise WebDriverError(f"Failed to open a new window.") from error
+        raise __WebDriverError("Failed to open a new window.") from error
 
 
 def switch_to_parent_frame(driver_url, session, element_frame):
     """Switch to parent frame of 'element_frame'"""
     try:
         url = f"{driver_url}/session/{session}/frame/parent"
         payload = {"id": {"ELEMENT": element_frame}}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to parent frame.") from error
+        raise __WebDriverError("Failed to switch to parent frame.") from error
 
 
 def switch_to_frame(driver_url, session, element_frame):
     """Switch to frame 'element_frame'"""
     try:
         url = f"{driver_url}/session/{session}/frame"
         payload = {"id": {"ELEMENT": element_frame}}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to switch to frame.") from error
+        raise __WebDriverError("Failed to switch to frame.") from error
 
 
 def delete_all_cookies(driver_url, session):
     """Delete all cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to delete cookies.") from error
+        raise __WebDriverError("Failed to delete cookies.") from error
 
 
 def send_alert_text(driver_url, session, text):
     """Fill the alert text area and send the text"""
     try:
         url = f"{driver_url}/session/{session}/alert/text"
         payload = {"text": text}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to sent text to alert.") from error
+        raise __WebDriverError("Failed to sent text to alert.") from error
 
 
 def accept_alert(driver_url, session):
     """Accept an alert"""
     try:
         return __handle_alerts(driver_url, session, "accept")
     except Exception as error:
-        raise WebDriverError(f"Failed to accept the alert.") from error
+        raise __WebDriverError("Failed to accept the alert.") from error
 
 
 def dismiss_alert(driver_url, session):
     """Dismiss an alert"""
     try:
         return __handle_alerts(driver_url, session, "dismiss")
     except Exception as error:
-        raise WebDriverError(f"Failed to dismiss the alert.") from error
+        raise __WebDriverError("Failed to dismiss the alert.") from error
 
 
 def take_screenshot_element(
     driver_url, session, element, path="/tmp", file_name="caqui"
 ):
     """Take screenshot of element."""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/screenshot"
         response = __get(url).get("value")
-        helper.save_picture(session, path, file_name, response)
+        __helper.save_picture(session, path, file_name, response)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to take screeshot.") from error
+        raise __WebDriverError("Failed to take screeshot.") from error
 
 
 def take_screenshot(driver_url, session, path="/tmp", file_name="caqui"):
     """Take screenshot."""
     try:
         url = f"{driver_url}/session/{session}/screenshot"
         response = __get(url).get("value")
-        helper.save_picture(session, path, file_name, response)
+        __helper.save_picture(session, path, file_name, response)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to take screeshot.") from error
+        raise __WebDriverError("Failed to take screeshot.") from error
 
 
 def get_named_cookie(driver_url, session, name):
     """Get cookie by name."""
     try:
         url = f"{driver_url}/session/{session}/cookie/{name}"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the cookie '{name}'.") from error
+        raise __WebDriverError(f"Failed to get the cookie '{name}'.") from error
 
 
 def get_computed_label(driver_url, session, element):
     """Get the element computed label. Get the accessibility name."""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/computedlabel"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the element computed label.") from error
+        raise __WebDriverError("Failed to get the element computed label.") from error
 
 
 def get_computed_role(driver_url, session, element):
     """Get the element computed role (the element role)"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/computedrole"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the element computed role.") from error
+        raise __WebDriverError("Failed to get the element computed role.") from error
 
 
 def get_tag_name(driver_url, session, element):
     """Get the element tag name"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/name"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the element name.") from error
+        raise __WebDriverError("Failed to get the element name.") from error
 
 
 def get_shadow_root(driver_url, session, element):
     """Get the shadow root element"""
     try:
         root_element = "shadow-6066-11e4-a52e-4f735466cecf"
         url = f"{driver_url}/session/{session}/element/{element}/shadow"
         return __get(url).get("value", {}).get(root_element)
     except Exception as error:
-        raise WebDriverError(f"Failed to get the element shadow.") from error
+        raise __WebDriverError("Failed to get the element shadow.") from error
 
 
 def get_rect(driver_url, session, element):
     """Get the element rectangle"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/rect"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the element rect.") from error
+        raise __WebDriverError("Failed to get the element rect.") from error
 
 
 def actions_move_to_element(driver_url, session, element):
     """Move to an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
@@ -337,15 +322,15 @@
                     "id": "key",
                     "actions": [{"type": "pause", "duration": 0}],
                 },
             ]
         }
         return actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to move to element.") from error
+        raise __WebDriverError("Failed to move to element.") from error
 
 
 def actions_scroll_to_element(driver_url, session, element):
     """Scroll to an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
@@ -364,15 +349,15 @@
                         }
                     ],
                 }
             ]
         }
         return actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to scroll to element.") from error
+        raise __WebDriverError("Failed to scroll to element.") from error
 
 
 def actions(driver_url, session, payload):
     url = f"{driver_url}/session/{session}/actions"
     __post(url, payload)
     return True
 
@@ -387,15 +372,15 @@
             session,
             element,
             locator_type="xpath",
             locator_value="//*[@type='submit']",
         )
         return click(driver_url, session, submit_element)
     except Exception as error:
-        raise WebDriverError(f"Failed to submit form.") from error
+        raise __WebDriverError("Failed to submit form.") from error
 
 
 def actions_click(driver_url, session, element):
     """Click an element simulating a mouse movement"""
     try:
         payload = {
             "actions": [
@@ -424,211 +409,211 @@
                         {"type": "pause", "duration": 0},
                     ],
                 },
             ]
         }
         return actions(driver_url, session, payload)
     except Exception as error:
-        raise WebDriverError(f"Failed to click the element.") from error
+        raise __WebDriverError("Failed to click the element.") from error
 
 
 def set_timeouts(driver_url, session, timeouts):
     """Set timeouts"""
     try:
         url = f"{driver_url}/session/{session}/timeouts"
         payload = {
             "implicit": timeouts,
         }
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to set timeouts.") from error
+        raise __WebDriverError("Failed to set timeouts.") from error
 
 
 def find_children_elements(
     driver_url, session, parent_element, locator_type, locator_value
 ):
     """Find the children elements by 'locator_type'
 
     If the 'parent_element' is a shadow element, set the 'locator_type' as 'id' or
     'css selector'
     """
     try:
         url = f"{driver_url}/session/{session}/element/{parent_element}/elements"
         payload = {"using": locator_type, "value": locator_value, "id": parent_element}
         response = __post(url, payload)
-        return helper.get_elements(response)
+        return __helper.get_elements(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find the children elements from '{parent_element}'."
         ) from error
 
 
 def find_child_element(
     driver_url, session, parent_element, locator_type, locator_value
 ):
     """Find the child element by 'locator_type'"""
     try:
         url = f"{driver_url}/session/{session}/element/{parent_element}/element"
         payload = {"using": locator_type, "value": locator_value, "id": parent_element}
         response = __post(url, payload)
-        return helper.get_element(response)
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find the child element from '{parent_element}'."
         ) from error
 
 
 def get_page_source(driver_url, session):
     """Get the page source (all content)"""
     try:
         url = f"{driver_url}/session/{session}/source"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the page source.") from error
+        raise __WebDriverError("Failed to get the page source.") from error
 
 
 def execute_script(driver_url, session, script, args=[]):
     """Executes a script, like 'alert('something')' to open an alert window"""
     try:
         url = f"{driver_url}/session/{session}/execute/sync"
         payload = {"script": script, "args": args}
         response = __post(url, payload)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to run the script.") from error
+        raise __WebDriverError("Failed to run the script.") from error
 
 
 def get_alert_text(driver_url, session):
     """Get the text from an alert"""
     try:
         url = f"{driver_url}/session/{session}/alert/text"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the alert text.") from error
+        raise __WebDriverError("Failed to get the alert text.") from error
 
 
 def get_active_element(driver_url, session):
     """Get the active element"""
     try:
         url = f"{driver_url}/session/{session}/element/active"
         response = __get(url)
-        return helper.get_element(response)
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError(f"Failed to get the active element.") from error
+        raise __WebDriverError("Failed to get the active element.") from error
 
 
 def clear_element(driver_url, session, element):
     """Clear the element text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/clear"
         payload = {"id": element}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to clear the element text.") from error
+        raise __WebDriverError("Failed to clear the element text.") from error
 
 
 def is_element_enabled(driver_url, session, element):
     """Check if element is enabled"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/enabled"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to check if element is enabled.") from error
+        raise __WebDriverError("Failed to check if element is enabled.") from error
 
 
 def get_css_value(driver_url, session, element, property_name):
     """Get the css property value"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/css/{property_name}"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get the css property value.") from error
+        raise __WebDriverError("Failed to get the css property value.") from error
 
 
 def is_element_selected(driver_url, session, element):
     """Check if element is selected"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/selected"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to check if element is selected.") from error
+        raise __WebDriverError("Failed to check if element is selected.") from error
 
 
 def get_window_rectangle(driver_url, session):
     """Get window rectangle"""
     try:
         url = f"{driver_url}/session/{session}/window/rect"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get window rectangle.") from error
+        raise __WebDriverError("Failed to get window rectangle.") from error
 
 
 def get_window_handles(driver_url, session):
     """Get window handles"""
     try:
         url = f"{driver_url}/session/{session}/window/handles"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get window handles.") from error
+        raise __WebDriverError("Failed to get window handles.") from error
 
 
 def close_window(driver_url, session):
     """Close active window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         return __delete(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to close active window.") from error
+        raise __WebDriverError("Failed to close active window.") from error
 
 
 def get_window(driver_url, session):
     """Get window"""
     try:
         url = f"{driver_url}/session/{session}/window"
         return __get(url).get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get window.") from error
+        raise __WebDriverError("Failed to get window.") from error
 
 
 def go_back(driver_url, session):
     """
     This command causes the browser to traverse one step backward in the joint session history of the
     current browse. This is equivalent to pressing the back button in the browser.
     """
     try:
         url = f"{driver_url}/session/{session}/back"
         __post(url, {})
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to go back to page.") from error
+        raise __WebDriverError("Failed to go back to page.") from error
 
 
 def get_url(driver_url, session):
     """Return the URL from web page:"""
     try:
         url = f"{driver_url}/session/{session}/url"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get page url.") from error
+        raise __WebDriverError("Failed to get page url.") from error
 
 
 def get_timeouts(driver_url, session):
     """
     Return the configured timeouts:
         {"implicit": 0, "pageLoad": 300000, "script": 30000}
     """
     try:
         url = f"{driver_url}/session/{session}/timeouts"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get timeouts.") from error
+        raise __WebDriverError("Failed to get timeouts.") from error
 
 
 def get_status(driver_url):
     """
     Return the status and details of the WebDriver:
         "build": {
                 "version": "113.0.5672.63 (0e1a4471d5ae5bf128b1bd8f4d627c8cbd55f70c-refs/branch-heads/5672@{#912})"
@@ -638,68 +623,70 @@
             "ready": True,
         }
     """
     try:
         url = f"{driver_url}/status"
         return __get(url)
     except Exception as error:
-        raise WebDriverError(f"Failed to get status.") from error
+        raise __WebDriverError("Failed to get status.") from error
 
 
 def get_title(driver_url, session):
     """Get the page title"""
     try:
         url = f"{driver_url}/session/{session}/title"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError(f"Failed to get page title.") from error
+        raise __WebDriverError("Failed to get page title.") from error
 
 
 def find_elements(driver_url, session, locator_type, locator_value):
     """Search the DOM elements by 'locator', for example, 'xpath'"""
     try:
         url = f"{driver_url}/session/{session}/elements"
         payload = {"using": locator_type, "value": locator_value}
         response = __post(url, payload)
         return [x.get("ELEMENT") for x in response.get("value")]
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find elements by '{locator_type}'-'{locator_value}'."
         ) from error
 
 
-def get_property(driver_url, session, element, property):
+def get_property(driver_url, session, element, property_name):
     """Get the given HTML property of an element, for example, 'href'"""
     try:
-        url = f"{driver_url}/session/{session}/element/{element}/property/{property}"
+        url = (
+            f"{driver_url}/session/{session}/element/{element}/property/{property_name}"
+        )
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get value from element.") from error
+        raise __WebDriverError("Failed to get value from element.") from error
 
 
 def get_attribute(driver_url, session, element, attribute):
     """Get the given HTML attribute of an element, for example, 'aria-valuenow'"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/attribute/{attribute}"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get value from element.") from error
+        raise __WebDriverError("Failed to get value from element.") from error
 
 
 def get_cookies(driver_url, session):
     """Get the page cookies"""
     try:
         url = f"{driver_url}/session/{session}/cookie"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get page cookies.") from error
+        raise __WebDriverError("Failed to get page cookies.") from error
 
 
 def get(driver_url, session, page_url):
     """Does the same of 'go_to_page'. Added to be compatible with selenium method name'"""
     return go_to_page(driver_url, session, page_url)
 
 
@@ -707,57 +694,57 @@
     """Navigate to 'page_url'"""
     try:
         url = f"{driver_url}/session/{session}/url"
         payload = {"url": page_url}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to navigate to '{page_url}'") from error
+        raise __WebDriverError(f"Failed to navigate to '{page_url}'") from error
 
 
 def close_session(driver_url, session):
     """Close an opened session and close the browser"""
     try:
         url = f"{driver_url}/session/{session}"
         __delete(url)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to close session.") from error
+        raise __WebDriverError("Failed to close session.") from error
 
 
 def get_text(driver_url, session, element):
     """Get the text of an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/text"
         response = __get(url)
         return response.get("value")
     except Exception as error:
-        raise WebDriverError("Failed to get text from element.") from error
+        raise __WebDriverError("Failed to get text from element.") from error
 
 
 def send_keys(driver_url, session, element, text):
     """Fill an editable element, for example a textarea, with a given text"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/value"
         payload = {"text": text, "value": [*text], "id": element}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError(f"Failed to send key '{text}'.") from error
+        raise __WebDriverError(f"Failed to send key '{text}'.") from error
 
 
 def click(driver_url, session, element):
     """Click on an element"""
     try:
         url = f"{driver_url}/session/{session}/element/{element}/click"
         payload = {"id": element}
         __post(url, payload)
         return True
     except Exception as error:
-        raise WebDriverError("Failed to click on element.") from error
+        raise __WebDriverError("Failed to click on element.") from error
 
 
 def __get_session(response):
     # Firefox response
     value = response.get("value")
     session_id = value.get("sessionId")
     if session_id:
@@ -771,27 +758,27 @@
     """Opens a browser and a session. This session is used for all functions to perform events in the page"""
     try:
         url = f"{driver_url}/session"
         data = capabilities
         response = __post(url, payload=data)
         return __get_session(response)
     except Exception as error:
-        raise WebDriverError("Failed to open session.") from error
+        raise __WebDriverError("Failed to open session.") from error
 
 
 def find_element(driver_url, session, locator_type, locator_value):
     """Find an element by a 'locator', for example 'xpath'"""
     try:
         url = f"{driver_url}/session/{session}/element"
         payload = {"using": locator_type, "value": locator_value}
         response = __post(url, payload)
 
         # Firefox does not support id locator, so it prints the error message to the user
         # It helps on debug
         if response.get("value").get("error"):
-            raise WebDriverError(f"Failed to find element. {response}")
+            raise __WebDriverError(f"Failed to find element. {response}")
 
-        return helper.get_element(response)
+        return __helper.get_element(response)
     except Exception as error:
-        raise WebDriverError(
+        raise __WebDriverError(
             f"Failed to find element by '{locator_type}'-'{locator_value}'."
         ) from error
```

### Comparing `caqui-2.0.0rc2/tests/fake_responses.py` & `caqui-2.1.0/tests/fake_responses.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/tests/test_sniffer.py` & `caqui-2.1.0/tests/test_sniffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     }
 
     driver = webdriver.Remote(
         command_executor="http://localhost:9999",
         desired_capabilities=desired_capabilities,
     )
     driver.get(PAGE_URL)
-    driver
+    # driver.find_element().value_of_css_property()
     yield driver
     driver.quit()
 
 
 @fixture
 def setup_binary():
     homedir = os.path.expanduser("~")
```

### Comparing `caqui-2.0.0rc2/tests/apk/app-debug.apk` & `caqui-2.1.0/tests/apk/app-debug.apk`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/tests/feature/test_sync_and_async.py` & `caqui-2.1.0/tests/feature/test_sync_and_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from pytest import fixture, mark, raises
 from caqui import asynchronous, synchronous
 from tests.constants import PAGE_URL
 from caqui.exceptions import WebDriverError
 from caqui.by import By
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
-    capabilities = {
-        "desiredCapabilities": {
-            By.NAME: "webdriver",
-            "browserName": "chrome",
-            "marionette": False,
-            "acceptInsecureCerts": True,
-            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-        }
-    }
+    capabilities = (
+        CapabilitiesBuilder()
+        .browser_name("webdriver")
+        .accept_insecure_certs(True)
+        .additional_capability(
+            {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+        )
+    ).build()
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
         driver_url,
         session,
         PAGE_URL,
     )
     yield driver_url, session
@@ -36,15 +36,15 @@
         driver_url,
         session,
         "http://www.google.com",
     )
     cookies_before = synchronous.get_cookies(driver_url, session)
 
     cookie = cookies_before[0]
-    cookie[By.NAME] = "other"
+    cookie["name"] = "other"
 
     assert synchronous.add_cookie(driver_url, session, cookie) is True
     cookies_after = synchronous.get_cookies(driver_url, session)
     assert len(cookies_after) > len(cookies_before)
 
     cookies_before = cookies_after
     cookie = cookies_before[0]
```

### Comparing `caqui-2.0.0rc2/tests/html/playground.html` & `caqui-2.1.0/tests/html/playground.html`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/tests/integration/test_async_scenarios.py` & `caqui-2.1.0/tests/integration/test_async_scenarios.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from caqui import synchronous, asynchronous
 from tests.constants import PAGE_URL
 from pytest import fixture, mark
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
-    capabilities = {
-        "desiredCapabilities": {
-            "browserName": "firefox",
-            "marionette": True,
-            "acceptInsecureCerts": True,
-            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-        }
-    }
+    capabilities = (
+        CapabilitiesBuilder()
+        .browser_name("webdriver")
+        .accept_insecure_certs(True)
+        .additional_capability(
+            {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+        )
+    ).build()
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
         driver_url,
         session,
         PAGE_URL,
     )
     yield driver_url, session
```

### Comparing `caqui-2.0.0rc2/tests/integration/test_sync_scenarios.py` & `caqui-2.1.0/tests/integration/test_sync_scenarios.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,28 @@
     get_attribute,
     switch_to_frame,
     switch_to_parent_frame,
     dismiss_alert,
 )
 from tests.constants import PAGE_URL
 from pytest import fixture
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
-    capabilities = {
-        "desiredCapabilities": {
-            "browserName": "chrome",
-            "marionette": True,
-            "acceptInsecureCerts": True,
-            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-        }
-    }
+    capabilities = (
+        CapabilitiesBuilder()
+        .browser_name("webdriver")
+        .accept_insecure_certs(True)
+        .additional_capability(
+            {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+        )
+    ).build()
     session = get_session(driver_url, capabilities)
     go_to_page(
         driver_url,
         session,
         PAGE_URL,
     )
     yield driver_url, session
@@ -98,23 +99,23 @@
 def test_add_text__click_button_and_get_properties(__setup):
     driver_url, session = __setup
     expected = "end"
     locator_type = "xpath"
 
     input = find_element(driver_url, session, locator_type, locator_value="//input")
     send_keys(driver_url, session, input, "any")
-    assert get_property(driver_url, session, input, property="value") == "any"
+    assert get_property(driver_url, session, input, property_name="value") == "any"
     clear_element(driver_url, session, input)
-    assert get_property(driver_url, session, input, property="value") == ""
+    assert get_property(driver_url, session, input, property_name="value") == ""
 
     anchor = find_element(driver_url, session, locator_type, locator_value="//a")
     assert (
-        get_property(driver_url, session, anchor, property="href") == "http://any1.com/"
+        get_property(driver_url, session, anchor, property_name="href")
+        == "http://any1.com/"
     )
 
     button = find_element(driver_url, session, locator_type, locator_value="//button")
     click(driver_url, session, button)
 
     p = find_element(driver_url, session, locator_type, locator_value="//p[@id='end']")
-    get_text(driver_url, session, p)
 
     assert get_text(driver_url, session, p) == expected
```

### Comparing `caqui-2.0.0rc2/tests/unit/test_async_unit.py` & `caqui-2.1.0/tests/unit/test_async_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/tests/unit/test_by.py` & `caqui-2.1.0/tests/unit/test_by.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from caqui.by import By
 from caqui import synchronous
 from tests.constants import PAGE_URL
 from pytest import fixture, mark
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
-    capabilities = {
-        "desiredCapabilities": {
-            "name": "webdriver",
-            "browserName": "chrome",
-            "marionette": False,
-            "acceptInsecureCerts": True,
-            "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-        }
-    }
+    capabilities = (
+        CapabilitiesBuilder()
+        .browser_name("webdriver")
+        .accept_insecure_certs(True)
+        .additional_capability(
+            {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+        )
+    ).build()
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
         driver_url,
         session,
         PAGE_URL,
     )
     yield driver_url, session
```

### Comparing `caqui-2.0.0rc2/tests/unit/test_helper.py` & `caqui-2.1.0/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/tests/unit/test_objects.py` & `caqui-2.1.0/tests/feature/test_objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from caqui.caqui import AsyncDriver, Element, ActionChains
+from caqui.easy import AsyncDriver, ActionChains
 from caqui.by import By
 from pytest import mark, fixture
 from tests.constants import PAGE_URL
 from caqui import synchronous
+from caqui.easy.capabilities import CapabilitiesBuilder
 
 
 class TestObject:
     @fixture
     def setup(self):
         remote = "http://127.0.0.1:9999"
-        capabilities = {
-            "desiredCapabilities": {
-                By.NAME: "webdriver",
-                "browserName": "chrome",
-                "marionette": False,
-                "acceptInsecureCerts": True,
-                "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
-            }
-        }
+        capabilities = (
+            CapabilitiesBuilder()
+            .browser_name("webdriver")
+            .accept_insecure_certs(True)
+            .additional_capability(
+                {"goog:chromeOptions": {"extensions": [], "args": ["--headless"]}}
+            )
+        ).build()
         driver = AsyncDriver(remote, capabilities, PAGE_URL)
         yield driver
         driver.quit()
 
     @mark.asyncio
     async def test_action_chains(self, setup: AsyncDriver):
         driver = setup
         element = await driver.find_element(By.XPATH, "//button")
         actions = (
-            await driver.actions()
-            .move_to_element(element)
+            await driver.actions.move_to_element(element)
             .scroll_to_element(element)
             .click()
             .perform()
         )
         assert actions is True
 
         actions = (
@@ -105,23 +104,21 @@
     @mark.asyncio
     async def test_find_elements_from_element(self, setup: AsyncDriver):
         driver = setup
         expected = 1
         element = await driver.find_element(locator=By.XPATH, value="//body")
         actual = await element.find_elements(By.XPATH, "//button")
         assert len(actual) >= expected
-        assert isinstance(actual[0], Element)
 
     @mark.asyncio
     async def test_find_element_from_element(self, setup: AsyncDriver):
         driver = setup
         element = await driver.find_element(locator=By.XPATH, value="//body")
         actual = await element.find_element(By.XPATH, "//button")
         assert actual is not None
-        assert isinstance(actual, Element)
 
     @mark.asyncio
     async def test_find_elements(self, setup: AsyncDriver):
         driver = setup
         expected = 1
         actual = await driver.find_elements(locator=By.XPATH, value="//button")
         assert len(actual) >= expected
```

### Comparing `caqui-2.0.0rc2/tests/unit/test_sync_unit.py` & `caqui-2.1.0/tests/unit/test_sync_unit.py`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/.gitignore` & `caqui-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/LICENSE` & `caqui-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-2.0.0rc2/README.md` & `caqui-2.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 000005e0: 7229 2020 207c 2031 3133 2020 2020 2020  r)   | 113      
 000005f0: 2020 2020 207c 2059 2020 2020 2020 207c       | Y       |
 00000600: 204e 6565 6420 746f 2061 6464 2074 6865   Need to add the
 00000610: 2068 6f73 7420 6970 2c20 652e 672e 2022   host ip, e.g. "
 00000620: 2d2d 686f 7374 2031 3233 2e34 352e 362e  --host 123.45.6.
 00000630: 3738 2220 7c0a 7c20 476f 6f67 6c65 2043  78" |.| Google C
 00000640: 6872 6f6d 6520 2020 2020 2020 2020 2020  hrome           
-00000650: 7c20 3131 332c 2031 3134 2020 2020 2020  | 113, 114      
+00000650: 7c20 3131 332b 2020 2020 2020 2020 2020  | 113+          
 00000660: 7c20 5920 2020 2020 2020 7c20 4e65 6564  | Y       | Need
 00000670: 2074 6f20 696e 666f 726d 2061 6c6c 6f77   to inform allow
 00000680: 6564 2069 7073 2074 6f20 636f 6e6e 6563  ed ips to connec
 00000690: 742c 2065 2e67 2022 2d2d 616c 6c6f 7765  t, e.g "--allowe
 000006a0: 642d 6970 733d 3132 332e 3435 2e36 2e37  d-ips=123.45.6.7
 000006b0: 3822 207c 0a7c 204f 7065 7261 2020 2020  8" |.| Opera    
 000006c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
@@ -216,444 +216,565 @@
 00000d70: 2061 7379 6e63 696f 0a69 6d70 6f72 7420   asyncio.import 
 00000d80: 7469 6d65 0a66 726f 6d20 6361 7175 6920  time.from caqui 
 00000d90: 696d 706f 7274 2073 796e 6368 726f 6e6f  import synchrono
 00000da0: 7573 2c20 6173 796e 6368 726f 6e6f 7573  us, asynchronous
 00000db0: 0a66 726f 6d20 6f73 2069 6d70 6f72 7420  .from os import 
 00000dc0: 6765 7463 7764 0a66 726f 6d20 7465 7374  getcwd.from test
 00000dd0: 732e 636f 6e73 7461 6e74 7320 696d 706f  s.constants impo
-00000de0: 7274 2050 4147 455f 5552 4c0a 0a42 4153  rt PAGE_URL..BAS
-00000df0: 455f 4449 5220 3d20 6765 7463 7764 2829  E_DIR = getcwd()
-00000e00: 0a0a 4d41 585f 434f 4e43 5552 5245 4e43  ..MAX_CONCURRENC
-00000e10: 5920 3d20 3520 2023 206e 756d 6265 7220  Y = 5  # number 
-00000e20: 6f66 2077 6562 6472 6976 6572 2069 6e73  of webdriver ins
-00000e30: 7461 6e63 6573 2072 756e 6e69 6e67 0a73  tances running.s
-00000e40: 656d 203d 2061 7379 6e63 696f 2e53 656d  em = asyncio.Sem
-00000e50: 6170 686f 7265 284d 4158 5f43 4f4e 4355  aphore(MAX_CONCU
-00000e60: 5252 454e 4359 290a 0a0a 6173 796e 6320  RRENCY)...async 
-00000e70: 6465 6620 6765 745f 616c 6c5f 6c69 6e6b  def get_all_link
-00000e80: 7328 293a 0a20 2020 2061 7379 6e63 2077  s():.    async w
-00000e90: 6974 6820 7365 6d3a 0a20 2020 2020 2020  ith sem:.       
-00000ea0: 2064 7269 7665 725f 7572 6c20 3d20 2268   driver_url = "h
-00000eb0: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00000ec0: 3939 3939 220a 2020 2020 2020 2020 6361  9999".        ca
-00000ed0: 7061 6269 6c69 7469 6573 203d 207b 0a20  pabilities = {. 
-00000ee0: 2020 2020 2020 2020 2020 2022 6465 7369             "desi
-00000ef0: 7265 6443 6170 6162 696c 6974 6965 7322  redCapabilities"
-00000f00: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000f10: 2020 2020 2262 726f 7773 6572 4e61 6d65      "browserName
-00000f20: 223a 2022 6669 7265 666f 7822 2c0a 2020  ": "firefox",.  
-00000f30: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00000f40: 6172 696f 6e65 7474 6522 3a20 5472 7565  arionette": True
-00000f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000f60: 2020 2261 6363 6570 7449 6e73 6563 7572    "acceptInsecur
-00000f70: 6543 6572 7473 223a 2054 7275 652c 0a20  eCerts": True,. 
-00000f80: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000f90: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00000fa0: 7365 7373 696f 6e20 3d20 6177 6169 7420  session = await 
-00000fb0: 6173 796e 6368 726f 6e6f 7573 2e67 6574  asynchronous.get
-00000fc0: 5f73 6573 7369 6f6e 2864 7269 7665 725f  _session(driver_
-00000fd0: 7572 6c2c 2063 6170 6162 696c 6974 6965  url, capabilitie
-00000fe0: 7329 0a20 2020 2020 2020 2061 7761 6974  s).        await
-00000ff0: 2061 7379 6e63 6872 6f6e 6f75 732e 676f   asynchronous.go
-00001000: 5f74 6f5f 7061 6765 280a 2020 2020 2020  _to_page(.      
-00001010: 2020 2020 2020 6472 6976 6572 5f75 726c        driver_url
-00001020: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00001030: 7373 696f 6e2c 0a20 2020 2020 2020 2020  ssion,.         
-00001040: 2020 2050 4147 455f 5552 4c2c 0a20 2020     PAGE_URL,.   
-00001050: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00001060: 666f 7220 6920 696e 2072 616e 6765 2834  for i in range(4
-00001070: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00001080: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00001090: 2020 6c6f 6361 746f 725f 7661 6c75 6520    locator_value 
-000010a0: 3d20 6622 2f2f 615b 4069 643d 2761 7b69  = f"//a[@id='a{i
-000010b0: 7d27 5d22 0a20 2020 2020 2020 2020 2020  }']".           
-000010c0: 206c 6f63 6174 6f72 5f74 7970 6520 3d20   locator_type = 
-000010d0: 2278 7061 7468 220a 2020 2020 2020 2020  "xpath".        
-000010e0: 2020 2020 616e 6368 6f72 7320 3d20 5b5d      anchors = []
-000010f0: 0a0a 2020 2020 2020 2020 2020 2020 616e  ..            an
-00001100: 6368 6f72 7320 3d20 6177 6169 7420 6173  chors = await as
-00001110: 796e 6368 726f 6e6f 7573 2e66 696e 645f  ynchronous.find_
-00001120: 656c 656d 656e 7473 280a 2020 2020 2020  elements(.      
-00001130: 2020 2020 2020 2020 2020 6472 6976 6572            driver
-00001140: 5f75 726c 2c20 7365 7373 696f 6e2c 206c  _url, session, l
-00001150: 6f63 6174 6f72 5f74 7970 652c 206c 6f63  ocator_type, loc
-00001160: 6174 6f72 5f76 616c 7565 0a20 2020 2020  ator_value.     
-00001170: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001180: 2020 2020 2070 7269 6e74 2866 2246 6f75       print(f"Fou
-00001190: 6e64 207b 6c65 6e28 616e 6368 6f72 7329  nd {len(anchors)
-000011a0: 7d20 6c69 6e6b 7322 290a 0a20 2020 2020  } links")..     
-000011b0: 2020 2066 6f72 2061 6e63 686f 7220 696e     for anchor in
-000011c0: 2061 6e63 686f 7273 3a0a 2020 2020 2020   anchors:.      
-000011d0: 2020 2020 2020 7465 7874 203d 2061 7761        text = awa
-000011e0: 6974 2061 7379 6e63 6872 6f6e 6f75 732e  it asynchronous.
-000011f0: 6765 745f 7072 6f70 6572 7479 2864 7269  get_property(dri
-00001200: 7665 725f 7572 6c2c 2073 6573 7369 6f6e  ver_url, session
-00001210: 2c20 616e 6368 6f72 2c20 2268 7265 6622  , anchor, "href"
-00001220: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001230: 696e 7428 6622 4c69 6e6b 2066 6f75 6e64  int(f"Link found
-00001240: 2027 7b74 6578 747d 2722 290a 0a20 2020   '{text}'")..   
-00001250: 2020 2020 2073 796e 6368 726f 6e6f 7573       synchronous
-00001260: 2e63 6c6f 7365 5f73 6573 7369 6f6e 2864  .close_session(d
-00001270: 7269 7665 725f 7572 6c2c 2073 6573 7369  river_url, sessi
-00001280: 6f6e 290a 0a0a 2320 5265 6665 7265 6e63  on)...# Referenc
-00001290: 653a 2068 7474 7073 3a2f 2f73 7461 636b  e: https://stack
-000012a0: 6f76 6572 666c 6f77 2e63 6f6d 2f71 7565  overflow.com/que
-000012b0: 7374 696f 6e73 2f34 3834 3833 3334 382f  stions/48483348/
-000012c0: 686f 772d 746f 2d6c 696d 6974 2d63 6f6e  how-to-limit-con
-000012d0: 6375 7272 656e 6379 2d77 6974 682d 7079  currency-with-py
-000012e0: 7468 6f6e 2d61 7379 6e63 696f 0a61 7379  thon-asyncio.asy
-000012f0: 6e63 2064 6566 206d 6169 6e28 293a 0a20  nc def main():. 
-00001300: 2020 206e 756d 6265 725f 6f66 5f77 6562     number_of_web
-00001310: 7369 7465 7320 3d20 7261 6e67 6528 3130  sites = range(10
-00001320: 290a 2020 2020 7461 736b 7320 3d20 5b61  ).    tasks = [a
-00001330: 7379 6e63 696f 2e65 6e73 7572 655f 6675  syncio.ensure_fu
-00001340: 7475 7265 2867 6574 5f61 6c6c 5f6c 696e  ture(get_all_lin
-00001350: 6b73 2829 2920 666f 7220 6e75 6d62 6572  ks()) for number
-00001360: 2069 6e20 6e75 6d62 6572 5f6f 665f 7765   in number_of_we
-00001370: 6273 6974 6573 5d0a 2020 2020 6177 6169  bsites].    awai
-00001380: 7420 6173 796e 6369 6f2e 6761 7468 6572  t asyncio.gather
-00001390: 282a 7461 736b 7329 0a0a 0a69 6620 5f5f  (*tasks)...if __
-000013a0: 6e61 6d65 5f5f 203d 3d20 225f 5f6d 6169  name__ == "__mai
-000013b0: 6e5f 5f22 3a0a 2020 2020 7374 6172 7420  n__":.    start 
-000013c0: 3d20 7469 6d65 2e74 696d 6528 290a 2020  = time.time().  
-000013d0: 2020 6c6f 6f70 203d 2061 7379 6e63 696f    loop = asyncio
-000013e0: 2e67 6574 5f65 7665 6e74 5f6c 6f6f 7028  .get_event_loop(
-000013f0: 290a 2020 2020 7472 793a 0a20 2020 2020  ).    try:.     
-00001400: 2020 206c 6f6f 702e 7275 6e5f 756e 7469     loop.run_unti
-00001410: 6c5f 636f 6d70 6c65 7465 286d 6169 6e28  l_complete(main(
-00001420: 2929 0a20 2020 2066 696e 616c 6c79 3a0a  )).    finally:.
-00001430: 2020 2020 2020 2020 6c6f 6f70 2e72 756e          loop.run
-00001440: 5f75 6e74 696c 5f63 6f6d 706c 6574 6528  _until_complete(
-00001450: 6c6f 6f70 2e73 6875 7464 6f77 6e5f 6173  loop.shutdown_as
-00001460: 796e 6367 656e 7328 2929 0a20 2020 2020  yncgens()).     
-00001470: 2020 206c 6f6f 702e 636c 6f73 6528 290a     loop.close().
-00001480: 2020 2020 2020 2020 656e 6420 3d20 7469          end = ti
-00001490: 6d65 2e74 696d 6528 290a 2020 2020 2020  me.time().      
-000014a0: 2020 7072 696e 7428 6622 5469 6d65 3a20    print(f"Time: 
-000014b0: 7b65 6e64 2d73 7461 7274 3a2e 3266 7d20  {end-start:.2f} 
-000014c0: 7365 6322 290a 0a60 6060 0a0a 5275 6e20  sec")..```..Run 
-000014d0: 7468 6520 6669 6c65 0a60 6060 0a70 7974  the file.```.pyt
-000014e0: 686f 6e20 7361 6d70 6c65 2e70 790a 6060  hon sample.py.``
-000014f0: 600a 4f75 7470 7574 0a60 6060 0a46 6f75  `.Output.```.Fou
-00001500: 6e64 2031 206c 696e 6b73 0a46 6f75 6e64  nd 1 links.Found
-00001510: 2031 206c 696e 6b73 0a46 6f75 6e64 2031   1 links.Found 1
-00001520: 206c 696e 6b73 0a46 6f75 6e64 2031 206c   links.Found 1 l
-00001530: 696e 6b73 0a46 6f75 6e64 2031 206c 696e  inks.Found 1 lin
-00001540: 6b73 0a4c 696e 6b20 666f 756e 6420 2768  ks.Link found 'h
-00001550: 7474 703a 2f2f 616e 7934 2e63 6f6d 2f27  ttp://any4.com/'
-00001560: 0a46 6f75 6e64 2031 206c 696e 6b73 0a46  .Found 1 links.F
-00001570: 6f75 6e64 2031 206c 696e 6b73 0a46 6f75  ound 1 links.Fou
-00001580: 6e64 2031 206c 696e 6b73 0a46 6f75 6e64  nd 1 links.Found
-00001590: 2031 206c 696e 6b73 0a46 6f75 6e64 2031   1 links.Found 1
-000015a0: 206c 696e 6b73 0a46 6f75 6e64 2031 206c   links.Found 1 l
-000015b0: 696e 6b73 0a4c 696e 6b20 666f 756e 6420  inks.Link found 
-000015c0: 2768 7474 703a 2f2f 616e 7934 2e63 6f6d  'http://any4.com
-000015d0: 2f27 0a46 6f75 6e64 2031 206c 696e 6b73  /'.Found 1 links
-000015e0: 0a46 6f75 6e64 2031 206c 696e 6b73 0a46  .Found 1 links.F
-000015f0: 6f75 6e64 2031 206c 696e 6b73 0a46 6f75  ound 1 links.Fou
-00001600: 6e64 2031 206c 696e 6b73 0a46 6f75 6e64  nd 1 links.Found
-00001610: 2031 206c 696e 6b73 0a46 6f75 6e64 2031   1 links.Found 1
-00001620: 206c 696e 6b73 0a46 6f75 6e64 2031 206c   links.Found 1 l
-00001630: 696e 6b73 0a4c 696e 6b20 666f 756e 6420  inks.Link found 
-00001640: 2768 7474 703a 2f2f 616e 7934 2e63 6f6d  'http://any4.com
-00001650: 2f27 0a4c 696e 6b20 666f 756e 6420 2768  /'.Link found 'h
-00001660: 7474 703a 2f2f 616e 7934 2e63 6f6d 2f27  ttp://any4.com/'
-00001670: 0a46 6f75 6e64 2031 206c 696e 6b73 0a46  .Found 1 links.F
-00001680: 6f75 6e64 2031 206c 696e 6b73 0a4c 696e  ound 1 links.Lin
-00001690: 6b20 666f 756e 6420 2768 7474 703a 2f2f  k found 'http://
-000016a0: 616e 7934 2e63 6f6d 2f27 0a46 6f75 6e64  any4.com/'.Found
-000016b0: 2031 206c 696e 6b73 0a46 6f75 6e64 2031   1 links.Found 1
-000016c0: 206c 696e 6b73 0a46 6f75 6e64 2031 206c   links.Found 1 l
-000016d0: 696e 6b73 0a46 6f75 6e64 2031 206c 696e  inks.Found 1 lin
-000016e0: 6b73 0a4c 696e 6b20 666f 756e 6420 2768  ks.Link found 'h
-000016f0: 7474 703a 2f2f 616e 7934 2e63 6f6d 2f27  ttp://any4.com/'
-00001700: 0a46 6f75 6e64 2031 206c 696e 6b73 0a46  .Found 1 links.F
-00001710: 6f75 6e64 2031 206c 696e 6b73 0a46 6f75  ound 1 links.Fou
-00001720: 6e64 2031 206c 696e 6b73 0a46 6f75 6e64  nd 1 links.Found
-00001730: 2031 206c 696e 6b73 0a4c 696e 6b20 666f   1 links.Link fo
-00001740: 756e 6420 2768 7474 703a 2f2f 616e 7934  und 'http://any4
-00001750: 2e63 6f6d 2f27 0a46 6f75 6e64 2031 206c  .com/'.Found 1 l
-00001760: 696e 6b73 0a46 6f75 6e64 2031 206c 696e  inks.Found 1 lin
-00001770: 6b73 0a46 6f75 6e64 2031 206c 696e 6b73  ks.Found 1 links
-00001780: 0a46 6f75 6e64 2031 206c 696e 6b73 0a4c  .Found 1 links.L
-00001790: 696e 6b20 666f 756e 6420 2768 7474 703a  ink found 'http:
-000017a0: 2f2f 616e 7934 2e63 6f6d 2f27 0a46 6f75  //any4.com/'.Fou
-000017b0: 6e64 2031 206c 696e 6b73 0a46 6f75 6e64  nd 1 links.Found
-000017c0: 2031 206c 696e 6b73 0a46 6f75 6e64 2031   1 links.Found 1
-000017d0: 206c 696e 6b73 0a46 6f75 6e64 2031 206c   links.Found 1 l
-000017e0: 696e 6b73 0a4c 696e 6b20 666f 756e 6420  inks.Link found 
-000017f0: 2768 7474 703a 2f2f 616e 7934 2e63 6f6d  'http://any4.com
-00001800: 2f27 0a46 6f75 6e64 2031 206c 696e 6b73  /'.Found 1 links
-00001810: 0a46 6f75 6e64 2031 206c 696e 6b73 0a46  .Found 1 links.F
-00001820: 6f75 6e64 2031 206c 696e 6b73 0a46 6f75  ound 1 links.Fou
-00001830: 6e64 2031 206c 696e 6b73 0a4c 696e 6b20  nd 1 links.Link 
-00001840: 666f 756e 6420 2768 7474 703a 2f2f 616e  found 'http://an
-00001850: 7934 2e63 6f6d 2f27 0a54 696d 653a 2035  y4.com/'.Time: 5
-00001860: 2e30 3120 7365 630a 0a60 6060 0a0a 2320  .01 sec..```..# 
-00001870: 4472 6976 6572 2061 7320 7365 7276 6572  Driver as server
-00001880: 0a54 6f20 696c 6c75 7374 7261 7465 2077  .To illustrate w
-00001890: 6861 7420 4920 6d65 616e 2062 7920 2244  hat I mean by "D
-000018a0: 7269 7665 7220 6173 2073 6572 7665 7222  river as server"
-000018b0: 2c20 6c65 7473 2067 6574 205b 6368 726f  , lets get [chro
-000018c0: 6d65 6472 6976 6572 5d28 6874 7470 733a  medriver](https:
-000018d0: 2f2f 6368 726f 6d65 6472 6976 6572 2e63  //chromedriver.c
-000018e0: 6872 6f6d 6975 6d2e 6f72 672f 686f 6d65  hromium.org/home
-000018f0: 2920 616e 6420 6578 6563 7574 6520 6974  ) and execute it
-00001900: 2061 7320 616e 206f 7264 696e 6172 7920   as an ordinary 
-00001910: 7368 656c 6c20 7363 7269 7074 2066 696c  shell script fil
-00001920: 652e 0a0a 6060 600a 2e2f 6368 726f 6d65  e...```../chrome
-00001930: 6472 6976 6572 202d 2d70 6f72 743d 3939  driver --port=99
-00001940: 3939 0a53 7461 7274 696e 6720 4368 726f  99.Starting Chro
-00001950: 6d65 4472 6976 6572 2039 342e 302e 3436  meDriver 94.0.46
-00001960: 3036 2e36 3120 2834 3138 6237 3866 3538  06.61 (418b78f58
-00001970: 3338 6564 3062 3163 3639 6262 3465 3531  38ed0b1c69bb4e51
-00001980: 6561 3032 3532 3137 3138 3534 3931 352d  ea0252171854915-
-00001990: 7265 6673 2f62 7261 6e63 682d 6865 6164  refs/branch-head
-000019a0: 732f 3436 3036 407b 2331 3230 347d 2920  s/4606@{#1204}) 
-000019b0: 6f6e 2070 6f72 7420 3939 3939 0a4f 6e6c  on port 9999.Onl
-000019c0: 7920 6c6f 6361 6c20 636f 6e6e 6563 7469  y local connecti
-000019d0: 6f6e 7320 6172 6520 616c 6c6f 7765 642e  ons are allowed.
-000019e0: 0a50 6c65 6173 6520 7365 6520 6874 7470  .Please see http
-000019f0: 733a 2f2f 6368 726f 6d65 6472 6976 6572  s://chromedriver
-00001a00: 2e63 6872 6f6d 6975 6d2e 6f72 672f 7365  .chromium.org/se
-00001a10: 6375 7269 7479 2d63 6f6e 7369 6465 7261  curity-considera
-00001a20: 7469 6f6e 7320 666f 7220 7375 6767 6573  tions for sugges
-00001a30: 7469 6f6e 7320 6f6e 206b 6565 7069 6e67  tions on keeping
-00001a40: 2043 6872 6f6d 6544 7269 7665 7220 7361   ChromeDriver sa
-00001a50: 6665 2e0a 4368 726f 6d65 4472 6976 6572  fe..ChromeDriver
-00001a60: 2077 6173 2073 7461 7274 6564 2073 7563   was started suc
-00001a70: 6365 7373 6675 6c6c 792e 0a0a 6060 600a  cessfully...```.
-00001a80: 4e6f 7469 6365 2074 6865 2044 7269 7665  Notice the Drive
-00001a90: 7220 6973 2072 756e 6e69 6e67 2061 6e64  r is running and
-00001aa0: 2077 6169 7469 6e67 2066 6f72 2048 5454   waiting for HTT
-00001ab0: 5020 7265 7175 6573 7473 2e0a 0a4c 6574  P requests...Let
-00001ac0: 7320 6f70 656e 2061 206e 6577 2073 6573  s open a new ses
-00001ad0: 7369 6f6e 2061 6761 696e 7374 2069 740a  sion against it.
-00001ae0: 6060 600a 6375 726c 202d 2d6c 6f63 6174  ```.curl --locat
-00001af0: 696f 6e20 2731 3237 2e30 2e30 2e31 3a39  ion '127.0.0.1:9
-00001b00: 3939 392f 7365 7373 696f 6e27 205c 0a2d  999/session' \.-
-00001b10: 2d68 6561 6465 7220 2743 6f6e 7465 6e74  -header 'Content
-00001b20: 2d54 7970 653a 2061 7070 6c69 6361 7469  -Type: applicati
-00001b30: 6f6e 2f6a 736f 6e27 205c 0a2d 2d64 6174  on/json' \.--dat
-00001b40: 6120 277b 0a20 2020 2022 6465 7369 7265  a '{.    "desire
-00001b50: 6443 6170 6162 696c 6974 6965 7322 3a20  dCapabilities": 
-00001b60: 7b0a 2020 2020 2020 2020 2262 726f 7773  {.        "brows
-00001b70: 6572 4e61 6d65 223a 2022 6669 7265 666f  erName": "firefo
-00001b80: 7822 2c0a 2020 2020 2020 2020 226d 6172  x",.        "mar
-00001b90: 696f 6e65 7474 6522 3a20 7472 7565 2c0a  ionette": true,.
-00001ba0: 2020 2020 2020 2020 2261 6363 6570 7449          "acceptI
-00001bb0: 6e73 6563 7572 6543 6572 7473 223a 2074  nsecureCerts": t
-00001bc0: 7275 650a 2020 2020 7d0a 7d27 0a60 6060  rue.    }.}'.```
-00001bd0: 0a48 6572 6520 6973 2074 6865 2072 6573  .Here is the res
-00001be0: 706f 6e73 6520 7265 7475 726e 6564 0a60  ponse returned.`
-00001bf0: 6060 0a7b 0a20 2020 2022 7365 7373 696f  ``.{.    "sessio
-00001c00: 6e49 6422 3a20 2262 3636 3534 3132 3163  nId": "b6654121c
-00001c10: 3462 6131 6538 3339 3564 6564 3733 6132  4ba1e8395ded73a2
-00001c20: 3762 3764 3866 3522 2c0a 2020 2020 2273  7b7d8f5",.    "s
-00001c30: 7461 7475 7322 3a20 302c 0a20 2020 2022  tatus": 0,.    "
-00001c40: 7661 6c75 6522 3a20 7b0a 2020 2020 2020  value": {.      
-00001c50: 2020 2261 6363 6570 7449 6e73 6563 7572    "acceptInsecur
-00001c60: 6543 6572 7473 223a 2074 7275 652c 0a20  eCerts": true,. 
-00001c70: 2020 2020 2020 2022 6163 6365 7074 5373         "acceptSs
-00001c80: 6c43 6572 7473 223a 2074 7275 652c 0a20  lCerts": true,. 
-00001c90: 2020 2020 2020 2022 6170 706c 6963 6174         "applicat
-00001ca0: 696f 6e43 6163 6865 456e 6162 6c65 6422  ionCacheEnabled"
-00001cb0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00001cc0: 2022 6272 6f77 7365 7243 6f6e 6e65 6374   "browserConnect
-00001cd0: 696f 6e45 6e61 626c 6564 223a 2066 616c  ionEnabled": fal
-00001ce0: 7365 2c0a 2020 2020 2020 2020 2262 726f  se,.        "bro
-00001cf0: 7773 6572 4e61 6d65 223a 2022 6368 726f  wserName": "chro
-00001d00: 6d65 222c 0a20 2020 2020 2020 2022 6368  me",.        "ch
-00001d10: 726f 6d65 223a 207b 0a20 2020 2020 2020  rome": {.       
-00001d20: 2020 2020 2022 6368 726f 6d65 6472 6976       "chromedriv
-00001d30: 6572 5665 7273 696f 6e22 3a20 2239 342e  erVersion": "94.
-00001d40: 302e 3436 3036 2e36 3120 2834 3138 6237  0.4606.61 (418b7
-00001d50: 3866 3538 3338 6564 3062 3163 3639 6262  8f5838ed0b1c69bb
-00001d60: 3465 3531 6561 3032 3532 3137 3138 3534  4e51ea0252171854
-00001d70: 3931 352d 7265 6673 2f62 7261 6e63 682d  915-refs/branch-
-00001d80: 6865 6164 732f 3436 3036 407b 2331 3230  heads/4606@{#120
-00001d90: 347d 2922 2c0a 2020 2020 2020 2020 2020  4})",.          
-00001da0: 2020 2275 7365 7244 6174 6144 6972 223a    "userDataDir":
-00001db0: 2022 2f74 6d70 2f2e 636f 6d2e 676f 6f67   "/tmp/.com.goog
-00001dc0: 6c65 2e43 6872 6f6d 652e 7874 5a55 4f6a  le.Chrome.xtZUOj
-00001dd0: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
-00001de0: 2020 2020 2022 6373 7353 656c 6563 746f       "cssSelecto
-00001df0: 7273 456e 6162 6c65 6422 3a20 7472 7565  rsEnabled": true
-00001e00: 2c0a 2020 2020 2020 2020 2264 6174 6162  ,.        "datab
-00001e10: 6173 6545 6e61 626c 6564 223a 2066 616c  aseEnabled": fal
-00001e20: 7365 2c0a 2020 2020 2020 2020 2267 6f6f  se,.        "goo
-00001e30: 673a 6368 726f 6d65 4f70 7469 6f6e 7322  g:chromeOptions"
-00001e40: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001e50: 2264 6562 7567 6765 7241 6464 7265 7373  "debuggerAddress
-00001e60: 223a 2022 6c6f 6361 6c68 6f73 743a 3434  ": "localhost:44
-00001e70: 3433 3722 0a20 2020 2020 2020 207d 2c0a  437".        },.
-00001e80: 2020 2020 2020 2020 2268 616e 646c 6573          "handles
-00001e90: 416c 6572 7473 223a 2074 7275 652c 0a20  Alerts": true,. 
-00001ea0: 2020 2020 2020 2022 6861 7354 6f75 6368         "hasTouch
-00001eb0: 5363 7265 656e 223a 2066 616c 7365 2c0a  Screen": false,.
-00001ec0: 2020 2020 2020 2020 226a 6176 6173 6372          "javascr
-00001ed0: 6970 7445 6e61 626c 6564 223a 2074 7275  iptEnabled": tru
-00001ee0: 652c 0a20 2020 2020 2020 2022 6c6f 6361  e,.        "loca
-00001ef0: 7469 6f6e 436f 6e74 6578 7445 6e61 626c  tionContextEnabl
-00001f00: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00001f10: 2020 2022 6d6f 6269 6c65 456d 756c 6174     "mobileEmulat
-00001f20: 696f 6e45 6e61 626c 6564 223a 2066 616c  ionEnabled": fal
-00001f30: 7365 2c0a 2020 2020 2020 2020 226e 6174  se,.        "nat
-00001f40: 6976 6545 7665 6e74 7322 3a20 7472 7565  iveEvents": true
-00001f50: 2c0a 2020 2020 2020 2020 226e 6574 776f  ,.        "netwo
-00001f60: 726b 436f 6e6e 6563 7469 6f6e 456e 6162  rkConnectionEnab
-00001f70: 6c65 6422 3a20 6661 6c73 652c 0a20 2020  led": false,.   
-00001f80: 2020 2020 2022 7061 6765 4c6f 6164 5374       "pageLoadSt
-00001f90: 7261 7465 6779 223a 2022 6e6f 726d 616c  rategy": "normal
-00001fa0: 222c 0a20 2020 2020 2020 2022 706c 6174  ",.        "plat
-00001fb0: 666f 726d 223a 2022 4c69 6e75 7822 2c0a  form": "Linux",.
-00001fc0: 2020 2020 2020 2020 2270 726f 7879 223a          "proxy":
-00001fd0: 207b 7d2c 0a20 2020 2020 2020 2022 726f   {},.        "ro
-00001fe0: 7461 7461 626c 6522 3a20 6661 6c73 652c  tatable": false,
-00001ff0: 0a20 2020 2020 2020 2022 7365 7457 696e  .        "setWin
-00002000: 646f 7752 6563 7422 3a20 7472 7565 2c0a  dowRect": true,.
-00002010: 2020 2020 2020 2020 2273 7472 6963 7446          "strictF
-00002020: 696c 6549 6e74 6572 6163 7461 6269 6c69  ileInteractabili
-00002030: 7479 223a 2066 616c 7365 2c0a 2020 2020  ty": false,.    
-00002040: 2020 2020 2274 616b 6573 4865 6170 536e      "takesHeapSn
-00002050: 6170 7368 6f74 223a 2074 7275 652c 0a20  apshot": true,. 
-00002060: 2020 2020 2020 2022 7461 6b65 7353 6372         "takesScr
-00002070: 6565 6e73 686f 7422 3a20 7472 7565 2c0a  eenshot": true,.
-00002080: 2020 2020 2020 2020 2274 696d 656f 7574          "timeout
-00002090: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000020a0: 2020 2269 6d70 6c69 6369 7422 3a20 302c    "implicit": 0,
-000020b0: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
-000020c0: 6765 4c6f 6164 223a 2033 3030 3030 302c  geLoad": 300000,
-000020d0: 0a20 2020 2020 2020 2020 2020 2022 7363  .            "sc
-000020e0: 7269 7074 223a 2033 3030 3030 0a20 2020  ript": 30000.   
-000020f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00002100: 2275 6e65 7870 6563 7465 6441 6c65 7274  "unexpectedAlert
-00002110: 4265 6861 7669 6f75 7222 3a20 2269 676e  Behaviour": "ign
-00002120: 6f72 6522 2c0a 2020 2020 2020 2020 2276  ore",.        "v
-00002130: 6572 7369 6f6e 223a 2022 3934 2e30 2e34  ersion": "94.0.4
-00002140: 3630 362e 3534 222c 0a20 2020 2020 2020  606.54",.       
-00002150: 2022 7765 6253 746f 7261 6765 456e 6162   "webStorageEnab
-00002160: 6c65 6422 3a20 7472 7565 2c0a 2020 2020  led": true,.    
-00002170: 2020 2020 2277 6562 6175 7468 6e3a 6578      "webauthn:ex
-00002180: 7465 6e73 696f 6e3a 6372 6564 426c 6f62  tension:credBlob
-00002190: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-000021a0: 2022 7765 6261 7574 686e 3a65 7874 656e   "webauthn:exten
-000021b0: 7369 6f6e 3a6c 6172 6765 426c 6f62 223a  sion:largeBlob":
-000021c0: 2074 7275 652c 0a20 2020 2020 2020 2022   true,.        "
-000021d0: 7765 6261 7574 686e 3a76 6972 7475 616c  webauthn:virtual
-000021e0: 4175 7468 656e 7469 6361 746f 7273 223a  Authenticators":
-000021f0: 2074 7275 650a 2020 2020 7d0a 7d0a 6060   true.    }.}.``
-00002200: 600a 5468 6520 2a73 6573 7369 6f6e 4964  `.The *sessionId
-00002210: 2a20 7661 6c75 6520 6361 6e20 6265 2075  * value can be u
-00002220: 7365 6420 746f 2070 6572 666f 726d 2066  sed to perform f
-00002230: 7572 7468 6572 2061 6374 696f 6e73 206c  urther actions l
-00002240: 696b 6520 2a66 696e 6420 656c 656d 656e  ike *find elemen
-00002250: 742a 2c20 2a73 656e 6420 6b65 7973 2a20  t*, *send keys* 
-00002260: 6f72 202a 636c 6963 6b2a 2062 7574 746f  or *click* butto
-00002270: 6e73 2e20 4d6f 7265 2064 6574 6169 6c73  ns. More details
-00002280: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
-00002290: 205b 4a73 6f6e 2057 6972 6520 5072 6f74   [Json Wire Prot
-000022a0: 6f63 6f6c 2053 7065 6369 6669 6361 7469  ocol Specificati
-000022b0: 6f6e 5d28 6874 7470 733a 2f2f 7777 772e  on](https://www.
-000022c0: 7365 6c65 6e69 756d 2e64 6576 2f64 6f63  selenium.dev/doc
-000022d0: 756d 656e 7461 7469 6f6e 2f6c 6567 6163  umentation/legac
-000022e0: 792f 6a73 6f6e 5f77 6972 655f 7072 6f74  y/json_wire_prot
-000022f0: 6f63 6f6c 2f29 2e0a 416c 736f 2077 6974  ocol/)..Also wit
-00002300: 6820 7468 6520 2a2d 682a 2070 6172 616d  h the *-h* param
-00002310: 6574 6572 2069 6e20 4472 6976 6572 732c  eter in Drivers,
-00002320: 2066 6f72 2065 7861 6d70 6c65 3a20 0a60   for example: .`
-00002330: 6060 0a2e 2f63 6872 6f6d 6564 7269 7665  ``../chromedrive
-00002340: 7220 2d68 0a0a 5573 6167 653a 202e 2f63  r -h..Usage: ./c
-00002350: 6872 6f6d 6564 7269 7665 7220 5b4f 5054  hromedriver [OPT
-00002360: 494f 4e53 5d0a 0a4f 7074 696f 6e73 0a20  IONS]..Options. 
-00002370: 202d 2d70 6f72 743d 504f 5254 2020 2020   --port=PORT    
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2070 6f72 7420 746f 206c 6973 7465 6e20   port to listen 
-000023a0: 6f6e 0a20 202d 2d61 6462 2d70 6f72 743d  on.  --adb-port=
-000023b0: 504f 5254 2020 2020 2020 2020 2020 2020  PORT            
-000023c0: 2020 2020 2061 6462 2073 6572 7665 7220       adb server 
-000023d0: 706f 7274 0a20 202d 2d6c 6f67 2d70 6174  port.  --log-pat
-000023e0: 683d 4649 4c45 2020 2020 2020 2020 2020  h=FILE          
-000023f0: 2020 2020 2020 2077 7269 7465 2073 6572         write ser
-00002400: 7665 7220 6c6f 6720 746f 2066 696c 6520  ver log to file 
-00002410: 696e 7374 6561 6420 6f66 2073 7464 6572  instead of stder
-00002420: 722c 2069 6e63 7265 6173 6573 206c 6f67  r, increases log
-00002430: 206c 6576 656c 2074 6f20 494e 464f 0a20   level to INFO. 
-00002440: 202d 2d6c 6f67 2d6c 6576 656c 3d4c 4556   --log-level=LEV
-00002450: 454c 2020 2020 2020 2020 2020 2020 2020  EL              
-00002460: 2073 6574 206c 6f67 206c 6576 656c 3a20   set log level: 
-00002470: 414c 4c2c 2044 4542 5547 2c20 494e 464f  ALL, DEBUG, INFO
-00002480: 2c20 5741 524e 494e 472c 2053 4556 4552  , WARNING, SEVER
-00002490: 452c 204f 4646 0a20 202d 2d76 6572 626f  E, OFF.  --verbo
-000024a0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
-000024b0: 2020 2020 2020 2020 206c 6f67 2076 6572           log ver
-000024c0: 626f 7365 6c79 2028 6571 7569 7661 6c65  bosely (equivale
-000024d0: 6e74 2074 6f20 2d2d 6c6f 672d 6c65 7665  nt to --log-leve
-000024e0: 6c3d 414c 4c29 0a20 202d 2d73 696c 656e  l=ALL).  --silen
-000024f0: 7420 2020 2020 2020 2020 2020 2020 2020  t               
-00002500: 2020 2020 2020 2020 206c 6f67 206e 6f74           log not
-00002510: 6869 6e67 2028 6571 7569 7661 6c65 6e74  hing (equivalent
-00002520: 2074 6f20 2d2d 6c6f 672d 6c65 7665 6c3d   to --log-level=
-00002530: 4f46 4629 0a20 202d 2d61 7070 656e 642d  OFF).  --append-
-00002540: 6c6f 6720 2020 2020 2020 2020 2020 2020  log             
-00002550: 2020 2020 2020 2061 7070 656e 6420 6c6f         append lo
-00002560: 6720 6669 6c65 2069 6e73 7465 6164 206f  g file instead o
-00002570: 6620 7265 7772 6974 696e 670a 2020 2d2d  f rewriting.  --
-00002580: 7265 706c 6179 6162 6c65 2020 2020 2020  replayable      
-00002590: 2020 2020 2020 2020 2020 2020 2020 2865                (e
-000025a0: 7870 6572 696d 656e 7461 6c29 206c 6f67  xperimental) log
-000025b0: 2076 6572 626f 7365 6c79 2061 6e64 2064   verbosely and d
-000025c0: 6f6e 2774 2074 7275 6e63 6174 6520 6c6f  on't truncate lo
-000025d0: 6e67 2073 7472 696e 6773 2073 6f20 7468  ng strings so th
-000025e0: 6174 2074 6865 206c 6f67 2063 616e 2062  at the log can b
-000025f0: 6520 7265 706c 6179 6564 2e0a 2020 2d2d  e replayed..  --
-00002600: 7665 7273 696f 6e20 2020 2020 2020 2020  version         
-00002610: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002620: 696e 7420 7468 6520 7665 7273 696f 6e20  int the version 
-00002630: 6e75 6d62 6572 2061 6e64 2065 7869 740a  number and exit.
-00002640: 2020 2d2d 7572 6c2d 6261 7365 2020 2020    --url-base    
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2020 6261 7365 2055 524c 2070 6174 6820    base URL path 
-00002670: 7072 6566 6978 2066 6f72 2063 6f6d 6d61  prefix for comma
-00002680: 6e64 732c 2065 2e67 2e20 7764 2f75 726c  nds, e.g. wd/url
-00002690: 0a20 202d 2d72 6561 6461 626c 652d 7469  .  --readable-ti
-000026a0: 6d65 7374 616d 7020 2020 2020 2020 2020  mestamp         
-000026b0: 2020 2061 6464 2072 6561 6461 626c 6520     add readable 
-000026c0: 7469 6d65 7374 616d 7073 2074 6f20 6c6f  timestamps to lo
-000026d0: 670a 2020 2d2d 656e 6162 6c65 2d63 6872  g.  --enable-chr
-000026e0: 6f6d 652d 6c6f 6773 2020 2020 2020 2020  ome-logs        
-000026f0: 2020 2020 7368 6f77 206c 6f67 7320 6672      show logs fr
-00002700: 6f6d 2074 6865 2062 726f 7773 6572 2028  om the browser (
-00002710: 6f76 6572 7269 6465 7320 6f74 6865 7220  overrides other 
-00002720: 6c6f 6767 696e 6720 6f70 7469 6f6e 7329  logging options)
-00002730: 0a20 202d 2d64 6973 6162 6c65 2d64 6576  .  --disable-dev
-00002740: 2d73 686d 2d75 7361 6765 2020 2020 2020  -shm-usage      
-00002750: 2020 2064 6f20 6e6f 7420 7573 6520 2f64     do not use /d
-00002760: 6576 2f73 686d 2028 6164 6420 7468 6973  ev/shm (add this
-00002770: 2073 7769 7463 6820 6966 2073 6565 696e   switch if seein
-00002780: 6720 6572 726f 7273 2072 656c 6174 6564  g errors related
-00002790: 2074 6f20 7368 6172 6564 206d 656d 6f72   to shared memor
-000027a0: 7929 0a20 202d 2d61 6c6c 6f77 6564 2d69  y).  --allowed-i
-000027b0: 7073 2020 2020 2020 2020 2020 2020 2020  ps              
-000027c0: 2020 2020 2063 6f6d 6d61 2d73 6570 6172       comma-separ
-000027d0: 6174 6564 2061 6c6c 6f77 6c69 7374 206f  ated allowlist o
-000027e0: 6620 7265 6d6f 7465 2049 5020 6164 6472  f remote IP addr
-000027f0: 6573 7365 7320 7768 6963 6820 6172 6520  esses which are 
-00002800: 616c 6c6f 7765 6420 746f 2063 6f6e 6e65  allowed to conne
-00002810: 6374 2074 6f20 4368 726f 6d65 4472 6976  ct to ChromeDriv
-00002820: 6572 0a60 6060 0a23 2043 6f6e 7472 6962  er.```.# Contrib
-00002830: 7574 696e 670a 5265 6164 2074 6865 205b  uting.Read the [
-00002840: 436f 6465 206f 6620 436f 6e64 7563 745d  Code of Conduct]
-00002850: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002860: 636f 6d2f 646f 7567 6c61 7364 636d 2f63  com/douglasdcm/c
-00002870: 6171 7569 2f62 6c6f 622f 6d61 696e 2f43  aqui/blob/main/C
-00002880: 4f44 455f 4f46 5f43 4f4e 4455 4354 2e6d  ODE_OF_CONDUCT.m
-00002890: 6429 2062 6566 6f72 6520 7075 7368 206e  d) before push n
-000028a0: 6577 204d 6572 6765 2052 6571 7565 7374  ew Merge Request
-000028b0: 732e 0a4e 6f77 2c20 666f 6c6c 6f77 2074  s..Now, follow t
-000028c0: 6865 2073 7465 7073 2069 6e20 5b43 6f6e  he steps in [Con
-000028d0: 7472 6962 7574 696e 675d 2868 7474 7073  tributing](https
-000028e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-000028f0: 7567 6c61 7364 636d 2f63 6171 7569 2f62  uglasdcm/caqui/b
-00002900: 6c6f 622f 6d61 696e 2f43 4f4e 5452 4942  lob/main/CONTRIB
-00002910: 5554 494e 472e 6d64 2920 7365 7373 696f  UTING.md) sessio
-00002920: 6e2e                                     n.
+00000de0: 7274 2050 4147 455f 5552 4c0a 6672 6f6d  rt PAGE_URL.from
+00000df0: 2063 6171 7569 2e65 6173 792e 6361 7061   caqui.easy.capa
+00000e00: 6269 6c69 7469 6573 2069 6d70 6f72 7420  bilities import 
+00000e10: 4361 7061 6269 6c69 7469 6573 4275 696c  CapabilitiesBuil
+00000e20: 6465 720a 0a42 4153 455f 4449 5220 3d20  der..BASE_DIR = 
+00000e30: 6765 7463 7764 2829 0a0a 4d41 585f 434f  getcwd()..MAX_CO
+00000e40: 4e43 5552 5245 4e43 5920 3d20 3520 2023  NCURRENCY = 5  #
+00000e50: 206e 756d 6265 7220 6f66 2077 6562 6472   number of webdr
+00000e60: 6976 6572 2069 6e73 7461 6e63 6573 2072  iver instances r
+00000e70: 756e 6e69 6e67 0a73 656d 203d 2061 7379  unning.sem = asy
+00000e80: 6e63 696f 2e53 656d 6170 686f 7265 284d  ncio.Semaphore(M
+00000e90: 4158 5f43 4f4e 4355 5252 454e 4359 290a  AX_CONCURRENCY).
+00000ea0: 0a0a 6173 796e 6320 6465 6620 6765 745f  ..async def get_
+00000eb0: 616c 6c5f 6c69 6e6b 7328 293a 0a20 2020  all_links():.   
+00000ec0: 2061 7379 6e63 2077 6974 6820 7365 6d3a   async with sem:
+00000ed0: 0a20 2020 2020 2020 2064 7269 7665 725f  .        driver_
+00000ee0: 7572 6c20 3d20 2268 7474 703a 2f2f 3132  url = "http://12
+00000ef0: 372e 302e 302e 313a 3939 3939 220a 2020  7.0.0.1:9999".  
+00000f00: 2020 2020 2020 6361 7061 6269 6c69 7469        capabiliti
+00000f10: 6573 203d 2028 0a20 2020 2020 2020 2020  es = (.         
+00000f20: 2020 2043 6170 6162 696c 6974 6965 7342     CapabilitiesB
+00000f30: 7569 6c64 6572 2829 0a20 2020 2020 2020  uilder().       
+00000f40: 2020 2020 202e 6272 6f77 7365 725f 6e61       .browser_na
+00000f50: 6d65 2822 7765 6264 7269 7665 7222 290a  me("webdriver").
+00000f60: 2020 2020 2020 2020 2020 2020 2e61 6363              .acc
+00000f70: 6570 745f 696e 7365 6375 7265 5f63 6572  ept_insecure_cer
+00000f80: 7473 2854 7275 6529 0a20 2020 2020 2020  ts(True).       
+00000f90: 2020 2020 202e 6164 6469 7469 6f6e 616c       .additional
+00000fa0: 5f63 6170 6162 696c 6974 7928 0a20 2020  _capability(.   
+00000fb0: 2020 2020 2020 2020 2020 2020 207b 2267               {"g
+00000fc0: 6f6f 673a 6368 726f 6d65 4f70 7469 6f6e  oog:chromeOption
+00000fd0: 7322 3a20 7b22 6578 7465 6e73 696f 6e73  s": {"extensions
+00000fe0: 223a 205b 5d2c 2022 6172 6773 223a 205b  ": [], "args": [
+00000ff0: 222d 2d68 6561 646c 6573 7322 5d7d 7d0a  "--headless"]}}.
+00001000: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001010: 2020 2020 2020 292e 6275 696c 6428 290a        ).build().
+00001020: 0a20 2020 2020 2020 2073 6573 7369 6f6e  .        session
+00001030: 203d 2061 7761 6974 2061 7379 6e63 6872   = await asynchr
+00001040: 6f6e 6f75 732e 6765 745f 7365 7373 696f  onous.get_sessio
+00001050: 6e28 6472 6976 6572 5f75 726c 2c20 6361  n(driver_url, ca
+00001060: 7061 6269 6c69 7469 6573 290a 2020 2020  pabilities).    
+00001070: 2020 2020 6177 6169 7420 6173 796e 6368      await asynch
+00001080: 726f 6e6f 7573 2e67 6f5f 746f 5f70 6167  ronous.go_to_pag
+00001090: 6528 0a20 2020 2020 2020 2020 2020 2064  e(.            d
+000010a0: 7269 7665 725f 7572 6c2c 0a20 2020 2020  river_url,.     
+000010b0: 2020 2020 2020 2073 6573 7369 6f6e 2c0a         session,.
+000010c0: 2020 2020 2020 2020 2020 2020 5041 4745              PAGE
+000010d0: 5f55 524c 2c0a 2020 2020 2020 2020 290a  _URL,.        ).
+000010e0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+000010f0: 6e20 7261 6e67 6528 3429 3a0a 2020 2020  n range(4):.    
+00001100: 2020 2020 2020 2020 6920 2b3d 2031 0a20          i += 1. 
+00001110: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
+00001120: 6f72 5f76 616c 7565 203d 2066 222f 2f61  or_value = f"//a
+00001130: 5b40 6964 3d27 617b 697d 275d 220a 2020  [@id='a{i}']".  
+00001140: 2020 2020 2020 2020 2020 6c6f 6361 746f            locato
+00001150: 725f 7479 7065 203d 2022 7870 6174 6822  r_type = "xpath"
+00001160: 0a20 2020 2020 2020 2020 2020 2061 6e63  .            anc
+00001170: 686f 7273 203d 205b 5d0a 0a20 2020 2020  hors = []..     
+00001180: 2020 2020 2020 2061 6e63 686f 7273 203d         anchors =
+00001190: 2061 7761 6974 2061 7379 6e63 6872 6f6e   await asynchron
+000011a0: 6f75 732e 6669 6e64 5f65 6c65 6d65 6e74  ous.find_element
+000011b0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+000011c0: 2020 2064 7269 7665 725f 7572 6c2c 2073     driver_url, s
+000011d0: 6573 7369 6f6e 2c20 6c6f 6361 746f 725f  ession, locator_
+000011e0: 7479 7065 2c20 6c6f 6361 746f 725f 7661  type, locator_va
+000011f0: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
+00001200: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00001210: 696e 7428 6622 466f 756e 6420 7b6c 656e  int(f"Found {len
+00001220: 2861 6e63 686f 7273 297d 206c 696e 6b73  (anchors)} links
+00001230: 2229 0a0a 2020 2020 2020 2020 666f 7220  ")..        for 
+00001240: 616e 6368 6f72 2069 6e20 616e 6368 6f72  anchor in anchor
+00001250: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+00001260: 6578 7420 3d20 6177 6169 7420 6173 796e  ext = await asyn
+00001270: 6368 726f 6e6f 7573 2e67 6574 5f70 726f  chronous.get_pro
+00001280: 7065 7274 7928 6472 6976 6572 5f75 726c  perty(driver_url
+00001290: 2c20 7365 7373 696f 6e2c 2061 6e63 686f  , session, ancho
+000012a0: 722c 2022 6872 6566 2229 0a20 2020 2020  r, "href").     
+000012b0: 2020 2020 2020 2070 7269 6e74 2866 224c         print(f"L
+000012c0: 696e 6b20 666f 756e 6420 277b 7465 7874  ink found '{text
+000012d0: 7d27 2229 0a0a 2020 2020 2020 2020 7379  }'")..        sy
+000012e0: 6e63 6872 6f6e 6f75 732e 636c 6f73 655f  nchronous.close_
+000012f0: 7365 7373 696f 6e28 6472 6976 6572 5f75  session(driver_u
+00001300: 726c 2c20 7365 7373 696f 6e29 0a0a 0a23  rl, session)...#
+00001310: 2052 6566 6572 656e 6365 3a20 6874 7470   Reference: http
+00001320: 733a 2f2f 7374 6163 6b6f 7665 7266 6c6f  s://stackoverflo
+00001330: 772e 636f 6d2f 7175 6573 7469 6f6e 732f  w.com/questions/
+00001340: 3438 3438 3333 3438 2f68 6f77 2d74 6f2d  48483348/how-to-
+00001350: 6c69 6d69 742d 636f 6e63 7572 7265 6e63  limit-concurrenc
+00001360: 792d 7769 7468 2d70 7974 686f 6e2d 6173  y-with-python-as
+00001370: 796e 6369 6f0a 6173 796e 6320 6465 6620  yncio.async def 
+00001380: 6d61 696e 2829 3a0a 2020 2020 6e75 6d62  main():.    numb
+00001390: 6572 5f6f 665f 7765 6273 6974 6573 203d  er_of_websites =
+000013a0: 2072 616e 6765 2831 3029 0a20 2020 2074   range(10).    t
+000013b0: 6173 6b73 203d 205b 6173 796e 6369 6f2e  asks = [asyncio.
+000013c0: 656e 7375 7265 5f66 7574 7572 6528 6765  ensure_future(ge
+000013d0: 745f 616c 6c5f 6c69 6e6b 7328 2929 2066  t_all_links()) f
+000013e0: 6f72 206e 756d 6265 7220 696e 206e 756d  or number in num
+000013f0: 6265 725f 6f66 5f77 6562 7369 7465 735d  ber_of_websites]
+00001400: 0a20 2020 2061 7761 6974 2061 7379 6e63  .    await async
+00001410: 696f 2e67 6174 6865 7228 2a74 6173 6b73  io.gather(*tasks
+00001420: 290a 0a0a 6966 205f 5f6e 616d 655f 5f20  )...if __name__ 
+00001430: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
+00001440: 2020 2073 7461 7274 203d 2074 696d 652e     start = time.
+00001450: 7469 6d65 2829 0a20 2020 206c 6f6f 7020  time().    loop 
+00001460: 3d20 6173 796e 6369 6f2e 6765 745f 6576  = asyncio.get_ev
+00001470: 656e 745f 6c6f 6f70 2829 0a20 2020 2074  ent_loop().    t
+00001480: 7279 3a0a 2020 2020 2020 2020 6c6f 6f70  ry:.        loop
+00001490: 2e72 756e 5f75 6e74 696c 5f63 6f6d 706c  .run_until_compl
+000014a0: 6574 6528 6d61 696e 2829 290a 2020 2020  ete(main()).    
+000014b0: 6669 6e61 6c6c 793a 0a20 2020 2020 2020  finally:.       
+000014c0: 206c 6f6f 702e 7275 6e5f 756e 7469 6c5f   loop.run_until_
+000014d0: 636f 6d70 6c65 7465 286c 6f6f 702e 7368  complete(loop.sh
+000014e0: 7574 646f 776e 5f61 7379 6e63 6765 6e73  utdown_asyncgens
+000014f0: 2829 290a 2020 2020 2020 2020 6c6f 6f70  ()).        loop
+00001500: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00001510: 2065 6e64 203d 2074 696d 652e 7469 6d65   end = time.time
+00001520: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
+00001530: 2866 2254 696d 653a 207b 656e 642d 7374  (f"Time: {end-st
+00001540: 6172 743a 2e32 667d 2073 6563 2229 0a0a  art:.2f} sec")..
+00001550: 6060 600a 0a52 756e 2074 6865 2066 696c  ```..Run the fil
+00001560: 650a 6060 600a 7079 7468 6f6e 2073 616d  e.```.python sam
+00001570: 706c 652e 7079 0a60 6060 0a4f 7574 7075  ple.py.```.Outpu
+00001580: 740a 6060 600a 466f 756e 6420 3120 6c69  t.```.Found 1 li
+00001590: 6e6b 730a 466f 756e 6420 3120 6c69 6e6b  nks.Found 1 link
+000015a0: 730a 466f 756e 6420 3120 6c69 6e6b 730a  s.Found 1 links.
+000015b0: 466f 756e 6420 3120 6c69 6e6b 730a 466f  Found 1 links.Fo
+000015c0: 756e 6420 3120 6c69 6e6b 730a 4c69 6e6b  und 1 links.Link
+000015d0: 2066 6f75 6e64 2027 6874 7470 3a2f 2f61   found 'http://a
+000015e0: 6e79 342e 636f 6d2f 270a 466f 756e 6420  ny4.com/'.Found 
+000015f0: 3120 6c69 6e6b 730a 466f 756e 6420 3120  1 links.Found 1 
+00001600: 6c69 6e6b 730a 466f 756e 6420 3120 6c69  links.Found 1 li
+00001610: 6e6b 730a 466f 756e 6420 3120 6c69 6e6b  nks.Found 1 link
+00001620: 730a 466f 756e 6420 3120 6c69 6e6b 730a  s.Found 1 links.
+00001630: 466f 756e 6420 3120 6c69 6e6b 730a 4c69  Found 1 links.Li
+00001640: 6e6b 2066 6f75 6e64 2027 6874 7470 3a2f  nk found 'http:/
+00001650: 2f61 6e79 342e 636f 6d2f 270a 466f 756e  /any4.com/'.Foun
+00001660: 6420 3120 6c69 6e6b 730a 466f 756e 6420  d 1 links.Found 
+00001670: 3120 6c69 6e6b 730a 466f 756e 6420 3120  1 links.Found 1 
+00001680: 6c69 6e6b 730a 466f 756e 6420 3120 6c69  links.Found 1 li
+00001690: 6e6b 730a 466f 756e 6420 3120 6c69 6e6b  nks.Found 1 link
+000016a0: 730a 466f 756e 6420 3120 6c69 6e6b 730a  s.Found 1 links.
+000016b0: 466f 756e 6420 3120 6c69 6e6b 730a 4c69  Found 1 links.Li
+000016c0: 6e6b 2066 6f75 6e64 2027 6874 7470 3a2f  nk found 'http:/
+000016d0: 2f61 6e79 342e 636f 6d2f 270a 4c69 6e6b  /any4.com/'.Link
+000016e0: 2066 6f75 6e64 2027 6874 7470 3a2f 2f61   found 'http://a
+000016f0: 6e79 342e 636f 6d2f 270a 466f 756e 6420  ny4.com/'.Found 
+00001700: 3120 6c69 6e6b 730a 466f 756e 6420 3120  1 links.Found 1 
+00001710: 6c69 6e6b 730a 4c69 6e6b 2066 6f75 6e64  links.Link found
+00001720: 2027 6874 7470 3a2f 2f61 6e79 342e 636f   'http://any4.co
+00001730: 6d2f 270a 466f 756e 6420 3120 6c69 6e6b  m/'.Found 1 link
+00001740: 730a 466f 756e 6420 3120 6c69 6e6b 730a  s.Found 1 links.
+00001750: 466f 756e 6420 3120 6c69 6e6b 730a 466f  Found 1 links.Fo
+00001760: 756e 6420 3120 6c69 6e6b 730a 4c69 6e6b  und 1 links.Link
+00001770: 2066 6f75 6e64 2027 6874 7470 3a2f 2f61   found 'http://a
+00001780: 6e79 342e 636f 6d2f 270a 466f 756e 6420  ny4.com/'.Found 
+00001790: 3120 6c69 6e6b 730a 466f 756e 6420 3120  1 links.Found 1 
+000017a0: 6c69 6e6b 730a 466f 756e 6420 3120 6c69  links.Found 1 li
+000017b0: 6e6b 730a 466f 756e 6420 3120 6c69 6e6b  nks.Found 1 link
+000017c0: 730a 4c69 6e6b 2066 6f75 6e64 2027 6874  s.Link found 'ht
+000017d0: 7470 3a2f 2f61 6e79 342e 636f 6d2f 270a  tp://any4.com/'.
+000017e0: 466f 756e 6420 3120 6c69 6e6b 730a 466f  Found 1 links.Fo
+000017f0: 756e 6420 3120 6c69 6e6b 730a 466f 756e  und 1 links.Foun
+00001800: 6420 3120 6c69 6e6b 730a 466f 756e 6420  d 1 links.Found 
+00001810: 3120 6c69 6e6b 730a 4c69 6e6b 2066 6f75  1 links.Link fou
+00001820: 6e64 2027 6874 7470 3a2f 2f61 6e79 342e  nd 'http://any4.
+00001830: 636f 6d2f 270a 466f 756e 6420 3120 6c69  com/'.Found 1 li
+00001840: 6e6b 730a 466f 756e 6420 3120 6c69 6e6b  nks.Found 1 link
+00001850: 730a 466f 756e 6420 3120 6c69 6e6b 730a  s.Found 1 links.
+00001860: 466f 756e 6420 3120 6c69 6e6b 730a 4c69  Found 1 links.Li
+00001870: 6e6b 2066 6f75 6e64 2027 6874 7470 3a2f  nk found 'http:/
+00001880: 2f61 6e79 342e 636f 6d2f 270a 466f 756e  /any4.com/'.Foun
+00001890: 6420 3120 6c69 6e6b 730a 466f 756e 6420  d 1 links.Found 
+000018a0: 3120 6c69 6e6b 730a 466f 756e 6420 3120  1 links.Found 1 
+000018b0: 6c69 6e6b 730a 466f 756e 6420 3120 6c69  links.Found 1 li
+000018c0: 6e6b 730a 4c69 6e6b 2066 6f75 6e64 2027  nks.Link found '
+000018d0: 6874 7470 3a2f 2f61 6e79 342e 636f 6d2f  http://any4.com/
+000018e0: 270a 5469 6d65 3a20 352e 3031 2073 6563  '.Time: 5.01 sec
+000018f0: 0a0a 6060 600a 2320 5665 7273 696f 6e20  ..```.# Version 
+00001900: 322e 302e 300a 496e 2076 6572 7369 6f6e  2.0.0.In version
+00001910: 2032 2069 7420 6973 2070 6f73 7369 626c   2 it is possibl
+00001920: 6520 746f 2075 7365 2050 7974 686f 6e20  e to use Python 
+00001930: 6f62 6a65 6374 7320 7369 6d69 6c61 726c  objects similarl
+00001940: 7920 746f 2053 656c 656e 6975 6d2e 2045  y to Selenium. E
+00001950: 7861 6d70 6c65 3a0a 0a60 6060 0a66 726f  xample:..```.fro
+00001960: 6d20 6361 7175 692e 6561 7379 2069 6d70  m caqui.easy imp
+00001970: 6f72 7420 4173 796e 6344 7269 7665 720a  ort AsyncDriver.
+00001980: 6672 6f6d 2063 6171 7569 2e62 7920 696d  from caqui.by im
+00001990: 706f 7274 2042 790a 6672 6f6d 2063 6171  port By.from caq
+000019a0: 7569 2069 6d70 6f72 7420 7379 6e63 6872  ui import synchr
+000019b0: 6f6e 6f75 730a 6672 6f6d 2074 6573 7473  onous.from tests
+000019c0: 2e63 6f6e 7374 616e 7473 2069 6d70 6f72  .constants impor
+000019d0: 7420 5041 4745 5f55 524c 0a66 726f 6d20  t PAGE_URL.from 
+000019e0: 7079 7465 7374 2069 6d70 6f72 7420 6d61  pytest import ma
+000019f0: 726b 2c20 6669 7874 7572 650a 6672 6f6d  rk, fixture.from
+00001a00: 2063 6171 7569 2e65 6173 792e 6361 7061   caqui.easy.capa
+00001a10: 6269 6c69 7469 6573 2069 6d70 6f72 7420  bilities import 
+00001a20: 4361 7061 6269 6c69 7469 6573 4275 696c  CapabilitiesBuil
+00001a30: 6465 720a 0a0a 4066 6978 7475 7265 0a64  der...@fixture.d
+00001a40: 6566 205f 5f73 6574 7570 2829 3a0a 2020  ef __setup():.  
+00001a50: 2020 7265 6d6f 7465 203d 2022 6874 7470    remote = "http
+00001a60: 3a2f 2f31 3237 2e30 2e30 2e31 3a39 3939  ://127.0.0.1:999
+00001a70: 3922 0a20 2020 2063 6170 6162 696c 6974  9".    capabilit
+00001a80: 6965 7320 3d20 280a 2020 2020 2020 2020  ies = (.        
+00001a90: 4361 7061 6269 6c69 7469 6573 4275 696c  CapabilitiesBuil
+00001aa0: 6465 7228 290a 2020 2020 2020 2020 2e62  der().        .b
+00001ab0: 726f 7773 6572 5f6e 616d 6528 2277 6562  rowser_name("web
+00001ac0: 6472 6976 6572 2229 0a20 2020 2020 2020  driver").       
+00001ad0: 202e 6163 6365 7074 5f69 6e73 6563 7572   .accept_insecur
+00001ae0: 655f 6365 7274 7328 5472 7565 290a 2020  e_certs(True).  
+00001af0: 2020 2020 2020 2e70 6167 655f 6c6f 6164        .page_load
+00001b00: 5f73 7472 6174 6567 7928 226e 6f72 6d61  _strategy("norma
+00001b10: 6c22 290a 2020 2020 2020 2020 2e61 6464  l").        .add
+00001b20: 7469 6f6e 616c 5f63 6170 6162 696c 6974  tional_capabilit
+00001b30: 7928 0a20 2020 2020 2020 2020 2020 207b  y(.            {
+00001b40: 2267 6f6f 673a 6368 726f 6d65 4f70 7469  "goog:chromeOpti
+00001b50: 6f6e 7322 3a20 7b22 6578 7465 6e73 696f  ons": {"extensio
+00001b60: 6e73 223a 205b 5d2c 2022 6172 6773 223a  ns": [], "args":
+00001b70: 205b 222d 2d68 6561 646c 6573 7322 5d7d   ["--headless"]}
+00001b80: 7d0a 2020 2020 2020 2020 290a 2020 2020  }.        ).    
+00001b90: 292e 6275 696c 6428 290a 2020 2020 6472  ).build().    dr
+00001ba0: 6976 6572 203d 2041 7379 6e63 4472 6976  iver = AsyncDriv
+00001bb0: 6572 2872 656d 6f74 652c 2063 6170 6162  er(remote, capab
+00001bc0: 696c 6974 6965 732c 2050 4147 455f 5552  ilities, PAGE_UR
+00001bd0: 4c29 0a20 2020 2079 6965 6c64 2064 7269  L).    yield dri
+00001be0: 7665 720a 2020 2020 6472 6976 6572 2e71  ver.    driver.q
+00001bf0: 7569 7428 290a 0a0a 406d 6172 6b2e 6173  uit()...@mark.as
+00001c00: 796e 6369 6f0a 6173 796e 6320 6465 6620  yncio.async def 
+00001c10: 7465 7374 5f73 7769 7463 685f 746f 5f70  test_switch_to_p
+00001c20: 6172 656e 745f 6672 616d 655f 616e 645f  arent_frame_and_
+00001c30: 636c 6963 6b5f 616c 6572 7428 5f5f 7365  click_alert(__se
+00001c40: 7475 703a 2041 7379 6e63 4472 6976 6572  tup: AsyncDriver
+00001c50: 293a 0a20 2020 2064 7269 7665 7220 3d20  ):.    driver = 
+00001c60: 5f5f 7365 7475 700a 2020 2020 6177 6169  __setup.    awai
+00001c70: 7420 6472 6976 6572 2e67 6574 2850 4147  t driver.get(PAG
+00001c80: 455f 5552 4c29 0a0a 2020 2020 6c6f 6361  E_URL)..    loca
+00001c90: 746f 725f 7479 7065 203d 2022 6964 220a  tor_type = "id".
+00001ca0: 2020 2020 6c6f 6361 746f 725f 7661 6c75      locator_valu
+00001cb0: 6520 3d20 226d 792d 6966 7261 6d65 220a  e = "my-iframe".
+00001cc0: 2020 2020 6c6f 6361 746f 725f 7661 6c75      locator_valu
+00001cd0: 655f 616c 6572 745f 7061 7265 6e74 203d  e_alert_parent =
+00001ce0: 2022 616c 6572 742d 6275 7474 6f6e 220a   "alert-button".
+00001cf0: 2020 2020 6c6f 6361 746f 725f 7661 6c75      locator_valu
+00001d00: 655f 616c 6572 745f 6672 616d 6520 3d20  e_alert_frame = 
+00001d10: 2261 6c65 7274 2d62 7574 746f 6e2d 6966  "alert-button-if
+00001d20: 7261 6d65 220a 0a20 2020 2065 6c65 6d65  rame"..    eleme
+00001d30: 6e74 5f66 7261 6d65 203d 2061 7761 6974  nt_frame = await
+00001d40: 2064 7269 7665 722e 6669 6e64 5f65 6c65   driver.find_ele
+00001d50: 6d65 6e74 286c 6f63 6174 6f72 5f74 7970  ment(locator_typ
+00001d60: 652c 206c 6f63 6174 6f72 5f76 616c 7565  e, locator_value
+00001d70: 290a 2020 2020 6173 7365 7274 2061 7761  ).    assert awa
+00001d80: 6974 2064 7269 7665 722e 7377 6974 6368  it driver.switch
+00001d90: 5f74 6f2e 6672 616d 6528 656c 656d 656e  _to.frame(elemen
+00001da0: 745f 6672 616d 6529 2069 7320 5472 7565  t_frame) is True
+00001db0: 0a0a 2020 2020 616c 6572 745f 6275 7474  ..    alert_butt
+00001dc0: 6f6e 5f66 7261 6d65 203d 2061 7761 6974  on_frame = await
+00001dd0: 2064 7269 7665 722e 6669 6e64 5f65 6c65   driver.find_ele
+00001de0: 6d65 6e74 280a 2020 2020 2020 2020 6c6f  ment(.        lo
+00001df0: 6361 746f 725f 7479 7065 2c20 6c6f 6361  cator_type, loca
+00001e00: 746f 725f 7661 6c75 655f 616c 6572 745f  tor_value_alert_
+00001e10: 6672 616d 650a 2020 2020 290a 2020 2020  frame.    ).    
+00001e20: 6173 7365 7274 2061 7761 6974 2061 6c65  assert await ale
+00001e30: 7274 5f62 7574 746f 6e5f 6672 616d 652e  rt_button_frame.
+00001e40: 636c 6963 6b28 2920 6973 2054 7275 650a  click() is True.
+00001e50: 2020 2020 6173 7365 7274 2061 7761 6974      assert await
+00001e60: 2064 7269 7665 722e 7377 6974 6368 5f74   driver.switch_t
+00001e70: 6f2e 616c 6572 742e 6469 736d 6973 7328  o.alert.dismiss(
+00001e80: 2920 6973 2054 7275 650a 0a20 2020 2061  ) is True..    a
+00001e90: 7373 6572 7420 6177 6169 7420 6472 6976  ssert await driv
+00001ea0: 6572 2e73 7769 7463 685f 746f 2e64 6566  er.switch_to.def
+00001eb0: 6175 6c74 5f63 6f6e 7465 6e74 2829 2069  ault_content() i
+00001ec0: 7320 5472 7565 0a20 2020 2061 6c65 7274  s True.    alert
+00001ed0: 5f62 7574 746f 6e5f 7061 7265 6e74 203d  _button_parent =
+00001ee0: 2061 7761 6974 2064 7269 7665 722e 6669   await driver.fi
+00001ef0: 6e64 5f65 6c65 6d65 6e74 280a 2020 2020  nd_element(.    
+00001f00: 2020 2020 6c6f 6361 746f 725f 7479 7065      locator_type
+00001f10: 2c20 6c6f 6361 746f 725f 7661 6c75 655f  , locator_value_
+00001f20: 616c 6572 745f 7061 7265 6e74 0a20 2020  alert_parent.   
+00001f30: 2029 0a20 2020 2061 7373 6572 7420 6177   ).    assert aw
+00001f40: 6169 7420 616c 6572 745f 6275 7474 6f6e  ait alert_button
+00001f50: 5f70 6172 656e 742e 6765 745f 6174 7472  _parent.get_attr
+00001f60: 6962 7574 6528 2261 6e79 2229 203d 3d20  ibute("any") == 
+00001f70: 2261 6e79 220a 2020 2020 6173 7365 7274  "any".    assert
+00001f80: 2061 7761 6974 2061 6c65 7274 5f62 7574   await alert_but
+00001f90: 746f 6e5f 7061 7265 6e74 2e63 6c69 636b  ton_parent.click
+00001fa0: 2829 2069 7320 5472 7565 0a0a 0a28 2273  () is True...("s
+00001fb0: 7479 6c65 2229 0a20 2020 2061 7373 6572  tyle").    asser
+00001fc0: 7420 2264 6973 706c 6179 3a20 6e6f 6e65  t "display: none
+00001fd0: 3b22 203d 3d20 6177 6169 7420 6869 6464  ;" == await hidd
+00001fe0: 656e 5f62 7574 746f 6e2e 6765 745f 6174  en_button.get_at
+00001ff0: 7472 6962 7574 6528 2273 7479 6c65 2229  tribute("style")
+00002000: 0a0a 6060 600a 0a0a 2320 4472 6976 6572  ..```...# Driver
+00002010: 2061 7320 7365 7276 6572 0a54 6f20 696c   as server.To il
+00002020: 6c75 7374 7261 7465 2077 6861 7420 4920  lustrate what I 
+00002030: 6d65 616e 2062 7920 2244 7269 7665 7220  mean by "Driver 
+00002040: 6173 2073 6572 7665 7222 2c20 6c65 7473  as server", lets
+00002050: 2067 6574 205b 6368 726f 6d65 6472 6976   get [chromedriv
+00002060: 6572 5d28 6874 7470 733a 2f2f 6368 726f  er](https://chro
+00002070: 6d65 6472 6976 6572 2e63 6872 6f6d 6975  medriver.chromiu
+00002080: 6d2e 6f72 672f 686f 6d65 2920 616e 6420  m.org/home) and 
+00002090: 6578 6563 7574 6520 6974 2061 7320 616e  execute it as an
+000020a0: 206f 7264 696e 6172 7920 7368 656c 6c20   ordinary shell 
+000020b0: 7363 7269 7074 2066 696c 652e 0a0a 6060  script file...``
+000020c0: 600a 2e2f 6368 726f 6d65 6472 6976 6572  `../chromedriver
+000020d0: 202d 2d70 6f72 743d 3939 3939 0a53 7461   --port=9999.Sta
+000020e0: 7274 696e 6720 4368 726f 6d65 4472 6976  rting ChromeDriv
+000020f0: 6572 2039 342e 302e 3436 3036 2e36 3120  er 94.0.4606.61 
+00002100: 2834 3138 6237 3866 3538 3338 6564 3062  (418b78f5838ed0b
+00002110: 3163 3639 6262 3465 3531 6561 3032 3532  1c69bb4e51ea0252
+00002120: 3137 3138 3534 3931 352d 7265 6673 2f62  171854915-refs/b
+00002130: 7261 6e63 682d 6865 6164 732f 3436 3036  ranch-heads/4606
+00002140: 407b 2331 3230 347d 2920 6f6e 2070 6f72  @{#1204}) on por
+00002150: 7420 3939 3939 0a4f 6e6c 7920 6c6f 6361  t 9999.Only loca
+00002160: 6c20 636f 6e6e 6563 7469 6f6e 7320 6172  l connections ar
+00002170: 6520 616c 6c6f 7765 642e 0a50 6c65 6173  e allowed..Pleas
+00002180: 6520 7365 6520 6874 7470 733a 2f2f 6368  e see https://ch
+00002190: 726f 6d65 6472 6976 6572 2e63 6872 6f6d  romedriver.chrom
+000021a0: 6975 6d2e 6f72 672f 7365 6375 7269 7479  ium.org/security
+000021b0: 2d63 6f6e 7369 6465 7261 7469 6f6e 7320  -considerations 
+000021c0: 666f 7220 7375 6767 6573 7469 6f6e 7320  for suggestions 
+000021d0: 6f6e 206b 6565 7069 6e67 2043 6872 6f6d  on keeping Chrom
+000021e0: 6544 7269 7665 7220 7361 6665 2e0a 4368  eDriver safe..Ch
+000021f0: 726f 6d65 4472 6976 6572 2077 6173 2073  romeDriver was s
+00002200: 7461 7274 6564 2073 7563 6365 7373 6675  tarted successfu
+00002210: 6c6c 792e 0a0a 6060 600a 4e6f 7469 6365  lly...```.Notice
+00002220: 2074 6865 2044 7269 7665 7220 6973 2072   the Driver is r
+00002230: 756e 6e69 6e67 2061 6e64 2077 6169 7469  unning and waiti
+00002240: 6e67 2066 6f72 2048 5454 5020 7265 7175  ng for HTTP requ
+00002250: 6573 7473 2e0a 0a4c 6574 7320 6f70 656e  ests...Lets open
+00002260: 2061 206e 6577 2073 6573 7369 6f6e 2061   a new session a
+00002270: 6761 696e 7374 2069 740a 6060 600a 6375  gainst it.```.cu
+00002280: 726c 202d 2d6c 6f63 6174 696f 6e20 2731  rl --location '1
+00002290: 3237 2e30 2e30 2e31 3a39 3939 392f 7365  27.0.0.1:9999/se
+000022a0: 7373 696f 6e27 205c 0a2d 2d68 6561 6465  ssion' \.--heade
+000022b0: 7220 2743 6f6e 7465 6e74 2d54 7970 653a  r 'Content-Type:
+000022c0: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
+000022d0: 6e27 205c 0a2d 2d64 6174 6120 277b 0a20  n' \.--data '{. 
+000022e0: 2020 2022 6465 7369 7265 6443 6170 6162     "desiredCapab
+000022f0: 696c 6974 6965 7322 3a20 7b0a 2020 2020  ilities": {.    
+00002300: 2020 2020 2262 726f 7773 6572 4e61 6d65      "browserName
+00002310: 223a 2022 6669 7265 666f 7822 2c0a 2020  ": "firefox",.  
+00002320: 2020 2020 2020 226d 6172 696f 6e65 7474        "marionett
+00002330: 6522 3a20 7472 7565 2c0a 2020 2020 2020  e": true,.      
+00002340: 2020 2261 6363 6570 7449 6e73 6563 7572    "acceptInsecur
+00002350: 6543 6572 7473 223a 2074 7275 650a 2020  eCerts": true.  
+00002360: 2020 7d0a 7d27 0a60 6060 0a48 6572 6520    }.}'.```.Here 
+00002370: 6973 2074 6865 2072 6573 706f 6e73 6520  is the response 
+00002380: 7265 7475 726e 6564 0a60 6060 0a7b 0a20  returned.```.{. 
+00002390: 2020 2022 7365 7373 696f 6e49 6422 3a20     "sessionId": 
+000023a0: 2262 3636 3534 3132 3163 3462 6131 6538  "b6654121c4ba1e8
+000023b0: 3339 3564 6564 3733 6132 3762 3764 3866  395ded73a27b7d8f
+000023c0: 3522 2c0a 2020 2020 2273 7461 7475 7322  5",.    "status"
+000023d0: 3a20 302c 0a20 2020 2022 7661 6c75 6522  : 0,.    "value"
+000023e0: 3a20 7b0a 2020 2020 2020 2020 2261 6363  : {.        "acc
+000023f0: 6570 7449 6e73 6563 7572 6543 6572 7473  eptInsecureCerts
+00002400: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00002410: 2022 6163 6365 7074 5373 6c43 6572 7473   "acceptSslCerts
+00002420: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00002430: 2022 6170 706c 6963 6174 696f 6e43 6163   "applicationCac
+00002440: 6865 456e 6162 6c65 6422 3a20 6661 6c73  heEnabled": fals
+00002450: 652c 0a20 2020 2020 2020 2022 6272 6f77  e,.        "brow
+00002460: 7365 7243 6f6e 6e65 6374 696f 6e45 6e61  serConnectionEna
+00002470: 626c 6564 223a 2066 616c 7365 2c0a 2020  bled": false,.  
+00002480: 2020 2020 2020 2262 726f 7773 6572 4e61        "browserNa
+00002490: 6d65 223a 2022 6368 726f 6d65 222c 0a20  me": "chrome",. 
+000024a0: 2020 2020 2020 2022 6368 726f 6d65 223a         "chrome":
+000024b0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000024c0: 6368 726f 6d65 6472 6976 6572 5665 7273  chromedriverVers
+000024d0: 696f 6e22 3a20 2239 342e 302e 3436 3036  ion": "94.0.4606
+000024e0: 2e36 3120 2834 3138 6237 3866 3538 3338  .61 (418b78f5838
+000024f0: 6564 3062 3163 3639 6262 3465 3531 6561  ed0b1c69bb4e51ea
+00002500: 3032 3532 3137 3138 3534 3931 352d 7265  0252171854915-re
+00002510: 6673 2f62 7261 6e63 682d 6865 6164 732f  fs/branch-heads/
+00002520: 3436 3036 407b 2331 3230 347d 2922 2c0a  4606@{#1204})",.
+00002530: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+00002540: 7244 6174 6144 6972 223a 2022 2f74 6d70  rDataDir": "/tmp
+00002550: 2f2e 636f 6d2e 676f 6f67 6c65 2e43 6872  /.com.google.Chr
+00002560: 6f6d 652e 7874 5a55 4f6a 220a 2020 2020  ome.xtZUOj".    
+00002570: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00002580: 6373 7353 656c 6563 746f 7273 456e 6162  cssSelectorsEnab
+00002590: 6c65 6422 3a20 7472 7565 2c0a 2020 2020  led": true,.    
+000025a0: 2020 2020 2264 6174 6162 6173 6545 6e61      "databaseEna
+000025b0: 626c 6564 223a 2066 616c 7365 2c0a 2020  bled": false,.  
+000025c0: 2020 2020 2020 2267 6f6f 673a 6368 726f        "goog:chro
+000025d0: 6d65 4f70 7469 6f6e 7322 3a20 7b0a 2020  meOptions": {.  
+000025e0: 2020 2020 2020 2020 2020 2264 6562 7567            "debug
+000025f0: 6765 7241 6464 7265 7373 223a 2022 6c6f  gerAddress": "lo
+00002600: 6361 6c68 6f73 743a 3434 3433 3722 0a20  calhost:44437". 
+00002610: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002620: 2020 2268 616e 646c 6573 416c 6572 7473    "handlesAlerts
+00002630: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00002640: 2022 6861 7354 6f75 6368 5363 7265 656e   "hasTouchScreen
+00002650: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00002660: 2020 226a 6176 6173 6372 6970 7445 6e61    "javascriptEna
+00002670: 626c 6564 223a 2074 7275 652c 0a20 2020  bled": true,.   
+00002680: 2020 2020 2022 6c6f 6361 7469 6f6e 436f       "locationCo
+00002690: 6e74 6578 7445 6e61 626c 6564 223a 2074  ntextEnabled": t
+000026a0: 7275 652c 0a20 2020 2020 2020 2022 6d6f  rue,.        "mo
+000026b0: 6269 6c65 456d 756c 6174 696f 6e45 6e61  bileEmulationEna
+000026c0: 626c 6564 223a 2066 616c 7365 2c0a 2020  bled": false,.  
+000026d0: 2020 2020 2020 226e 6174 6976 6545 7665        "nativeEve
+000026e0: 6e74 7322 3a20 7472 7565 2c0a 2020 2020  nts": true,.    
+000026f0: 2020 2020 226e 6574 776f 726b 436f 6e6e      "networkConn
+00002700: 6563 7469 6f6e 456e 6162 6c65 6422 3a20  ectionEnabled": 
+00002710: 6661 6c73 652c 0a20 2020 2020 2020 2022  false,.        "
+00002720: 7061 6765 4c6f 6164 5374 7261 7465 6779  pageLoadStrategy
+00002730: 223a 2022 6e6f 726d 616c 222c 0a20 2020  ": "normal",.   
+00002740: 2020 2020 2022 706c 6174 666f 726d 223a       "platform":
+00002750: 2022 4c69 6e75 7822 2c0a 2020 2020 2020   "Linux",.      
+00002760: 2020 2270 726f 7879 223a 207b 7d2c 0a20    "proxy": {},. 
+00002770: 2020 2020 2020 2022 726f 7461 7461 626c         "rotatabl
+00002780: 6522 3a20 6661 6c73 652c 0a20 2020 2020  e": false,.     
+00002790: 2020 2022 7365 7457 696e 646f 7752 6563     "setWindowRec
+000027a0: 7422 3a20 7472 7565 2c0a 2020 2020 2020  t": true,.      
+000027b0: 2020 2273 7472 6963 7446 696c 6549 6e74    "strictFileInt
+000027c0: 6572 6163 7461 6269 6c69 7479 223a 2066  eractability": f
+000027d0: 616c 7365 2c0a 2020 2020 2020 2020 2274  alse,.        "t
+000027e0: 616b 6573 4865 6170 536e 6170 7368 6f74  akesHeapSnapshot
+000027f0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00002800: 2022 7461 6b65 7353 6372 6565 6e73 686f   "takesScreensho
+00002810: 7422 3a20 7472 7565 2c0a 2020 2020 2020  t": true,.      
+00002820: 2020 2274 696d 656f 7574 7322 3a20 7b0a    "timeouts": {.
+00002830: 2020 2020 2020 2020 2020 2020 2269 6d70              "imp
+00002840: 6c69 6369 7422 3a20 302c 0a20 2020 2020  licit": 0,.     
+00002850: 2020 2020 2020 2022 7061 6765 4c6f 6164         "pageLoad
+00002860: 223a 2033 3030 3030 302c 0a20 2020 2020  ": 300000,.     
+00002870: 2020 2020 2020 2022 7363 7269 7074 223a         "script":
+00002880: 2033 3030 3030 0a20 2020 2020 2020 207d   30000.        }
+00002890: 2c0a 2020 2020 2020 2020 2275 6e65 7870  ,.        "unexp
+000028a0: 6563 7465 6441 6c65 7274 4265 6861 7669  ectedAlertBehavi
+000028b0: 6f75 7222 3a20 2269 676e 6f72 6522 2c0a  our": "ignore",.
+000028c0: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
+000028d0: 223a 2022 3934 2e30 2e34 3630 362e 3534  ": "94.0.4606.54
+000028e0: 222c 0a20 2020 2020 2020 2022 7765 6253  ",.        "webS
+000028f0: 746f 7261 6765 456e 6162 6c65 6422 3a20  torageEnabled": 
+00002900: 7472 7565 2c0a 2020 2020 2020 2020 2277  true,.        "w
+00002910: 6562 6175 7468 6e3a 6578 7465 6e73 696f  ebauthn:extensio
+00002920: 6e3a 6372 6564 426c 6f62 223a 2074 7275  n:credBlob": tru
+00002930: 652c 0a20 2020 2020 2020 2022 7765 6261  e,.        "weba
+00002940: 7574 686e 3a65 7874 656e 7369 6f6e 3a6c  uthn:extension:l
+00002950: 6172 6765 426c 6f62 223a 2074 7275 652c  argeBlob": true,
+00002960: 0a20 2020 2020 2020 2022 7765 6261 7574  .        "webaut
+00002970: 686e 3a76 6972 7475 616c 4175 7468 656e  hn:virtualAuthen
+00002980: 7469 6361 746f 7273 223a 2074 7275 650a  ticators": true.
+00002990: 2020 2020 7d0a 7d0a 6060 600a 5468 6520      }.}.```.The 
+000029a0: 2a73 6573 7369 6f6e 4964 2a20 7661 6c75  *sessionId* valu
+000029b0: 6520 6361 6e20 6265 2075 7365 6420 746f  e can be used to
+000029c0: 2070 6572 666f 726d 2066 7572 7468 6572   perform further
+000029d0: 2061 6374 696f 6e73 206c 696b 6520 2a66   actions like *f
+000029e0: 696e 6420 656c 656d 656e 742a 2c20 2a73  ind element*, *s
+000029f0: 656e 6420 6b65 7973 2a20 6f72 202a 636c  end keys* or *cl
+00002a00: 6963 6b2a 2062 7574 746f 6e73 2e20 4d6f  ick* buttons. Mo
+00002a10: 7265 2064 6574 6169 6c73 2063 616e 2062  re details can b
+00002a20: 6520 666f 756e 6420 696e 205b 4a73 6f6e  e found in [Json
+00002a30: 2057 6972 6520 5072 6f74 6f63 6f6c 2053   Wire Protocol S
+00002a40: 7065 6369 6669 6361 7469 6f6e 5d28 6874  pecification](ht
+00002a50: 7470 733a 2f2f 7777 772e 7365 6c65 6e69  tps://www.seleni
+00002a60: 756d 2e64 6576 2f64 6f63 756d 656e 7461  um.dev/documenta
+00002a70: 7469 6f6e 2f6c 6567 6163 792f 6a73 6f6e  tion/legacy/json
+00002a80: 5f77 6972 655f 7072 6f74 6f63 6f6c 2f29  _wire_protocol/)
+00002a90: 2e0a 416c 736f 2077 6974 6820 7468 6520  ..Also with the 
+00002aa0: 2a2d 682a 2070 6172 616d 6574 6572 2069  *-h* parameter i
+00002ab0: 6e20 4472 6976 6572 732c 2066 6f72 2065  n Drivers, for e
+00002ac0: 7861 6d70 6c65 3a20 0a60 6060 0a2e 2f63  xample: .```../c
+00002ad0: 6872 6f6d 6564 7269 7665 7220 2d68 0a0a  hromedriver -h..
+00002ae0: 5573 6167 653a 202e 2f63 6872 6f6d 6564  Usage: ./chromed
+00002af0: 7269 7665 7220 5b4f 5054 494f 4e53 5d0a  river [OPTIONS].
+00002b00: 0a4f 7074 696f 6e73 0a20 202d 2d70 6f72  .Options.  --por
+00002b10: 743d 504f 5254 2020 2020 2020 2020 2020  t=PORT          
+00002b20: 2020 2020 2020 2020 2020 2070 6f72 7420             port 
+00002b30: 746f 206c 6973 7465 6e20 6f6e 0a20 202d  to listen on.  -
+00002b40: 2d61 6462 2d70 6f72 743d 504f 5254 2020  -adb-port=PORT  
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002b60: 6462 2073 6572 7665 7220 706f 7274 0a20  db server port. 
+00002b70: 202d 2d6c 6f67 2d70 6174 683d 4649 4c45   --log-path=FILE
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2077 7269 7465 2073 6572 7665 7220 6c6f   write server lo
+00002ba0: 6720 746f 2066 696c 6520 696e 7374 6561  g to file instea
+00002bb0: 6420 6f66 2073 7464 6572 722c 2069 6e63  d of stderr, inc
+00002bc0: 7265 6173 6573 206c 6f67 206c 6576 656c  reases log level
+00002bd0: 2074 6f20 494e 464f 0a20 202d 2d6c 6f67   to INFO.  --log
+00002be0: 2d6c 6576 656c 3d4c 4556 454c 2020 2020  -level=LEVEL    
+00002bf0: 2020 2020 2020 2020 2020 2073 6574 206c             set l
+00002c00: 6f67 206c 6576 656c 3a20 414c 4c2c 2044  og level: ALL, D
+00002c10: 4542 5547 2c20 494e 464f 2c20 5741 524e  EBUG, INFO, WARN
+00002c20: 494e 472c 2053 4556 4552 452c 204f 4646  ING, SEVERE, OFF
+00002c30: 0a20 202d 2d76 6572 626f 7365 2020 2020  .  --verbose    
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2020 206c 6f67 2076 6572 626f 7365 6c79     log verbosely
+00002c60: 2028 6571 7569 7661 6c65 6e74 2074 6f20   (equivalent to 
+00002c70: 2d2d 6c6f 672d 6c65 7665 6c3d 414c 4c29  --log-level=ALL)
+00002c80: 0a20 202d 2d73 696c 656e 7420 2020 2020  .  --silent     
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ca0: 2020 206c 6f67 206e 6f74 6869 6e67 2028     log nothing (
+00002cb0: 6571 7569 7661 6c65 6e74 2074 6f20 2d2d  equivalent to --
+00002cc0: 6c6f 672d 6c65 7665 6c3d 4f46 4629 0a20  log-level=OFF). 
+00002cd0: 202d 2d61 7070 656e 642d 6c6f 6720 2020   --append-log   
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2061 7070 656e 6420 6c6f 6720 6669 6c65   append log file
+00002d00: 2069 6e73 7465 6164 206f 6620 7265 7772   instead of rewr
+00002d10: 6974 696e 670a 2020 2d2d 7265 706c 6179  iting.  --replay
+00002d20: 6162 6c65 2020 2020 2020 2020 2020 2020  able            
+00002d30: 2020 2020 2020 2020 2865 7870 6572 696d          (experim
+00002d40: 656e 7461 6c29 206c 6f67 2076 6572 626f  ental) log verbo
+00002d50: 7365 6c79 2061 6e64 2064 6f6e 2774 2074  sely and don't t
+00002d60: 7275 6e63 6174 6520 6c6f 6e67 2073 7472  runcate long str
+00002d70: 696e 6773 2073 6f20 7468 6174 2074 6865  ings so that the
+00002d80: 206c 6f67 2063 616e 2062 6520 7265 706c   log can be repl
+00002d90: 6179 6564 2e0a 2020 2d2d 7665 7273 696f  ayed..  --versio
+00002da0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00002db0: 2020 2020 2020 2020 7072 696e 7420 7468          print th
+00002dc0: 6520 7665 7273 696f 6e20 6e75 6d62 6572  e version number
+00002dd0: 2061 6e64 2065 7869 740a 2020 2d2d 7572   and exit.  --ur
+00002de0: 6c2d 6261 7365 2020 2020 2020 2020 2020  l-base          
+00002df0: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00002e00: 2055 524c 2070 6174 6820 7072 6566 6978   URL path prefix
+00002e10: 2066 6f72 2063 6f6d 6d61 6e64 732c 2065   for commands, e
+00002e20: 2e67 2e20 7764 2f75 726c 0a20 202d 2d72  .g. wd/url.  --r
+00002e30: 6561 6461 626c 652d 7469 6d65 7374 616d  eadable-timestam
+00002e40: 7020 2020 2020 2020 2020 2020 2061 6464  p            add
+00002e50: 2072 6561 6461 626c 6520 7469 6d65 7374   readable timest
+00002e60: 616d 7073 2074 6f20 6c6f 670a 2020 2d2d  amps to log.  --
+00002e70: 656e 6162 6c65 2d63 6872 6f6d 652d 6c6f  enable-chrome-lo
+00002e80: 6773 2020 2020 2020 2020 2020 2020 7368  gs            sh
+00002e90: 6f77 206c 6f67 7320 6672 6f6d 2074 6865  ow logs from the
+00002ea0: 2062 726f 7773 6572 2028 6f76 6572 7269   browser (overri
+00002eb0: 6465 7320 6f74 6865 7220 6c6f 6767 696e  des other loggin
+00002ec0: 6720 6f70 7469 6f6e 7329 0a20 202d 2d64  g options).  --d
+00002ed0: 6973 6162 6c65 2d64 6576 2d73 686d 2d75  isable-dev-shm-u
+00002ee0: 7361 6765 2020 2020 2020 2020 2064 6f20  sage         do 
+00002ef0: 6e6f 7420 7573 6520 2f64 6576 2f73 686d  not use /dev/shm
+00002f00: 2028 6164 6420 7468 6973 2073 7769 7463   (add this switc
+00002f10: 6820 6966 2073 6565 696e 6720 6572 726f  h if seeing erro
+00002f20: 7273 2072 656c 6174 6564 2074 6f20 7368  rs related to sh
+00002f30: 6172 6564 206d 656d 6f72 7929 0a20 202d  ared memory).  -
+00002f40: 2d61 6c6c 6f77 6564 2d69 7073 2020 2020  -allowed-ips    
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002f60: 6f6d 6d61 2d73 6570 6172 6174 6564 2061  omma-separated a
+00002f70: 6c6c 6f77 6c69 7374 206f 6620 7265 6d6f  llowlist of remo
+00002f80: 7465 2049 5020 6164 6472 6573 7365 7320  te IP addresses 
+00002f90: 7768 6963 6820 6172 6520 616c 6c6f 7765  which are allowe
+00002fa0: 6420 746f 2063 6f6e 6e65 6374 2074 6f20  d to connect to 
+00002fb0: 4368 726f 6d65 4472 6976 6572 0a60 6060  ChromeDriver.```
+00002fc0: 0a23 2043 6f6e 7472 6962 7574 696e 670a  .# Contributing.
+00002fd0: 5265 6164 2074 6865 205b 436f 6465 206f  Read the [Code o
+00002fe0: 6620 436f 6e64 7563 745d 2868 7474 7073  f Conduct](https
+00002ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
+00003000: 7567 6c61 7364 636d 2f63 6171 7569 2f62  uglasdcm/caqui/b
+00003010: 6c6f 622f 6d61 696e 2f43 4f44 455f 4f46  lob/main/CODE_OF
+00003020: 5f43 4f4e 4455 4354 2e6d 6429 2062 6566  _CONDUCT.md) bef
+00003030: 6f72 6520 7075 7368 206e 6577 204d 6572  ore push new Mer
+00003040: 6765 2052 6571 7565 7374 732e 0a4e 6f77  ge Requests..Now
+00003050: 2c20 666f 6c6c 6f77 2074 6865 2073 7465  , follow the ste
+00003060: 7073 2069 6e20 5b43 6f6e 7472 6962 7574  ps in [Contribut
+00003070: 696e 675d 2868 7474 7073 3a2f 2f67 6974  ing](https://git
+00003080: 6875 622e 636f 6d2f 646f 7567 6c61 7364  hub.com/douglasd
+00003090: 636d 2f63 6171 7569 2f62 6c6f 622f 6d61  cm/caqui/blob/ma
+000030a0: 696e 2f43 4f4e 5452 4942 5554 494e 472e  in/CONTRIBUTING.
+000030b0: 6d64 2920 7365 7373 696f 6e2e 0a         md) session..
```


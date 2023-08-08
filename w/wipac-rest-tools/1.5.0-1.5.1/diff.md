# Comparing `tmp/wipac-rest-tools-1.5.0.tar.gz` & `tmp/wipac-rest-tools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.5.0.tar", last modified: Thu Aug  3 15:25:30 2023, max compression
+gzip compressed data, was "wipac-rest-tools-1.5.1.tar", last modified: Tue Aug  8 16:05:10 2023, max compression
```

## Comparing `wipac-rest-tools-1.5.0.tar` & `wipac-rest-tools-1.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4257 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3238 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.578420 wipac-rest-tools-1.5.0/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2023-08-03 15:25:27.000000 wipac-rest-tools-1.5.0/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.578420 wipac-rest-tools-1.5.0/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      605 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     7380 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     3048 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      697 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8781 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    12754 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    19405 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5335 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4833 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-08-03 15:25:30.586421 wipac-rest-tools-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-08-03 15:25:26.000000 wipac-rest-tools-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 15:25:30.582421 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4257 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      531 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-03 15:25:30.000000 wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-08-08 16:05:08.000000 wipac-rest-tools-1.5.1/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8781 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    12754 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    19405 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-08-08 16:05:10.563795 wipac-rest-tools-1.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-08 16:05:07.000000 wipac-rest-tools-1.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:05:10.559795 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-08-08 16:05:10.000000 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2023-08-08 16:05:10.000000 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 16:05:10.000000 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      531 2023-08-08 16:05:10.000000 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-08 16:05:10.000000 wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.5.0/LICENSE` & `wipac-rest-tools-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/PKG-INFO` & `wipac-rest-tools-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.5.0
+Version: 1.5.1
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.5.0/README.md` & `wipac-rest-tools-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/__init__.py` & `wipac-rest-tools-1.5.1/rest_tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/__init__.py` & `wipac-rest-tools-1.5.1/rest_tools/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/client.py` & `wipac-rest-tools-1.5.1/rest_tools/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,21 +87,21 @@
                 break
         return retries
 
 
 def _log_retries_values(
     retries: int, timeout: float, backoff_factor: float, logger: logging.Logger
 ) -> None:
-    logger.info(f"using {retries=} {timeout=} {backoff_factor=}")
+    logger.debug(f"using {retries=} {timeout=} {backoff_factor=}")
     if retries:
         retries_schema = ' '.join(
             [f'<0.0s> {timeout}s']
             + [f'<{(backoff_factor * 2**i)}s> {timeout}s' for i in range(1, retries)]
         )
-        logger.info(
+        logger.debug(
             f"retry scheme (TIMEOUT [<BACKOFF> TIMEOUT ...]): "
             f"{timeout}s {retries_schema}"
         )
 
 
 class RestClient:
     """A REST client with token handling.
```

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.5.1/rest_tools/client/client_credentials.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/device_client.py` & `wipac-rest-tools-1.5.1/rest_tools/client/device_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.5.1/rest_tools/client/openid_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/client/session.py` & `wipac-rest-tools-1.5.1/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/__init__.py` & `wipac-rest-tools-1.5.1/rest_tools/server/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.5.1/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/decorators.py` & `wipac-rest-tools-1.5.1/rest_tools/server/decorators.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/handler.py` & `wipac-rest-tools-1.5.1/rest_tools/server/handler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/server.py` & `wipac-rest-tools-1.5.1/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/server/stats.py` & `wipac-rest-tools-1.5.1/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/telemetry.py` & `wipac-rest-tools-1.5.1/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/utils/auth.py` & `wipac-rest-tools-1.5.1/rest_tools/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
             # get keys
             r = requests.get(self.provider_info['jwks_uri'])
             r.raise_for_status()
             for jwk in r.json()['keys']:
                 logging.debug(f'jwk: {jwk}')
                 kid = jwk['kid']
-                logging.info(f'loaded JWT key {kid}')
+                logging.debug(f'loaded JWT key {kid}')
                 self.public_keys[kid] = jwt.algorithms.RSAAlgorithm.from_jwk(json.dumps(jwk))
         except Exception:
             logging.warning('failed to refresh OpenID keys', exc_info=True)
 
     def validate(self, token, **kwargs):
         """
         Validate a token.
```

### Comparing `wipac-rest-tools-1.5.0/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.5.1/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.5.1/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/setup.cfg` & `wipac-rest-tools-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.5.0
+Version: 1.5.1
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.5.0/wipac_rest_tools.egg-info/requires.txt` & `wipac-rest-tools-1.5.1/wipac_rest_tools.egg-info/requires.txt`

 * *Files identical despite different names*


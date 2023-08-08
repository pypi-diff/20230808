# Comparing `tmp/binance-futures-connector-4.0.0rc2.tar.gz` & `tmp/binance-futures-connector-4.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-futures-connector-4.0.0rc2.tar", last modified: Fri May 26 06:01:38 2023, max compression
+gzip compressed data, was "binance-futures-connector-4.0.0rc3.tar", last modified: Mon Jul  3 01:51:28 2023, max compression
```

## Comparing `binance-futures-connector-4.0.0rc2.tar` & `binance-futures-connector-4.0.0rc3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31509 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/portfolio_margin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.964544 binance-futures-connector-4.0.0rc3/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/cm_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/cm_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/cm_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/cm_futures/portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/um_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/um_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/um_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/um_futures/portfolio_margin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/websocket/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/cm_futures/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance/websocket/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/um_futures/websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-03 01:51:28.000000 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 01:51:28.000000 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:51:28.000000 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 01:51:28.000000 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 01:51:28.000000 binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 01:51:28.968544 binance-futures-connector-4.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-03 01:51:21.000000 binance-futures-connector-4.0.0rc3/setup.py
```

### Comparing `binance-futures-connector-4.0.0rc2/LICENSE.md` & `binance-futures-connector-4.0.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/PKG-INFO` & `binance-futures-connector-4.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-futures-connector
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/binance/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-futures-connector-4.0.0rc2/README.md` & `binance-futures-connector-4.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/api.py` & `binance-futures-connector-4.0.0rc3/binance/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.proxies = None
         self.private_key = private_key
         self.private_key_pass = private_key_passphrase
         self.session = requests.Session()
         self.session.headers.update(
             {
                 "Content-Type": "application/json;charset=utf-8",
-                "User-Agent": "binance-connector/" + __version__,
+                "User-Agent": "binance-futures-connector-python/" + __version__,
                 "X-MBX-APIKEY": key,
             }
         )
 
         if base_url:
             self.base_url = base_url
```

### Comparing `binance-futures-connector-4.0.0rc2/binance/cm_futures/__init__.py` & `binance-futures-connector-4.0.0rc3/binance/cm_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/cm_futures/account.py` & `binance-futures-connector-4.0.0rc3/binance/cm_futures/account.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/cm_futures/data_stream.py` & `binance-futures-connector-4.0.0rc3/binance/cm_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/cm_futures/market.py` & `binance-futures-connector-4.0.0rc3/binance/cm_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/error.py` & `binance-futures-connector-4.0.0rc3/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/lib/authentication.py` & `binance-futures-connector-4.0.0rc3/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/lib/utils.py` & `binance-futures-connector-4.0.0rc3/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/um_futures/__init__.py` & `binance-futures-connector-4.0.0rc3/binance/um_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/um_futures/account.py` & `binance-futures-connector-4.0.0rc3/binance/um_futures/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,22 +191,24 @@
         )
     elif orderId:
         params = {
             "symbol": symbol,
             "side": side,
             "quantity": quantity,
             "orderId": orderId,
+            "price": price,
             **kwargs,
         }
     else:
         params = {
             "symbol": symbol,
             "side": side,
             "quantity": quantity,
             "origClientOrderId": origClientOrderId,
+            "price": price,
             **kwargs,
         }
 
     url_path = "/fapi/v1/order"
     return self.sign_request("PUT", url_path, params)
```

### Comparing `binance-futures-connector-4.0.0rc2/binance/um_futures/data_stream.py` & `binance-futures-connector-4.0.0rc3/binance/um_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/um_futures/market.py` & `binance-futures-connector-4.0.0rc3/binance/um_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/websocket/binance_socket_manager.py` & `binance-futures-connector-4.0.0rc3/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/websocket_client.py` & `binance-futures-connector-4.0.0rc3/binance/websocket/cm_futures/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/websocket_client.py` & `binance-futures-connector-4.0.0rc3/binance/websocket/um_futures/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance/websocket/websocket_client.py` & `binance-futures-connector-4.0.0rc3/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/PKG-INFO` & `binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-futures-connector
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/binance/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/SOURCES.txt` & `binance-futures-connector-4.0.0rc3/binance_futures_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc2/setup.py` & `binance-futures-connector-4.0.0rc3/setup.py`

 * *Files identical despite different names*


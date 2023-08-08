# Comparing `tmp/volstreet-1.2.0.tar.gz` & `tmp/volstreet-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-1.2.0.tar", last modified: Mon Aug  7 09:13:26 2023, max compression
+gzip compressed data, was "volstreet-1.2.1.tar", last modified: Mon Aug  7 14:48:17 2023, max compression
```

## Comparing `volstreet-1.2.0.tar` & `volstreet-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.811662 volstreet-1.2.0/
--rw-rw-rw-   0        0        0      497 2023-08-07 09:13:26.811662 volstreet-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.2.0/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1391 2023-08-07 09:13:26.812659 volstreet-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.806675 volstreet-1.2.0/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.2.0/volstreet/__init__.py
--rw-rw-rw-   0        0        0    10080 2023-08-06 14:57:40.000000 volstreet-1.2.0/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2716 2023-08-03 18:56:13.000000 volstreet-1.2.0/volstreet/constants.py
--rw-rw-rw-   0        0        0    43826 2023-07-28 13:59:59.000000 volstreet-1.2.0/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   203180 2023-08-07 09:12:22.000000 volstreet-1.2.0/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      729 2023-08-02 13:31:19.000000 volstreet-1.2.0/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.2.0/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14632 2023-08-06 16:51:52.000000 volstreet-1.2.0/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-08-07 09:13:26.811662 volstreet-1.2.0/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      801 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-07 09:13:26.000000 volstreet-1.2.0/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 14:48:17.911559 volstreet-1.2.1/
+-rw-rw-rw-   0        0        0      497 2023-08-07 14:48:17.912897 volstreet-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-1.2.1/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1391 2023-08-07 14:48:17.912897 volstreet-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 14:48:17.906933 volstreet-1.2.1/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-1.2.1/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-1.2.1/volstreet/__init__.py
+-rw-rw-rw-   0        0        0    10080 2023-08-06 14:57:40.000000 volstreet-1.2.1/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2716 2023-08-03 18:56:13.000000 volstreet-1.2.1/volstreet/constants.py
+-rw-rw-rw-   0        0        0    43826 2023-07-28 13:59:59.000000 volstreet-1.2.1/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   203503 2023-08-07 14:45:36.000000 volstreet-1.2.1/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-1.2.1/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      729 2023-08-02 13:31:19.000000 volstreet-1.2.1/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-1.2.1/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14632 2023-08-06 16:51:52.000000 volstreet-1.2.1/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-08-07 14:48:17.911559 volstreet-1.2.1/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-08-07 14:48:17.000000 volstreet-1.2.1/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-08-07 14:48:17.000000 volstreet-1.2.1/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 14:48:17.000000 volstreet-1.2.1/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      801 2023-08-07 14:48:17.000000 volstreet-1.2.1/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 14:48:17.000000 volstreet-1.2.1/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-1.2.0/setup.cfg` & `volstreet-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 312e 322e 300d 0a61  rsion = 1.2.0..a
+00000020: 7273 696f 6e20 3d20 312e 322e 310d 0a61  rsion = 1.2.1..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
@@ -68,15 +68,15 @@
 00000430: 713d 3d32 352e 302e 300d 0a09 7265 7175  q==25.0.0...requ
 00000440: 6573 7473 3d3d 322e 3238 2e32 0d0a 0973  ests==2.28.2...s
 00000450: 6369 6b69 742d 6c65 6172 6e3d 3d31 2e32  cikit-learn==1.2
 00000460: 2e32 0d0a 0973 6369 7079 3d3d 312e 3130  .2...scipy==1.10
 00000470: 2e31 0d0a 0973 656c 656e 6975 6d3d 3d34  .1...selenium==4
 00000480: 2e31 302e 300d 0a09 7369 783d 3d31 2e31  .10.0...six==1.1
 00000490: 362e 300d 0a09 736d 6172 7461 7069 2d70  6.0...smartapi-p
-000004a0: 7974 686f 6e3d 3d31 2e33 2e30 0d0a 0973  ython==1.3.0...s
+000004a0: 7974 686f 6e3d 3d31 2e33 2e35 0d0a 0973  ython==1.3.5...s
 000004b0: 7461 636b 2d64 6174 613d 3d30 2e36 2e32  tack-data==0.6.2
 000004c0: 0d0a 0974 6f72 6e61 646f 3d3d 362e 320d  ...tornado==6.2.
 000004d0: 0a09 7472 6169 746c 6574 733d 3d35 2e38  ..traitlets==5.8
 000004e0: 2e31 0d0a 0975 726c 6c69 6233 3d3d 312e  .1...urllib3==1.
 000004f0: 3236 2e31 340d 0a09 7763 7769 6474 683d  26.14...wcwidth=
 00000500: 3d30 2e32 2e36 0d0a 0977 6562 736f 636b  =0.2.6...websock
 00000510: 6574 2d63 6c69 656e 743d 3d31 2e35 2e31  et-client==1.5.1
```

### Comparing `volstreet-1.2.0/volstreet/SmartWebSocketV2.py` & `volstreet-1.2.1/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/blackscholes.py` & `volstreet-1.2.1/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/constants.py` & `volstreet-1.2.1/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/datamodule.py` & `volstreet-1.2.1/volstreet/datamodule.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/dealingroom.py` & `volstreet-1.2.1/volstreet/dealingroom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pandas as pd
 import numpy as np
 from datetime import datetime, time, timedelta, timezone
 from time import sleep
 import requests
 import json
-from smartapi import SmartConnect
-from smartapi.smartExceptions import DataException
+from SmartApi import SmartConnect
+from SmartApi.smartExceptions import DataException
 import pyotp
 from threading import Thread
-from volstreet.SmartWebSocketV2 import SmartWebSocketV2
+from SmartApi.smartWebSocketV2 import SmartWebSocketV2
 from volstreet.constants import scrips, holidays, symbol_df, logger
 from volstreet import blackscholes as bs, datamodule as dm
 from volstreet.exceptions import OptionModelInputError
 from collections import defaultdict, deque
 import yfinance as yf
 from fuzzywuzzy import process
 import re
@@ -84,29 +84,36 @@
         self.last_update_time = None
         self.iv_log = defaultdict(lambda: defaultdict(dict))
         self.webhook_url = webhook_url
         self.index_option_chains_subscribed = []
         self.correlation_id = correlation_id
         self.finnifty_index = Index("FINNIFTY")  # Finnifty temp fix
 
-    def start_websocket(self):
+    def start_websocket(self, tokens=None, mode=None, exchange_type=None):
+        def _subscribe_tokens():
+            self.subscribe_tokens(tokens, mode, exchange_type)
+
         def on_open(wsapp):
-            self.subscribe_tokens()
+            _subscribe_tokens()
 
         # Assign the callbacks.
         self.on_open = on_open
         self.on_data = self.on_data_handler
         self.on_error = lambda wsapp, error: print(error)
         self.on_close = lambda wsapp: print("Close")
         Thread(target=self.connect).start()
 
-    def subscribe_tokens(self):
-        tokens = ["26000", "26009"]
-        mode = 1
-        token_list = [{"exchangeType": 1, "tokens": tokens}]
+    def subscribe_tokens(self, tokens=None, mode=None, exchange_type=None):
+        if tokens is None:
+            tokens = ["26000", "26009"]
+        if mode is None:
+            mode = 1
+        if exchange_type is None:
+            exchange_type = 1
+        token_list = [{"exchangeType": exchange_type, "tokens": tokens}]
         self.subscribe(self.correlation_id, mode, token_list)
 
     def on_data_handler(self, wsapp, message):
         self.price_dict[message["token"]] = {
             "ltp": message["last_traded_price"] / 100,
             "best_bid": message["best_5_sell_data"][0]["price"] / 100
             if "best_5_sell_data" in message
```

### Comparing `volstreet-1.2.0/volstreet/discord_bot.py` & `volstreet-1.2.1/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/exceptions.py` & `volstreet-1.2.1/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/nsefunctions.py` & `volstreet-1.2.1/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet/strategies.py` & `volstreet-1.2.1/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-1.2.0/volstreet.egg-info/requires.txt` & `volstreet-1.2.1/volstreet.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 pywin32==305
 pyzmq==25.0.0
 requests==2.28.2
 scikit-learn==1.2.2
 scipy==1.10.1
 selenium==4.10.0
 six==1.16.0
-smartapi-python==1.3.0
+smartapi-python==1.3.5
 stack-data==0.6.2
 tornado==6.2
 traitlets==5.8.1
 urllib3==1.26.14
 wcwidth==0.2.6
 websocket-client==1.5.1
 xlrd==2.0.1
```


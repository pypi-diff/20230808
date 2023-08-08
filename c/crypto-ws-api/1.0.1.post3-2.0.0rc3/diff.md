# Comparing `tmp/crypto-ws-api-1.0.1.post3.tar.gz` & `tmp/crypto-ws-api-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-ws-api-1.0.1.post3.tar", last modified: Mon Jul 17 18:53:55 2023, max compression
+gzip compressed data, was "crypto-ws-api-2.0.0rc3.tar", last modified: Tue Aug  8 16:55:04 2023, max compression
```

## Comparing `crypto-ws-api-1.0.1.post3.tar` & `crypto-ws-api-2.0.0rc3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-1.0.1.post3/.deepsource.toml
--rwxr-xr-x   0        0        0      373 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-1.0.1.post3/LICENSE.md
--rw-r--r--   0        0        0     5768 2023-07-05 15:44:42.509478 crypto-ws-api-1.0.1.post3/README.md
--rw-r--r--   0        0        0     1303 2023-07-17 18:34:11.883696 crypto-ws-api-1.0.1.post3/crypto_ws_api/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/crypto_ws_api/demo.py
--rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_api.toml.template
--rw-r--r--   0        0        0    10528 2023-07-17 18:01:30.262695 crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_session.py
--rw-r--r--   0        0        0      993 2023-07-17 18:34:11.879713 crypto-ws-api-1.0.1.post3/pyproject.toml
--rw-r--r--   0        0        0       83 2023-07-17 18:34:11.891662 crypto-ws-api-1.0.1.post3/requirements.txt
--rw-r--r--   0        0        0     6517 1970-01-01 00:00:00.000000 crypto-ws-api-1.0.1.post3/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-2.0.0rc3/.deepsource.toml
+-rwxr-xr-x   0        0        0      801 2023-08-08 16:18:12.394084 crypto-ws-api-2.0.0rc3/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-2.0.0rc3/LICENSE.md
+-rw-r--r--   0        0        0     7225 2023-08-08 16:17:50.942419 crypto-ws-api-2.0.0rc3/README.md
+-rw-r--r--   0        0        0     1412 2023-08-08 16:51:43.212671 crypto-ws-api-2.0.0rc3/crypto_ws_api/__init__.py
+-rw-r--r--   0        0        0     4558 2023-08-08 16:51:43.208671 crypto-ws-api-2.0.0rc3/crypto_ws_api/demo.py
+-rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-2.0.0rc3/crypto_ws_api/ws_api.toml.template
+-rw-r--r--   0        0        0    16526 2023-08-08 16:38:16.331913 crypto-ws-api-2.0.0rc3/crypto_ws_api/ws_session.py
+-rw-r--r--   0        0        0      969 2023-08-08 16:18:12.590081 crypto-ws-api-2.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-08-08 16:18:13.338069 crypto-ws-api-2.0.0rc3/requirements.txt
+-rw-r--r--   0        0        0     7939 1970-01-01 00:00:00.000000 crypto-ws-api-2.0.0rc3/PKG-INFO
```

### Comparing `crypto-ws-api-1.0.1.post3/LICENSE.md` & `crypto-ws-api-2.0.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.1.post3/README.md` & `crypto-ws-api-2.0.0rc3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,68 @@
+Metadata-Version: 2.1
+Name: crypto-ws-api
+Version: 2.0.0rc3
+Summary: Crypto WS API connector for ASYNC requests
+Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Requires-Dist: aiohttp==3.8.5
+Requires-Dist: shortuuid~=1.0.11
+Requires-Dist: platformdirs~=3.10.0
+Requires-Dist: toml~=0.10.2
+Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-api
+
 <h1 align="center"><img align="center" src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="75">Crypto WS API connector for ASYNC requests</h1>
 
 <h2 align="center">Full coverage of all methods provided by the interface</h2>
 
 <h3 align="center">Provides of connection management, keepalive and rate limits control</h3>
 
 ***
 <a href="https://pypi.org/project/crypto-ws-api/"><img src="https://img.shields.io/pypi/v/crypto-ws-api" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/crypto-ws-api/maintainability"><img src="https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/maintainability" /></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=resolved+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=active+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_crypto-ws-api" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_crypto-ws-api&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/crypto-ws-api" target="_blank"><img alt="Downloads" title="Downloads" src="https://static.pepy.tech/badge/crypto-ws-api"/></a>
 ***
-For :heavy_check_mark:Binance, 
+For :heavy_check_mark:Binance, :heavy_check_mark:OKX, :heavy_check_mark:Bitfinex
 ***
 
 ## Features
-Lightweight and efficient solution to utilize of all available methods provided through the:
+Lightweight and efficient solution to utilize of all available methods** provided through the:
 * [Binance Websocket API v3](https://developers.binance.com/docs/binance-trading-api/websocket_api)
+* [OKX Websocket API v5](https://www.okx.com/docs-v5/en/#overview-websocket)
+* [Bitfinex Websocket Inputs](https://docs.bitfinex.com/reference/ws-auth-input)
+
+** Not for channel by one-way subscription, for **_request <-> response_** mode only
 
 ### Session management layer for:
 - Credentials
 - Connection
 - Keepalive
 - Error handling
 - Limits control
 - Methods construction
-  + Generating session request id by default
   + Creating request on-the-fly from method name and params: {}
   + Generating signature if necessary
   + Response handling
 - logging
 
 ### User interface layer
 - Start session instance
-- Getting session operational status
 - Send async request
 - Get response or raised exception
+- Reuse instance for different type requests
 - Stop session instance
 
 ## Get started
 ### Install use PIP
 
 ```console
 pip install crypto_ws_api
@@ -62,14 +84,20 @@
 > 
 >Can't find config file! Creating it...
 > 
 >Before first run set account(s) API key into /home/ubuntu/.config/crypto_ws_api/ws_api.toml
 
 ### Prepare exchange account
 * For test purpose log in at [Binance Spot Test Network](https://testnet.binance.vision/)
+
+For OKX and Bitfinex, unlike Binance, a limited number of methods are implemented at the WS API level,
+such as creating, modifying, and deleting orders.
+There are no public get-time (), ping-pong, etc., so this demo script is limited to calling Binance
+to demonstrate capabilities.
+
 * Create API Key
 * After install and create environment specify api_key and api_secret to the config file
 
 ### Start demo
 * Run in terminal window
 ```
 crypto_ws_api_demo
@@ -78,61 +106,99 @@
 ## Useful tips
 
 _*`crypto_ws_api/demo.py` - complete and fully functional example*_
 
 ### Get credentials and create user session
 
 ```bazaar
-from crypto_ws_api.ws_session import get_credentials, UserWSSession
+from crypto_ws_api.ws_session import UserWSSession
 
-# Can be omitted if you have credentials
-_exchange, _test_net, api_key, api_secret, ws_api_endpoint = get_credentials(account_name)
+# Get credentials and create user session
+# Can be omitted if you have credentials from other source
+exchange, _test_net, api_key, api_secret, passphrase, ws_api_endpoint = get_credentials(account_name)
 
 session = aiohttp.ClientSession()
 
+trade_id = shortuuid.uuid()
+
 user_session = UserWSSession(
+    session,
+    exchange,
+    ws_api_endpoint,
     api_key,
     api_secret,
-    session=session,
-    endpoint=ws_api_endpoint
+    passphrase
 )
-
-await user_session.start()
-print(f"Operational status: {user_session.operational_status}")
-```
-### Demo method's calling
-```bazaar
-await account_information(user_session)
-```
-
-### Stop user session and close aiohttp session
-```bazaar
-await user_session.stop()
-await session.close()
-print(f"Operational status: {user_session.operational_status}")
 ```
 
-### Method call example
+### Method example
 ```bazaar
-async def account_information(user_session: UserWSSession):
+async def account_information(user_session: UserWSSession, _trade_id):
     # https://developers.binance.com/docs/binance-trading-api/websocket_api#account-information-user_data
     try:
         res = await user_session.handle_request(
+            _trade_id,
             "account.status",
-            api_key=True,
-            signed=True
+            _api_key=True,
+            _signed=True
         )
         if res is None:
-            print("Here handling state Out-of-Service")
+            logger.warning("Here handling state Out-of-Service")
     except asyncio.CancelledError:
         pass  # Task cancellation should not be logged as an error
     except Exception as _ex:
-        print(f"Handling exception: {_ex}")
+        logger.error(f"Handling exception: {_ex}")
     else:
-        print(f"Account information (USER_DATA) response: {res}")
+        logger.info(f"Account information (USER_DATA) response: {res}")
+```
+
+### Demo method's calling
+```bazaar
+await account_information(user_session, trade_id)
+```
+
+### Stop user session and close aiohttp session
+```bazaar
+await user_session.stop()
+await session.close()
+```
+
+### Create limit order example
+```bazaar
+if self.exchange == 'binance':
+    params = {
+        "symbol": "BTCUSDT",
+        "side": "SELL",
+        "type": "LIMIT",
+        "timeInForce": "GTC",
+        "price": "23416.10000000",
+        "quantity": "0.00847000",
+    }
+    binance_res = await user_session.handle_request(trade_id, "order.place", params, _api_key=True, _signed=True)
+
+elif self.exchange == 'bitfinex':
+    params = {
+        "type": "EXCHANGE LIMIT",
+        "symbol": "tBTCUSDT",
+        "price": "23416.10000000",
+        "amount": ('' if side == 'BUY' else '-') + "0.00847000",
+    }
+    bitfnex_res = await user_session.handle_request(trade_id, "on", params)
+
+elif self.exchange == 'okx':
+    params = {
+        "instId": "BTC-USDT",
+        "tdMode": "cash",
+        "clOrdId": "client_order_id",
+        "side": "buy",
+        "ordType": "limit",
+        "sz": "0.00847000",
+        "px": "23416.10000000",
+    }
+    okx_res = await user_session.handle_request(trade_id, "order", params)
 ```
 
 ### Logging setup
 For configure logging in multi-module project use next snippet for yours `main()`:
 ```bazaar
 import logging.handlers
 
@@ -145,18 +211,17 @@
 #
 root_logger = logging.getLogger()
 root_logger.setLevel(logging.DEBUG)
 root_logger.addHandler(sh)
 ```
 
 ## [Limits control](https://developers.binance.com/docs/binance-trading-api/websocket_api#general-information-on-rate-limits) :link:
-Upon reaching the limit threshold of each type, the session switches to the Out-of-Service state. Monitor the values
-of the variables `user_session.operational_status` and `user_session.order_handling`
-
+Upon reaching the limit threshold of each type, the session switches to the Out-of-Service state.
 If you send a request in this state, the answer will be `None`
 
 *In any case, you are protected from exceeding limits and blocking for this reason*
 
 ## Donate
 *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
 
 *USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
+
```

#### html2text {}

```diff
@@ -1,60 +1,87 @@
+Metadata-Version: 2.1 Name: crypto-ws-api Version: 2.0.0rc3 Summary: Crypto WS
+API connector for ASYNC requests Author-email: Jerry Fedorenko
+fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Classifier: Programming Language :: Python :: 3 Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: MIT License Classifier: Operating System :: Unix Classifier: Operating
+System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
+Dist: aiohttp==3.8.5 Requires-Dist: shortuuid~=1.0.11 Requires-Dist:
+platformdirs~=3.10.0 Requires-Dist: toml~=0.10.2 Project-URL: Source, https://
+github.com/DogsTailFarmer/crypto-ws-api
 ****** [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-
   a930-4467-a0cd-21627a6a41ed.svg]Crypto WS API connector for ASYNC requests
                                     ******
       ***** Full coverage of all methods provided by the interface *****
 **** Provides of connection management, keepalive and rate limits control ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** For :
-heavy_check_mark:Binance, *** ## Features Lightweight and efficient solution to
-utilize of all available methods provided through the: * [Binance Websocket API
-v3](https://developers.binance.com/docs/binance-trading-api/websocket_api) ###
+heavy_check_mark:Binance, :heavy_check_mark:OKX, :heavy_check_mark:Bitfinex ***
+## Features Lightweight and efficient solution to utilize of all available
+methods** provided through the: * [Binance Websocket API v3](https://
+developers.binance.com/docs/binance-trading-api/websocket_api) * [OKX Websocket
+API v5](https://www.okx.com/docs-v5/en/#overview-websocket) * [Bitfinex
+Websocket Inputs](https://docs.bitfinex.com/reference/ws-auth-input) ** Not for
+channel by one-way subscription, for **_request <-> response_** mode only ###
 Session management layer for: - Credentials - Connection - Keepalive - Error
-handling - Limits control - Methods construction + Generating session request
-id by default + Creating request on-the-fly from method name and params: {} +
-Generating signature if necessary + Response handling - logging ### User
-interface layer - Start session instance - Getting session operational status -
-Send async request - Get response or raised exception - Stop session instance
-## Get started ### Install use PIP ```console pip install crypto_ws_api ``` For
-upgrade to latest versions use: ```console pip install -U crypto_ws_api ```
-After first install create environment by run ```console crypto_ws_api_init ```
-in terminal window. The config directory will be created. You get path to
-config: >ubuntu@ubuntu:~$ crypto_ws_api_init > >Can't find config file!
-Creating it... > >Before first run set account(s) API key into /home/
-ubuntu/.config/crypto_ws_api/ws_api.toml ### Prepare exchange account * For
-test purpose log in at [Binance Spot Test Network](https://
-testnet.binance.vision/) * Create API Key * After install and create
+handling - Limits control - Methods construction + Creating request on-the-fly
+from method name and params: {} + Generating signature if necessary + Response
+handling - logging ### User interface layer - Start session instance - Send
+async request - Get response or raised exception - Reuse instance for different
+type requests - Stop session instance ## Get started ### Install use PIP
+```console pip install crypto_ws_api ``` For upgrade to latest versions use:
+```console pip install -U crypto_ws_api ``` After first install create
+environment by run ```console crypto_ws_api_init ``` in terminal window. The
+config directory will be created. You get path to config: >ubuntu@ubuntu:~$
+crypto_ws_api_init > >Can't find config file! Creating it... > >Before first
+run set account(s) API key into /home/ubuntu/.config/crypto_ws_api/ws_api.toml
+### Prepare exchange account * For test purpose log in at [Binance Spot Test
+Network](https://testnet.binance.vision/) For OKX and Bitfinex, unlike Binance,
+a limited number of methods are implemented at the WS API level, such as
+creating, modifying, and deleting orders. There are no public get-time (),
+ping-pong, etc., so this demo script is limited to calling Binance to
+demonstrate capabilities. * Create API Key * After install and create
 environment specify api_key and api_secret to the config file ### Start demo *
 Run in terminal window ``` crypto_ws_api_demo ``` ## Useful tips
 _*`crypto_ws_api/demo.py` - complete and fully functional example*_ ### Get
 credentials and create user session ```bazaar from crypto_ws_api.ws_session
-import get_credentials, UserWSSession # Can be omitted if you have credentials
-_exchange, _test_net, api_key, api_secret, ws_api_endpoint = get_credentials
-(account_name) session = aiohttp.ClientSession() user_session = UserWSSession
-( api_key, api_secret, session=session, endpoint=ws_api_endpoint ) await
-user_session.start() print(f"Operational status:
-{user_session.operational_status}") ``` ### Demo method's calling ```bazaar
-await account_information(user_session) ``` ### Stop user session and close
-aiohttp session ```bazaar await user_session.stop() await session.close() print
-(f"Operational status: {user_session.operational_status}") ``` ### Method call
-example ```bazaar async def account_information(user_session: UserWSSession): #
-https://developers.binance.com/docs/binance-trading-api/websocket_api#account-
-information-user_data try: res = await user_session.handle_request
-( "account.status", api_key=True, signed=True ) if res is None: print("Here
-handling state Out-of-Service") except asyncio.CancelledError: pass # Task
-cancellation should not be logged as an error except Exception as _ex: print
-(f"Handling exception: {_ex}") else: print(f"Account information (USER_DATA)
-response: {res}") ``` ### Logging setup For configure logging in multi-module
+import UserWSSession # Get credentials and create user session # Can be omitted
+if you have credentials from other source exchange, _test_net, api_key,
+api_secret, passphrase, ws_api_endpoint = get_credentials(account_name) session
+= aiohttp.ClientSession() trade_id = shortuuid.uuid() user_session =
+UserWSSession( session, exchange, ws_api_endpoint, api_key, api_secret,
+passphrase ) ``` ### Method example ```bazaar async def account_information
+(user_session: UserWSSession, _trade_id): # https://developers.binance.com/
+docs/binance-trading-api/websocket_api#account-information-user_data try: res =
+await user_session.handle_request( _trade_id, "account.status", _api_key=True,
+_signed=True ) if res is None: logger.warning("Here handling state Out-of-
+Service") except asyncio.CancelledError: pass # Task cancellation should not be
+logged as an error except Exception as _ex: logger.error(f"Handling exception:
+{_ex}") else: logger.info(f"Account information (USER_DATA) response: {res}")
+``` ### Demo method's calling ```bazaar await account_information(user_session,
+trade_id) ``` ### Stop user session and close aiohttp session ```bazaar await
+user_session.stop() await session.close() ``` ### Create limit order example
+```bazaar if self.exchange == 'binance': params = { "symbol": "BTCUSDT",
+"side": "SELL", "type": "LIMIT", "timeInForce": "GTC", "price":
+"23416.10000000", "quantity": "0.00847000", } binance_res = await
+user_session.handle_request(trade_id, "order.place", params, _api_key=True,
+_signed=True) elif self.exchange == 'bitfinex': params = { "type": "EXCHANGE
+LIMIT", "symbol": "tBTCUSDT", "price": "23416.10000000", "amount": ('' if side
+== 'BUY' else '-') + "0.00847000", } bitfnex_res = await
+user_session.handle_request(trade_id, "on", params) elif self.exchange ==
+'okx': params = { "instId": "BTC-USDT", "tdMode": "cash", "clOrdId":
+"client_order_id", "side": "buy", "ordType": "limit", "sz": "0.00847000", "px":
+"23416.10000000", } okx_res = await user_session.handle_request(trade_id,
+"order", params) ``` ### Logging setup For configure logging in multi-module
 project use next snippet for yours `main()`: ```bazaar import logging.handlers
 logger = logging.getLogger(__name__) formatter = logging.Formatter(fmt="[%
 (asctime)s: %(levelname)s] %(message)s") # sh = logging.StreamHandler()
 sh.setFormatter(formatter) sh.setLevel(logging.DEBUG) # root_logger =
 logging.getLogger() root_logger.setLevel(logging.DEBUG) root_logger.addHandler
 (sh) ``` ## [Limits control](https://developers.binance.com/docs/binance-
 trading-api/websocket_api#general-information-on-rate-limits) :link: Upon
 reaching the limit threshold of each type, the session switches to the Out-of-
-Service state. Monitor the values of the variables
-`user_session.operational_status` and `user_session.order_handling` If you send
-a request in this state, the answer will be `None` *In any case, you are
-protected from exceeding limits and blocking for this reason* ## Donate *BNB*,
-*BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT*
-(TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
+Service state. If you send a request in this state, the answer will be `None`
+*In any case, you are protected from exceeding limits and blocking for this
+reason* ## Donate *BNB*, *BUSD*, *USDT* (BEP20)
+0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
```

### Comparing `crypto-ws-api-1.0.1.post3/crypto_ws_api/__init__.py` & `crypto-ws-api-2.0.0rc3/crypto_ws_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Crypto WS API connector for ASYNC requests
 https://developers.binance.com/docs/binance-trading-api/websocket_api#general-api-information
 Provides methods of connection management, keepalive and rate limits control
 Full coverage of all methods provided by the interface
-For crypto exchanges: +Binance, -OKX, -Bitfinex,
+For crypto exchanges: Binance, OKX, Bitfinex,
 """
 __authors__ = ["Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.0.1-3"
+__version__ = "2.0.0rc3"
 
 from pathlib import Path
 import shutil
 from platformdirs import user_config_path
 
 
-TIMEOUT = 10  # sec timeout for WSS receive
+TIMEOUT = 5  # sec timeout for WSS receive
+# Maximum str size for unique query ID
+ID_LEN_LIMIT = {
+    "binance": 36,
+    "okx": 32,
+    "bitfinex": 32,
+}
 
 CONFIG_PATH = user_config_path("crypto_ws_api")
 CONFIG_FILE = Path(CONFIG_PATH, "ws_api.toml")
 
 
 def init():
     if CONFIG_FILE.exists():
```

### Comparing `crypto-ws-api-1.0.1.post3/crypto_ws_api/ws_api.toml.template` & `crypto-ws-api-2.0.0rc3/crypto_ws_api/ws_api.toml.template`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-1.0.1.post3/pyproject.toml` & `crypto-ws-api-2.0.0rc3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,17 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper",
-    "aiohttp==3.8.4",
+    "aiohttp==3.8.5",
     "shortuuid~=1.0.11",
-    "platformdirs~=3.8.0",
+    "platformdirs~=3.10.0",
     "toml~=0.10.2",
 ]
 
 [tool.flit.module]
 name = "crypto_ws_api"
 
 [project.urls]
```

### Comparing `crypto-ws-api-1.0.1.post3/PKG-INFO` & `crypto-ws-api-2.0.0rc3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,49 @@
-Metadata-Version: 2.1
-Name: crypto-ws-api
-Version: 1.0.1.post3
-Summary: Crypto WS API connector for ASYNC requests
-Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper
-Requires-Dist: aiohttp==3.8.4
-Requires-Dist: shortuuid~=1.0.11
-Requires-Dist: platformdirs~=3.8.0
-Requires-Dist: toml~=0.10.2
-Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-api
-
 <h1 align="center"><img align="center" src="https://user-images.githubusercontent.com/77513676/250364389-cbedc171-a930-4467-a0cd-21627a6a41ed.svg" width="75">Crypto WS API connector for ASYNC requests</h1>
 
 <h2 align="center">Full coverage of all methods provided by the interface</h2>
 
 <h3 align="center">Provides of connection management, keepalive and rate limits control</h3>
 
 ***
 <a href="https://pypi.org/project/crypto-ws-api/"><img src="https://img.shields.io/pypi/v/crypto-ws-api" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/crypto-ws-api/maintainability"><img src="https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/maintainability" /></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=resolved+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://app.deepsource.com/gh/DogsTailFarmer/crypto-ws-api.svg/?label=active+issues&token=TXghPzbi0YWhkCLU8Q1tmDyQ"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_crypto-ws-api" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_crypto-ws-api&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/crypto-ws-api" target="_blank"><img alt="Downloads" title="Downloads" src="https://static.pepy.tech/badge/crypto-ws-api"/></a>
 ***
-For :heavy_check_mark:Binance, 
+For :heavy_check_mark:Binance, :heavy_check_mark:OKX, :heavy_check_mark:Bitfinex
 ***
 
 ## Features
-Lightweight and efficient solution to utilize of all available methods provided through the:
+Lightweight and efficient solution to utilize of all available methods** provided through the:
 * [Binance Websocket API v3](https://developers.binance.com/docs/binance-trading-api/websocket_api)
+* [OKX Websocket API v5](https://www.okx.com/docs-v5/en/#overview-websocket)
+* [Bitfinex Websocket Inputs](https://docs.bitfinex.com/reference/ws-auth-input)
+
+** Not for channel by one-way subscription, for **_request <-> response_** mode only
 
 ### Session management layer for:
 - Credentials
 - Connection
 - Keepalive
 - Error handling
 - Limits control
 - Methods construction
-  + Generating session request id by default
   + Creating request on-the-fly from method name and params: {}
   + Generating signature if necessary
   + Response handling
 - logging
 
 ### User interface layer
 - Start session instance
-- Getting session operational status
 - Send async request
 - Get response or raised exception
+- Reuse instance for different type requests
 - Stop session instance
 
 ## Get started
 ### Install use PIP
 
 ```console
 pip install crypto_ws_api
@@ -82,14 +65,20 @@
 > 
 >Can't find config file! Creating it...
 > 
 >Before first run set account(s) API key into /home/ubuntu/.config/crypto_ws_api/ws_api.toml
 
 ### Prepare exchange account
 * For test purpose log in at [Binance Spot Test Network](https://testnet.binance.vision/)
+
+For OKX and Bitfinex, unlike Binance, a limited number of methods are implemented at the WS API level,
+such as creating, modifying, and deleting orders.
+There are no public get-time (), ping-pong, etc., so this demo script is limited to calling Binance
+to demonstrate capabilities.
+
 * Create API Key
 * After install and create environment specify api_key and api_secret to the config file
 
 ### Start demo
 * Run in terminal window
 ```
 crypto_ws_api_demo
@@ -98,61 +87,99 @@
 ## Useful tips
 
 _*`crypto_ws_api/demo.py` - complete and fully functional example*_
 
 ### Get credentials and create user session
 
 ```bazaar
-from crypto_ws_api.ws_session import get_credentials, UserWSSession
+from crypto_ws_api.ws_session import UserWSSession
 
-# Can be omitted if you have credentials
-_exchange, _test_net, api_key, api_secret, ws_api_endpoint = get_credentials(account_name)
+# Get credentials and create user session
+# Can be omitted if you have credentials from other source
+exchange, _test_net, api_key, api_secret, passphrase, ws_api_endpoint = get_credentials(account_name)
 
 session = aiohttp.ClientSession()
 
+trade_id = shortuuid.uuid()
+
 user_session = UserWSSession(
+    session,
+    exchange,
+    ws_api_endpoint,
     api_key,
     api_secret,
-    session=session,
-    endpoint=ws_api_endpoint
+    passphrase
 )
-
-await user_session.start()
-print(f"Operational status: {user_session.operational_status}")
-```
-### Demo method's calling
-```bazaar
-await account_information(user_session)
-```
-
-### Stop user session and close aiohttp session
-```bazaar
-await user_session.stop()
-await session.close()
-print(f"Operational status: {user_session.operational_status}")
 ```
 
-### Method call example
+### Method example
 ```bazaar
-async def account_information(user_session: UserWSSession):
+async def account_information(user_session: UserWSSession, _trade_id):
     # https://developers.binance.com/docs/binance-trading-api/websocket_api#account-information-user_data
     try:
         res = await user_session.handle_request(
+            _trade_id,
             "account.status",
-            api_key=True,
-            signed=True
+            _api_key=True,
+            _signed=True
         )
         if res is None:
-            print("Here handling state Out-of-Service")
+            logger.warning("Here handling state Out-of-Service")
     except asyncio.CancelledError:
         pass  # Task cancellation should not be logged as an error
     except Exception as _ex:
-        print(f"Handling exception: {_ex}")
+        logger.error(f"Handling exception: {_ex}")
     else:
-        print(f"Account information (USER_DATA) response: {res}")
+        logger.info(f"Account information (USER_DATA) response: {res}")
+```
+
+### Demo method's calling
+```bazaar
+await account_information(user_session, trade_id)
+```
+
+### Stop user session and close aiohttp session
+```bazaar
+await user_session.stop()
+await session.close()
+```
+
+### Create limit order example
+```bazaar
+if self.exchange == 'binance':
+    params = {
+        "symbol": "BTCUSDT",
+        "side": "SELL",
+        "type": "LIMIT",
+        "timeInForce": "GTC",
+        "price": "23416.10000000",
+        "quantity": "0.00847000",
+    }
+    binance_res = await user_session.handle_request(trade_id, "order.place", params, _api_key=True, _signed=True)
+
+elif self.exchange == 'bitfinex':
+    params = {
+        "type": "EXCHANGE LIMIT",
+        "symbol": "tBTCUSDT",
+        "price": "23416.10000000",
+        "amount": ('' if side == 'BUY' else '-') + "0.00847000",
+    }
+    bitfnex_res = await user_session.handle_request(trade_id, "on", params)
+
+elif self.exchange == 'okx':
+    params = {
+        "instId": "BTC-USDT",
+        "tdMode": "cash",
+        "clOrdId": "client_order_id",
+        "side": "buy",
+        "ordType": "limit",
+        "sz": "0.00847000",
+        "px": "23416.10000000",
+    }
+    okx_res = await user_session.handle_request(trade_id, "order", params)
 ```
 
 ### Logging setup
 For configure logging in multi-module project use next snippet for yours `main()`:
 ```bazaar
 import logging.handlers
 
@@ -165,19 +192,16 @@
 #
 root_logger = logging.getLogger()
 root_logger.setLevel(logging.DEBUG)
 root_logger.addHandler(sh)
 ```
 
 ## [Limits control](https://developers.binance.com/docs/binance-trading-api/websocket_api#general-information-on-rate-limits) :link:
-Upon reaching the limit threshold of each type, the session switches to the Out-of-Service state. Monitor the values
-of the variables `user_session.operational_status` and `user_session.order_handling`
-
+Upon reaching the limit threshold of each type, the session switches to the Out-of-Service state.
 If you send a request in this state, the answer will be `None`
 
 *In any case, you are protected from exceeding limits and blocking for this reason*
 
 ## Donate
 *BNB*, *BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92
 
 *USDT* (TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
-
```

#### html2text {}

```diff
@@ -1,71 +1,77 @@
-Metadata-Version: 2.1 Name: crypto-ws-api Version: 1.0.1.post3 Summary: Crypto
-WS API connector for ASYNC requests Author-email: Jerry Fedorenko
-fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
-markdown Classifier: Programming Language :: Python :: 3 Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: MIT License Classifier: Operating System :: Unix Classifier: Operating
-System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper Requires-Dist: aiohttp==3.8.4 Requires-Dist:
-shortuuid~=1.0.11 Requires-Dist: platformdirs~=3.8.0 Requires-Dist:
-toml~=0.10.2 Project-URL: Source, https://github.com/DogsTailFarmer/crypto-ws-
-api
 ****** [https://user-images.githubusercontent.com/77513676/250364389-cbedc171-
   a930-4467-a0cd-21627a6a41ed.svg]Crypto WS API connector for ASYNC requests
                                     ******
       ***** Full coverage of all methods provided by the interface *****
 **** Provides of connection management, keepalive and rate limits control ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/2d2a654ba393eb88d911/
 maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** For :
-heavy_check_mark:Binance, *** ## Features Lightweight and efficient solution to
-utilize of all available methods provided through the: * [Binance Websocket API
-v3](https://developers.binance.com/docs/binance-trading-api/websocket_api) ###
+heavy_check_mark:Binance, :heavy_check_mark:OKX, :heavy_check_mark:Bitfinex ***
+## Features Lightweight and efficient solution to utilize of all available
+methods** provided through the: * [Binance Websocket API v3](https://
+developers.binance.com/docs/binance-trading-api/websocket_api) * [OKX Websocket
+API v5](https://www.okx.com/docs-v5/en/#overview-websocket) * [Bitfinex
+Websocket Inputs](https://docs.bitfinex.com/reference/ws-auth-input) ** Not for
+channel by one-way subscription, for **_request <-> response_** mode only ###
 Session management layer for: - Credentials - Connection - Keepalive - Error
-handling - Limits control - Methods construction + Generating session request
-id by default + Creating request on-the-fly from method name and params: {} +
-Generating signature if necessary + Response handling - logging ### User
-interface layer - Start session instance - Getting session operational status -
-Send async request - Get response or raised exception - Stop session instance
-## Get started ### Install use PIP ```console pip install crypto_ws_api ``` For
-upgrade to latest versions use: ```console pip install -U crypto_ws_api ```
-After first install create environment by run ```console crypto_ws_api_init ```
-in terminal window. The config directory will be created. You get path to
-config: >ubuntu@ubuntu:~$ crypto_ws_api_init > >Can't find config file!
-Creating it... > >Before first run set account(s) API key into /home/
-ubuntu/.config/crypto_ws_api/ws_api.toml ### Prepare exchange account * For
-test purpose log in at [Binance Spot Test Network](https://
-testnet.binance.vision/) * Create API Key * After install and create
+handling - Limits control - Methods construction + Creating request on-the-fly
+from method name and params: {} + Generating signature if necessary + Response
+handling - logging ### User interface layer - Start session instance - Send
+async request - Get response or raised exception - Reuse instance for different
+type requests - Stop session instance ## Get started ### Install use PIP
+```console pip install crypto_ws_api ``` For upgrade to latest versions use:
+```console pip install -U crypto_ws_api ``` After first install create
+environment by run ```console crypto_ws_api_init ``` in terminal window. The
+config directory will be created. You get path to config: >ubuntu@ubuntu:~$
+crypto_ws_api_init > >Can't find config file! Creating it... > >Before first
+run set account(s) API key into /home/ubuntu/.config/crypto_ws_api/ws_api.toml
+### Prepare exchange account * For test purpose log in at [Binance Spot Test
+Network](https://testnet.binance.vision/) For OKX and Bitfinex, unlike Binance,
+a limited number of methods are implemented at the WS API level, such as
+creating, modifying, and deleting orders. There are no public get-time (),
+ping-pong, etc., so this demo script is limited to calling Binance to
+demonstrate capabilities. * Create API Key * After install and create
 environment specify api_key and api_secret to the config file ### Start demo *
 Run in terminal window ``` crypto_ws_api_demo ``` ## Useful tips
 _*`crypto_ws_api/demo.py` - complete and fully functional example*_ ### Get
 credentials and create user session ```bazaar from crypto_ws_api.ws_session
-import get_credentials, UserWSSession # Can be omitted if you have credentials
-_exchange, _test_net, api_key, api_secret, ws_api_endpoint = get_credentials
-(account_name) session = aiohttp.ClientSession() user_session = UserWSSession
-( api_key, api_secret, session=session, endpoint=ws_api_endpoint ) await
-user_session.start() print(f"Operational status:
-{user_session.operational_status}") ``` ### Demo method's calling ```bazaar
-await account_information(user_session) ``` ### Stop user session and close
-aiohttp session ```bazaar await user_session.stop() await session.close() print
-(f"Operational status: {user_session.operational_status}") ``` ### Method call
-example ```bazaar async def account_information(user_session: UserWSSession): #
-https://developers.binance.com/docs/binance-trading-api/websocket_api#account-
-information-user_data try: res = await user_session.handle_request
-( "account.status", api_key=True, signed=True ) if res is None: print("Here
-handling state Out-of-Service") except asyncio.CancelledError: pass # Task
-cancellation should not be logged as an error except Exception as _ex: print
-(f"Handling exception: {_ex}") else: print(f"Account information (USER_DATA)
-response: {res}") ``` ### Logging setup For configure logging in multi-module
+import UserWSSession # Get credentials and create user session # Can be omitted
+if you have credentials from other source exchange, _test_net, api_key,
+api_secret, passphrase, ws_api_endpoint = get_credentials(account_name) session
+= aiohttp.ClientSession() trade_id = shortuuid.uuid() user_session =
+UserWSSession( session, exchange, ws_api_endpoint, api_key, api_secret,
+passphrase ) ``` ### Method example ```bazaar async def account_information
+(user_session: UserWSSession, _trade_id): # https://developers.binance.com/
+docs/binance-trading-api/websocket_api#account-information-user_data try: res =
+await user_session.handle_request( _trade_id, "account.status", _api_key=True,
+_signed=True ) if res is None: logger.warning("Here handling state Out-of-
+Service") except asyncio.CancelledError: pass # Task cancellation should not be
+logged as an error except Exception as _ex: logger.error(f"Handling exception:
+{_ex}") else: logger.info(f"Account information (USER_DATA) response: {res}")
+``` ### Demo method's calling ```bazaar await account_information(user_session,
+trade_id) ``` ### Stop user session and close aiohttp session ```bazaar await
+user_session.stop() await session.close() ``` ### Create limit order example
+```bazaar if self.exchange == 'binance': params = { "symbol": "BTCUSDT",
+"side": "SELL", "type": "LIMIT", "timeInForce": "GTC", "price":
+"23416.10000000", "quantity": "0.00847000", } binance_res = await
+user_session.handle_request(trade_id, "order.place", params, _api_key=True,
+_signed=True) elif self.exchange == 'bitfinex': params = { "type": "EXCHANGE
+LIMIT", "symbol": "tBTCUSDT", "price": "23416.10000000", "amount": ('' if side
+== 'BUY' else '-') + "0.00847000", } bitfnex_res = await
+user_session.handle_request(trade_id, "on", params) elif self.exchange ==
+'okx': params = { "instId": "BTC-USDT", "tdMode": "cash", "clOrdId":
+"client_order_id", "side": "buy", "ordType": "limit", "sz": "0.00847000", "px":
+"23416.10000000", } okx_res = await user_session.handle_request(trade_id,
+"order", params) ``` ### Logging setup For configure logging in multi-module
 project use next snippet for yours `main()`: ```bazaar import logging.handlers
 logger = logging.getLogger(__name__) formatter = logging.Formatter(fmt="[%
 (asctime)s: %(levelname)s] %(message)s") # sh = logging.StreamHandler()
 sh.setFormatter(formatter) sh.setLevel(logging.DEBUG) # root_logger =
 logging.getLogger() root_logger.setLevel(logging.DEBUG) root_logger.addHandler
 (sh) ``` ## [Limits control](https://developers.binance.com/docs/binance-
 trading-api/websocket_api#general-information-on-rate-limits) :link: Upon
 reaching the limit threshold of each type, the session switches to the Out-of-
-Service state. Monitor the values of the variables
-`user_session.operational_status` and `user_session.order_handling` If you send
-a request in this state, the answer will be `None` *In any case, you are
-protected from exceeding limits and blocking for this reason* ## Donate *BNB*,
-*BUSD*, *USDT* (BEP20) 0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT*
-(TRC20) TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
+Service state. If you send a request in this state, the answer will be `None`
+*In any case, you are protected from exceeding limits and blocking for this
+reason* ## Donate *BNB*, *BUSD*, *USDT* (BEP20)
+0x5b52c6ba862b11318616ee6cef64388618318b92 *USDT* (TRC20)
+TP1Y43dpY7rrRyTSLaSKDZmFirqvRcpopC
```


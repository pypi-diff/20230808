# Comparing `tmp/marketfeed_multi_broker_sdk-0.1.16.tar.gz` & `tmp/marketfeed_multi_broker_sdk-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.16.tar", last modified: Tue Aug  8 04:59:16 2023, max compression
+gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.17.tar", last modified: Tue Aug  8 05:27:53 2023, max compression
```

## Comparing `marketfeed_multi_broker_sdk-0.1.16.tar` & `marketfeed_multi_broker_sdk-0.1.17.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.819860 marketfeed_multi_broker_sdk-0.1.16/
--rw-r--r--   0 farazs     (501) staff       (20)     2703 2023-08-08 04:59:16.819511 marketfeed_multi_broker_sdk-0.1.16/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     2455 2023-08-03 09:47:25.000000 marketfeed_multi_broker_sdk-0.1.16/README.md
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.805776 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/
--rw-r--r--   0 farazs     (501) staff       (20)      448 2023-08-05 14:15:31.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1120 2023-08-05 14:11:02.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/broker_interface.py
--rw-r--r--   0 farazs     (501) staff       (20)     1751 2023-08-07 08:46:42.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/broker_sdk.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.809472 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-08-02 16:32:42.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     2330 2023-08-06 08:04:14.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1599 2023-08-03 09:44:53.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/kotak.py
--rw-r--r--   0 farazs     (501) staff       (20)     1619 2023-08-07 16:41:39.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/kotak_neo.py
--rw-r--r--   0 farazs     (501) staff       (20)     1622 2023-08-03 09:45:07.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     2280 2023-08-05 14:48:05.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/xts.py
--rw-r--r--   0 farazs     (501) staff       (20)     2688 2023-08-08 04:20:49.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/enums.py
--rw-r--r--   0 farazs     (501) staff       (20)     2373 2023-08-07 11:16:09.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/models.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.813596 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)    15471 2023-08-06 08:02:39.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/fyers_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     9781 2023-08-08 04:47:45.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/kotak_neo_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     8695 2023-08-03 05:09:10.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/kotak_services.py
--rw-r--r--   0 farazs     (501) staff       (20)    11255 2023-08-08 04:30:46.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/shoonya_services.py
--rw-r--r--   0 farazs     (501) staff       (20)    11473 2023-08-08 04:31:04.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/xts_services.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.814830 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/utils/
--rw-r--r--   0 farazs     (501) staff       (20)      131 2023-08-02 09:59:25.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/utils/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)      314 2023-08-01 12:50:32.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/utils/env_generator.py
--rw-r--r--   0 farazs     (501) staff       (20)      987 2023-08-07 16:40:41.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/utils/jwt_handler.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.807231 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/
--rw-r--r--   0 farazs     (501) staff       (20)     2703 2023-08-08 04:59:16.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     1331 2023-08-08 04:59:16.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-08 04:59:16.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 farazs     (501) staff       (20)       24 2023-08-08 04:59:16.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/requires.txt
--rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-08 04:59:16.000000 marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/top_level.txt
--rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-08 04:59:16.819955 marketfeed_multi_broker_sdk-0.1.16/setup.cfg
--rw-r--r--   0 farazs     (501) staff       (20)      680 2023-08-08 04:49:20.000000 marketfeed_multi_broker_sdk-0.1.16/setup.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 04:59:16.818746 marketfeed_multi_broker_sdk-0.1.16/tests/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.16/tests/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1650 2023-08-01 12:53:43.000000 marketfeed_multi_broker_sdk-0.1.16/tests/test_fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1146 2023-08-01 12:35:26.000000 marketfeed_multi_broker_sdk-0.1.16/tests/test_fyers_mock.py
--rw-r--r--   0 farazs     (501) staff       (20)     1917 2023-08-01 12:54:15.000000 marketfeed_multi_broker_sdk-0.1.16/tests/test_shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     1662 2023-08-01 12:54:11.000000 marketfeed_multi_broker_sdk-0.1.16/tests/test_xts.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.911925 marketfeed_multi_broker_sdk-0.1.17/
+-rw-r--r--   0 farazs     (501) staff       (20)     2703 2023-08-08 05:27:53.911765 marketfeed_multi_broker_sdk-0.1.17/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     2455 2023-08-03 09:47:25.000000 marketfeed_multi_broker_sdk-0.1.17/README.md
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.905519 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/
+-rw-r--r--   0 farazs     (501) staff       (20)      448 2023-08-05 14:15:31.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1120 2023-08-05 14:11:02.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/broker_interface.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1751 2023-08-07 08:46:42.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/broker_sdk.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.907221 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-08-02 16:32:42.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2330 2023-08-06 08:04:14.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1878 2023-08-08 05:24:27.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/kotak.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:06.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/kotak_neo.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:24.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2280 2023-08-05 14:48:05.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/xts.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2688 2023-08-08 04:20:49.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/enums.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2373 2023-08-07 11:16:09.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/models.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.909089 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)    15471 2023-08-06 08:02:39.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/fyers_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     9783 2023-08-08 05:26:59.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/kotak_neo_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     8695 2023-08-03 05:09:10.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/kotak_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)    11255 2023-08-08 04:30:46.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/shoonya_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)    11473 2023-08-08 04:31:04.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/xts_services.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.910061 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/utils/
+-rw-r--r--   0 farazs     (501) staff       (20)      131 2023-08-02 09:59:25.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/utils/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)      314 2023-08-01 12:50:32.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/utils/env_generator.py
+-rw-r--r--   0 farazs     (501) staff       (20)      987 2023-08-07 16:40:41.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/utils/jwt_handler.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.906316 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/
+-rw-r--r--   0 farazs     (501) staff       (20)     2703 2023-08-08 05:27:53.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     1331 2023-08-08 05:27:53.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-08 05:27:53.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       24 2023-08-08 05:27:53.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/requires.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-08 05:27:53.000000 marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-08 05:27:53.912029 marketfeed_multi_broker_sdk-0.1.17/setup.cfg
+-rw-r--r--   0 farazs     (501) staff       (20)      680 2023-08-08 05:27:42.000000 marketfeed_multi_broker_sdk-0.1.17/setup.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 05:27:53.911461 marketfeed_multi_broker_sdk-0.1.17/tests/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.17/tests/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1650 2023-08-01 12:53:43.000000 marketfeed_multi_broker_sdk-0.1.17/tests/test_fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1146 2023-08-01 12:35:26.000000 marketfeed_multi_broker_sdk-0.1.17/tests/test_fyers_mock.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1917 2023-08-01 12:54:15.000000 marketfeed_multi_broker_sdk-0.1.17/tests/test_shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1662 2023-08-01 12:54:11.000000 marketfeed_multi_broker_sdk-0.1.17/tests/test_xts.py
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed_multi_broker_sdk
-Version: 0.1.16
+Version: 0.1.17
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/README.md` & `marketfeed_multi_broker_sdk-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/broker_interface.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/broker_interface.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/broker_sdk.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/broker_sdk.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/fyers.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/kotak.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/kotak.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # from typing import Any, Dict
 from marketfeed_multi_broker_sdk.broker_interface import BrokerInterface
-from marketfeed_multi_broker_sdk.models import Login, MarginResponse, Order, LoginResponse, OrderResponse, GetTransactionHistoryResponse
+from marketfeed_multi_broker_sdk.models import Login, MarginResponse, Order, LoginResponse, OrderResponse, HoldingResponse, PositionResponse, GetTransactionHistoryResponse
 from marketfeed_multi_broker_sdk.services.kotak_services import KotakAPIServices
 
 
 class KOTAK(BrokerInterface):
 
     def login(self, login_details: Login):
         kotak_api_service = KotakAPIServices()
@@ -22,14 +22,20 @@
         order_number, message = kotak_api_service.KotakPlaceOrder(
             token=token,
             client_code=self.client_code,
             order_details=order_details
         )
         return OrderResponse(order_number=order_number, message=message)
 
+    def holding(self, token) -> HoldingResponse:
+        return HoldingResponse(holding=None, message="not available")
+
+    def position(self, token) -> PositionResponse:
+        return PositionResponse(position=None, message="not available")
+
     def get_transaction_history(self) -> GetTransactionHistoryResponse:
         # Replace with actual implementation for getting transaction history from xts
         print(
             f"Getting transaction history for xts client {self.client_code}")
         # This is just a placeholder and should be replaced with actual transactions
         transactions = []
         return GetTransactionHistoryResponse(status='success', transactions=transactions)
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/kotak_neo.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/shoonya.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-# from typing import Any, Dict
+from typing import Any, Dict
 from marketfeed_multi_broker_sdk.broker_interface import BrokerInterface
-from marketfeed_multi_broker_sdk.models import Login, MarginResponse, Order, LoginResponse, OrderResponse, GetTransactionHistoryResponse
-from marketfeed_multi_broker_sdk.services.kotak_neo_services import KotakNeoAPIServices
+from marketfeed_multi_broker_sdk.models import Login, MarginResponse, Order, LoginResponse, OrderResponse, HoldingResponse, PositionResponse, GetTransactionHistoryResponse
+from marketfeed_multi_broker_sdk.services.shoonya_services import ShoonyaAPIServices
 
 
-class KOTAK_NEO(BrokerInterface):
+class SHOONYA(BrokerInterface):
 
     def login(self, login_details: Login):
-        kotak_api_service = KotakNeoAPIServices()
-        token, message = kotak_api_service.KotakLogin(
+        shoonya_api_service = ShoonyaAPIServices()
+        token, message = shoonya_api_service.ShoonyaLogin(
             client_code=self.client_code,
-            login_details=login_details,
+            login_details=login_details
         )
         return LoginResponse(token=token, message=message)
 
     def margin(self, token) -> MarginResponse:
         return MarginResponse(margin=None, message="not available")
 
     def place_order(self, token, order_details: Order) -> OrderResponse:
-        kotak_api_service = KotakNeoAPIServices()
-        order_number, message = kotak_api_service.KotakNeoPlaceOrder(
+        shoonya_api_service = ShoonyaAPIServices()
+        order_number, message = shoonya_api_service.ShoonyaPlaceOrder(
             token=token,
             client_code=self.client_code,
             order_details=order_details
         )
         return OrderResponse(order_number=order_number, message=message)
 
+    def holding(self, token) -> HoldingResponse:
+        return HoldingResponse(holding=None, message="not available")
+
+    def position(self, token) -> PositionResponse:
+        return PositionResponse(position=None, message="not available")
+
     def get_transaction_history(self) -> GetTransactionHistoryResponse:
-        # Replace with actual implementation for getting transaction history from xts
+        # Replace with actual implementation for getting transaction history from fyers
         print(
-            f"Getting transaction history for xts client {self.client_code}")
+            f"Getting transaction history for fyers client {self.client_code}")
         # This is just a placeholder and should be replaced with actual transactions
         transactions = []
         return GetTransactionHistoryResponse(status='success', transactions=transactions)
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/shoonya.py` & `marketfeed_multi_broker_sdk-0.1.17/tests/test_xts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,51 @@
-from typing import Any, Dict
-from marketfeed_multi_broker_sdk.broker_interface import BrokerInterface
-from marketfeed_multi_broker_sdk.models import Login, MarginResponse, Order, LoginResponse, OrderResponse, GetTransactionHistoryResponse
-from marketfeed_multi_broker_sdk.services.shoonya_services import ShoonyaAPIServices
-
-
-class SHOONYA(BrokerInterface):
-
-    def login(self, login_details: Login):
-        shoonya_api_service = ShoonyaAPIServices()
-        token, message = shoonya_api_service.ShoonyaLogin(
-            client_code=self.client_code,
-            login_details=login_details
-        )
-        return LoginResponse(token=token, message=message)
-
-    def margin(self, token) -> MarginResponse:
-        return MarginResponse(margin=None, message="not available")
-
-    def place_order(self, token, order_details: Order) -> OrderResponse:
-        shoonya_api_service = ShoonyaAPIServices()
-        order_number, message = shoonya_api_service.ShoonyaPlaceOrder(
-            token=token,
-            client_code=self.client_code,
-            order_details=order_details
+import pytest
+from marketfeed_multi_broker_sdk.brokers.xts import XTS
+from marketfeed_multi_broker_sdk.models import Login, LoginResponse, OrderResponse, GetTransactionHistoryResponse, Order, Transaction
+from marketfeed_multi_broker_sdk.utils.env_generator import load_env_value
+
+client_code = load_env_value('XTS_CLIENT_CODE')
+api_key = load_env_value('XTS_API_KEY')
+api_secret = load_env_value('XTS_API_SECRET')
+
+
+@pytest.fixture
+def broker():
+    return XTS(client_code=client_code)
+
+
+def test_login(broker):
+    response = broker.login(
+        Login(
+            api_key=api_key,
+            api_secret=api_secret
         )
-        return OrderResponse(order_number=order_number, message=message)
-
-    def get_transaction_history(self) -> GetTransactionHistoryResponse:
-        # Replace with actual implementation for getting transaction history from fyers
-        print(
-            f"Getting transaction history for fyers client {self.client_code}")
-        # This is just a placeholder and should be replaced with actual transactions
-        transactions = []
-        return GetTransactionHistoryResponse(status='success', transactions=transactions)
+    )
+    assert isinstance(response, LoginResponse)
+    assert response.token != None
+    assert response.token != ''
+
+
+@pytest.mark.parametrize(
+    "order_details, expected_status",
+    [
+        ({"order_id": "1", "product": "Apple",
+         "price": 150.00, "quantity": 10}, 'success'),
+        ({"order_id": "1", "product": "Apple",
+          "price": 150.00, "quantity": 10}, 'success'),
+        # Add more test cases here
+    ],
+)
+def test_place_order(broker, order_details, expected_status):
+    response = broker.place_order(order_details)
+    assert isinstance(response, OrderResponse)
+    assert response.status == expected_status
+    assert isinstance(response.order, Order)
+
+
+def test_get_transaction_history(broker):
+    response = broker.get_transaction_history()
+    assert isinstance(response, GetTransactionHistoryResponse)
+    assert response.status == 'success'
+    assert isinstance(response.transactions, list)
+    for transaction in response.transactions:
+        assert isinstance(transaction, Transaction)
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/brokers/xts.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/brokers/xts.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/enums.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/enums.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/models.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/models.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/fyers_services.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/fyers_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/kotak_neo_services.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/kotak_neo_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             except Exception as e:
                 return [self._ERROR, response_json['error']]
 
         except Exception as e:
             print("EE", e)
             return [self._ERROR, e]
 
-    def _validate_2FA(self, app_token, one_time_token, mobile_number, pin):
+    def _validate_2FA(self, app_token, one_time_token, mobile_number, mpin):
         try:
             headers = {
                 'sid': one_time_token['sid'],
                 'Auth': one_time_token['token'],
                 'Content-Type': 'application/json',
                 'Authorization': f'Bearer {app_token}',
             }
@@ -160,15 +160,15 @@
             return ["", one_time_token_response[1]]
         one_time_token = one_time_token_response[1]
 
         session_token_response = super()._validate_2FA(
             app_token=app_token,
             one_time_token=one_time_token,
             mobile_number=login_details.mobile,
-            pin=login_details.mpin
+            mpin=login_details.mpin
         )
         if session_token_response[0] == super()._ERROR:
             return ["", session_token_response[1]]
         session_token = session_token_response[1]
 
         # The data you want to store
         token_payload = {
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/kotak_services.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/kotak_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/shoonya_services.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/shoonya_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/services/xts_services.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/services/xts_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk/utils/jwt_handler.py` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk/utils/jwt_handler.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed-multi-broker-sdk
-Version: 0.1.16
+Version: 0.1.17
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt` & `marketfeed_multi_broker_sdk-0.1.17/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/setup.py` & `marketfeed_multi_broker_sdk-0.1.17/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the long description from the README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='marketfeed_multi_broker_sdk',
-    version='0.1.16',
+    version='0.1.17',
     url='https://github.com/tradeclone/multi-broker-sdk',
     author='Faraz',
     author_email='faraz.s@marketfeed.com',
     description='Multi Broker SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     packages=find_packages(),
```

### Comparing `marketfeed_multi_broker_sdk-0.1.16/tests/test_fyers.py` & `marketfeed_multi_broker_sdk-0.1.17/tests/test_fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/tests/test_fyers_mock.py` & `marketfeed_multi_broker_sdk-0.1.17/tests/test_fyers_mock.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.16/tests/test_shoonya.py` & `marketfeed_multi_broker_sdk-0.1.17/tests/test_shoonya.py`

 * *Files identical despite different names*


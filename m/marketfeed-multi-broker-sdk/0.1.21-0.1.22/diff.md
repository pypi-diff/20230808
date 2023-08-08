# Comparing `tmp/marketfeed_multi_broker_sdk-0.1.21.tar.gz` & `tmp/marketfeed_multi_broker_sdk-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.21.tar", last modified: Tue Aug  8 11:42:28 2023, max compression
+gzip compressed data, was "marketfeed_multi_broker_sdk-0.1.22.tar", last modified: Tue Aug  8 11:44:59 2023, max compression
```

## Comparing `marketfeed_multi_broker_sdk-0.1.21.tar` & `marketfeed_multi_broker_sdk-0.1.22.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.903864 marketfeed_multi_broker_sdk-0.1.21/
--rw-r--r--   0 farazs     (501) staff       (20)     3175 2023-08-08 11:42:28.903695 marketfeed_multi_broker_sdk-0.1.21/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     2927 2023-08-08 07:08:11.000000 marketfeed_multi_broker_sdk-0.1.21/README.md
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.895767 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/
--rw-r--r--   0 farazs     (501) staff       (20)      448 2023-08-05 14:15:31.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1120 2023-08-05 14:11:02.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/broker_interface.py
--rw-r--r--   0 farazs     (501) staff       (20)     1751 2023-08-07 08:46:42.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/broker_sdk.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.898887 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-08-02 16:32:42.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     2330 2023-08-06 08:04:14.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1878 2023-08-08 05:24:27.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/kotak.py
--rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:06.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/kotak_neo.py
--rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:24.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     2280 2023-08-05 14:48:05.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/xts.py
--rw-r--r--   0 farazs     (501) staff       (20)     2842 2023-08-08 11:23:53.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/enums.py
--rw-r--r--   0 farazs     (501) staff       (20)     2373 2023-08-07 11:16:09.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/models.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.900724 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)    15471 2023-08-06 08:02:39.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/fyers_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     9746 2023-08-08 06:53:52.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/kotak_neo_services.py
--rw-r--r--   0 farazs     (501) staff       (20)     8635 2023-08-08 06:53:15.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/kotak_services.py
--rw-r--r--   0 farazs     (501) staff       (20)    11255 2023-08-08 04:30:46.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/shoonya_services.py
--rw-r--r--   0 farazs     (501) staff       (20)    11473 2023-08-08 04:31:04.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/xts_services.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.901637 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/utils/
--rw-r--r--   0 farazs     (501) staff       (20)      131 2023-08-02 09:59:25.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/utils/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)      314 2023-08-01 12:50:32.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/utils/env_generator.py
--rw-r--r--   0 farazs     (501) staff       (20)      987 2023-08-07 16:40:41.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/utils/jwt_handler.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.896880 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/
--rw-r--r--   0 farazs     (501) staff       (20)     3175 2023-08-08 11:42:28.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
--rw-r--r--   0 farazs     (501) staff       (20)     1355 2023-08-08 11:42:28.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-08 11:42:28.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 farazs     (501) staff       (20)       35 2023-08-08 11:42:28.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/requires.txt
--rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-08 11:42:28.000000 marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/top_level.txt
--rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-08 11:42:28.903916 marketfeed_multi_broker_sdk-0.1.21/setup.cfg
--rw-r--r--   0 farazs     (501) staff       (20)      702 2023-08-08 11:42:20.000000 marketfeed_multi_broker_sdk-0.1.21/setup.py
-drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:42:28.903298 marketfeed_multi_broker_sdk-0.1.21/tests/
--rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.21/tests/__init__.py
--rw-r--r--   0 farazs     (501) staff       (20)     1650 2023-08-01 12:53:43.000000 marketfeed_multi_broker_sdk-0.1.21/tests/test_fyers.py
--rw-r--r--   0 farazs     (501) staff       (20)     1146 2023-08-01 12:35:26.000000 marketfeed_multi_broker_sdk-0.1.21/tests/test_fyers_mock.py
--rw-r--r--   0 farazs     (501) staff       (20)     2003 2023-08-08 06:37:19.000000 marketfeed_multi_broker_sdk-0.1.21/tests/test_kotak_neo.py
--rw-r--r--   0 farazs     (501) staff       (20)     1917 2023-08-01 12:54:15.000000 marketfeed_multi_broker_sdk-0.1.21/tests/test_shoonya.py
--rw-r--r--   0 farazs     (501) staff       (20)     1662 2023-08-01 12:54:11.000000 marketfeed_multi_broker_sdk-0.1.21/tests/test_xts.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.570927 marketfeed_multi_broker_sdk-0.1.22/
+-rw-r--r--   0 farazs     (501) staff       (20)     3175 2023-08-08 11:44:59.570722 marketfeed_multi_broker_sdk-0.1.22/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     2927 2023-08-08 07:08:11.000000 marketfeed_multi_broker_sdk-0.1.22/README.md
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.560441 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/
+-rw-r--r--   0 farazs     (501) staff       (20)      448 2023-08-05 14:15:31.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1120 2023-08-05 14:11:02.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/broker_interface.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1751 2023-08-07 08:46:42.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/broker_sdk.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.563904 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-08-02 16:32:42.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2330 2023-08-06 08:04:14.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1878 2023-08-08 05:24:27.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/kotak.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:06.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/kotak_neo.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1901 2023-08-08 05:24:24.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2280 2023-08-05 14:48:05.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/xts.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2842 2023-08-08 11:23:53.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/enums.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2373 2023-08-07 11:16:09.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/models.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.566778 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-27 05:40:23.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)    15471 2023-08-06 08:02:39.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/fyers_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     9746 2023-08-08 06:53:52.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/kotak_neo_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)     8635 2023-08-08 06:53:15.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/kotak_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)    11255 2023-08-08 04:30:46.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/shoonya_services.py
+-rw-r--r--   0 farazs     (501) staff       (20)    11473 2023-08-08 04:31:04.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/xts_services.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.567980 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/utils/
+-rw-r--r--   0 farazs     (501) staff       (20)      131 2023-08-02 09:59:25.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/utils/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)      314 2023-08-01 12:50:32.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/utils/env_generator.py
+-rw-r--r--   0 farazs     (501) staff       (20)      987 2023-08-07 16:40:41.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/utils/jwt_handler.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.561808 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/
+-rw-r--r--   0 farazs     (501) staff       (20)     3175 2023-08-08 11:44:59.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 farazs     (501) staff       (20)     1355 2023-08-08 11:44:59.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 farazs     (501) staff       (20)        1 2023-08-08 11:44:59.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       36 2023-08-08 11:44:59.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/requires.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       34 2023-08-08 11:44:59.000000 marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/top_level.txt
+-rw-r--r--   0 farazs     (501) staff       (20)       38 2023-08-08 11:44:59.571004 marketfeed_multi_broker_sdk-0.1.22/setup.cfg
+-rw-r--r--   0 farazs     (501) staff       (20)      703 2023-08-08 11:44:57.000000 marketfeed_multi_broker_sdk-0.1.22/setup.py
+drwxr-xr-x   0 farazs     (501) staff       (20)        0 2023-08-08 11:44:59.570262 marketfeed_multi_broker_sdk-0.1.22/tests/
+-rw-r--r--   0 farazs     (501) staff       (20)        0 2023-07-04 08:53:00.000000 marketfeed_multi_broker_sdk-0.1.22/tests/__init__.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1650 2023-08-01 12:53:43.000000 marketfeed_multi_broker_sdk-0.1.22/tests/test_fyers.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1146 2023-08-01 12:35:26.000000 marketfeed_multi_broker_sdk-0.1.22/tests/test_fyers_mock.py
+-rw-r--r--   0 farazs     (501) staff       (20)     2003 2023-08-08 06:37:19.000000 marketfeed_multi_broker_sdk-0.1.22/tests/test_kotak_neo.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1917 2023-08-01 12:54:15.000000 marketfeed_multi_broker_sdk-0.1.22/tests/test_shoonya.py
+-rw-r--r--   0 farazs     (501) staff       (20)     1662 2023-08-01 12:54:11.000000 marketfeed_multi_broker_sdk-0.1.22/tests/test_xts.py
```

### Comparing `marketfeed_multi_broker_sdk-0.1.21/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed_multi_broker_sdk
-Version: 0.1.21
+Version: 0.1.22
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
```

### Comparing `marketfeed_multi_broker_sdk-0.1.21/README.md` & `marketfeed_multi_broker_sdk-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/broker_interface.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/broker_interface.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/broker_sdk.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/broker_sdk.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/fyers.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/kotak.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/kotak.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/kotak_neo.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/kotak_neo.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/shoonya.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/shoonya.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/brokers/xts.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/brokers/xts.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/enums.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/enums.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/models.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/models.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/fyers_services.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/fyers_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/kotak_neo_services.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/kotak_neo_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/kotak_services.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/kotak_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/shoonya_services.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/shoonya_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/services/xts_services.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/services/xts_services.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk/utils/jwt_handler.py` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk/utils/jwt_handler.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/PKG-INFO` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketfeed-multi-broker-sdk
-Version: 0.1.21
+Version: 0.1.22
 Summary: Multi Broker SDK
 Home-page: https://github.com/tradeclone/multi-broker-sdk
 Author: Faraz
 Author-email: faraz.s@marketfeed.com
 Description-Content-Type: text/markdown
 
 # Multi-Broker SDK
```

### Comparing `marketfeed_multi_broker_sdk-0.1.21/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt` & `marketfeed_multi_broker_sdk-0.1.22/marketfeed_multi_broker_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/setup.py` & `marketfeed_multi_broker_sdk-0.1.22/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # Get the long description from the README file
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='marketfeed_multi_broker_sdk',
-    version='0.1.21',
+    version='0.1.22',
     url='https://github.com/tradeclone/multi-broker-sdk',
     author='Faraz',
     author_email='faraz.s@marketfeed.com',
     description='Multi Broker SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     packages=find_packages(),
     install_requires=[
         'requests',
         'pydantic',
-        'pyotp'
+        'pyotp',
         'load_dotenv'
     ],
 )
```

### Comparing `marketfeed_multi_broker_sdk-0.1.21/tests/test_fyers.py` & `marketfeed_multi_broker_sdk-0.1.22/tests/test_fyers.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/tests/test_fyers_mock.py` & `marketfeed_multi_broker_sdk-0.1.22/tests/test_fyers_mock.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/tests/test_kotak_neo.py` & `marketfeed_multi_broker_sdk-0.1.22/tests/test_kotak_neo.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/tests/test_shoonya.py` & `marketfeed_multi_broker_sdk-0.1.22/tests/test_shoonya.py`

 * *Files identical despite different names*

### Comparing `marketfeed_multi_broker_sdk-0.1.21/tests/test_xts.py` & `marketfeed_multi_broker_sdk-0.1.22/tests/test_xts.py`

 * *Files identical despite different names*


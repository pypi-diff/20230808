# Comparing `tmp/freeoptionschain-0.0.2.tar.gz` & `tmp/freeoptionschain-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeoptionschain-0.0.2.tar", last modified: Tue Aug  8 16:31:59 2023, max compression
+gzip compressed data, was "freeoptionschain-0.1.tar", last modified: Tue Aug  8 16:32:02 2023, max compression
```

## Comparing `freeoptionschain-0.0.2.tar` & `freeoptionschain-0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:59.401127 freeoptionschain-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:59.401127 freeoptionschain-0.0.2/FOC/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/FOC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/FOC/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/FOC/defined.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/FOC/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-08-08 16:31:59.401127 freeoptionschain-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-08 16:31:49.000000 freeoptionschain-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:31:59.401127 freeoptionschain-0.0.2/freeoptionschain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-08-08 16:31:59.000000 freeoptionschain-0.0.2/freeoptionschain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 16:31:59.000000 freeoptionschain-0.0.2/freeoptionschain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:31:59.000000 freeoptionschain-0.0.2/freeoptionschain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 16:31:59.000000 freeoptionschain-0.0.2/freeoptionschain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 16:31:59.000000 freeoptionschain-0.0.2/freeoptionschain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 16:31:59.401127 freeoptionschain-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-08 16:31:52.000000 freeoptionschain-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:02.986173 freeoptionschain-0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:02.982173 freeoptionschain-0.1/FOC/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 16:31:48.000000 freeoptionschain-0.1/FOC/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   880472 2023-08-08 16:31:48.000000 freeoptionschain-0.1/FOC/db.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 16:31:48.000000 freeoptionschain-0.1/FOC/defined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-08-08 16:31:48.000000 freeoptionschain-0.1/FOC/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-08-08 16:31:48.000000 freeoptionschain-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-08 16:32:02.986173 freeoptionschain-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-08-08 16:31:48.000000 freeoptionschain-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:02.986173 freeoptionschain-0.1/freeoptionschain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-08-08 16:32:02.000000 freeoptionschain-0.1/freeoptionschain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-08 16:32:02.000000 freeoptionschain-0.1/freeoptionschain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:32:02.000000 freeoptionschain-0.1/freeoptionschain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 16:32:02.000000 freeoptionschain-0.1/freeoptionschain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-08 16:32:02.000000 freeoptionschain-0.1/freeoptionschain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-08 16:32:02.986173 freeoptionschain-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-08 16:31:55.000000 freeoptionschain-0.1/setup.py
```

### Comparing `freeoptionschain-0.0.2/FOC/defined.py` & `freeoptionschain-0.1/FOC/defined.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 def get_options_price_url(tickersymbol:str, expiration_date:str,option_type):
     option_type = enum_OptionType_to_string(option_type)
     return f"https://api.nasdaq.com/api/quote/{tickersymbol}/option-chain?assetclass=stocks&limit=1000&fromdate={expiration_date}&todate={expiration_date}&excode=oprac&callput={option_type}&money=all&type=all"
 
 def get_options_contract_url(tickersymbol:str, recordID:str):
     return f"https://api.nasdaq.com/api/quote/{tickersymbol}/option-chain?assetclass=stocks&recordID={recordID}"
 
-def get_stock_price_url(tickersymbol:str, last_n_price:int):
-    str_last_n_price = str(last_n_price)
-    return f"https://api.nasdaq.com/api/quote/{tickersymbol}/realtime-trades?&limit={str_last_n_price}"
-
 class OptionType(Enum):
     CALL = auto()
     PUT = auto()
     CALLPUT = auto()
 
 def get_OptionType(optiontype):
     if isinstance(optiontype, str):
```

### Comparing `freeoptionschain-0.0.2/FOC/main.py` & `freeoptionschain-0.1/FOC/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .defined import *
 from .db import *
-import requests, pytz,threading, concurrent.futures, pytz,json
+import requests, pytz,threading, concurrent.futures, pytz
 import pandas as pd
 import yfinance as yf
 from yahoo_fin import options as op
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
 from urllib.parse import unquote
 from json import JSONDecodeError
@@ -216,46 +216,14 @@
         try:
             options_data = response.json()
         except JSONDecodeError:
             pass
         
         return options_data
     
-    def get_stocks_data(self,tickersymbol:str,last_n_price:int):
-        stocks_data = None
-
-        url = get_stock_price_url(tickersymbol,last_n_price)
-        headers = {
-                    'authority': 'api.nasdaq.com',
-                    'accept': 'application/json, text/plain, */*',
-                    'accept-language': 'en-GB,en-US;q=0.9,en;q=0.8',
-                    'origin': 'https://www.nasdaq.com',
-                    'referer': 'https://www.nasdaq.com/',
-                    'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
-                    'sec-ch-ua-mobile': '?0',
-                    'sec-ch-ua-platform': '"Linux"',
-                    'sec-fetch-dest': 'empty',
-                    'sec-fetch-mode': 'cors',
-                    'sec-fetch-site': 'same-site',
-                    'user-agent': self.User_Agent,
-                    }
-        
-        response = requests.get(
-                                url,
-                                headers=headers,
-                                cookies=self.session.cookies,
-                                timeout=100
-                            )
-        try:
-            stocks_data = response.json()
-        except JSONDecodeError:
-            pass
-        
-        return stocks_data
-    
     def get_options_type(self,contract_symbol:str):
         char_optiontype = contract_symbol.split(contract_symbol_delimiter)[-1][6] #options type symbol is the 7th char, e.g. YYMMddT000000
         char_optiontype = char_optiontype.upper()
         optiontype = OptionType.CALL if char_optiontype == 'C' else OptionType.PUT
         return optiontype
 
     def get_options_price_data(self,contract_symbol:str):
@@ -278,20 +246,7 @@
             options_price_data['contract_symbol'] = contract_symbol
             
             if self.dbconn:
                 df_to_save = options_price_data.copy()
                 self.dbconn.insert_data("options_price_data", df_to_save)
             
         return options_price_data
-    
-    def get_stock_price(self, tickersymbol:str, last_n_price = 1):
-        stock_price_data = None
-        stock_data = self.get_stocks_data(tickersymbol,last_n_price)
-        if stock_data is not None:
-            stock_price_data = {}
-            stock_price_data['price'] = json.dumps(self.json_extract_node(stock_data,['data','rows']))
-            
-            price_meta = self.json_extract_node(stock_data,['data','topTable','rows'])[0]
-            stock_price_data.update(price_meta)
-            stock_price_data = pd.DataFrame(stock_price_data, index=[0])
-
-        return stock_price_data
```

### Comparing `freeoptionschain-0.0.2/LICENSE` & `freeoptionschain-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeoptionschain-0.0.2/PKG-INFO` & `freeoptionschain-0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeoptionschain
-Version: 0.0.2
+Version: 0.1
 Summary: This library module retrieves stock options data from NASDAQ.
 Home-page: https://github.com/benjamincham/free_options_chain
 Author: Benjamin Cham
 Author-email: benjaminchamwb@gmail.com
 Project-URL: Bug Tracker, https://github.com/benjamincham/free_options_chain/issues
 Project-URL: Changelog, https://github.com/benjamincham/free_options_chain/releases
 Classifier: Topic :: Office/Business :: Financial :: Investment
@@ -110,26 +110,14 @@
 ref_FOC = FOC()
 
 # get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
 contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
 #fetch options contract with greeks
 options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
-Fetch current price of the stock
----------------------------------
-To fetch the current price of a ticker symbol, you can
-simply use:
-
-``` {.sourceCode .python}
-#create instance
-ref_FOC = FOC()
-
-#fetch current stock price for AAPL
-stock_price = ref_FOC.get_stock_price("AAPL")
-```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E0NVBCJ)
```

### Comparing `freeoptionschain-0.0.2/README.md` & `freeoptionschain-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -90,26 +90,14 @@
 ref_FOC = FOC()
 
 # get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
 contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
 #fetch options contract with greeks
 options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
-Fetch current price of the stock
----------------------------------
-To fetch the current price of a ticker symbol, you can
-simply use:
-
-``` {.sourceCode .python}
-#create instance
-ref_FOC = FOC()
-
-#fetch current stock price for AAPL
-stock_price = ref_FOC.get_stock_price("AAPL")
-```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E0NVBCJ)
```

### Comparing `freeoptionschain-0.0.2/freeoptionschain.egg-info/PKG-INFO` & `freeoptionschain-0.1/freeoptionschain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeoptionschain
-Version: 0.0.2
+Version: 0.1
 Summary: This library module retrieves stock options data from NASDAQ.
 Home-page: https://github.com/benjamincham/free_options_chain
 Author: Benjamin Cham
 Author-email: benjaminchamwb@gmail.com
 Project-URL: Bug Tracker, https://github.com/benjamincham/free_options_chain/issues
 Project-URL: Changelog, https://github.com/benjamincham/free_options_chain/releases
 Classifier: Topic :: Office/Business :: Financial :: Investment
@@ -110,26 +110,14 @@
 ref_FOC = FOC()
 
 # get options contract symbol for AAPL CALL options with strike $200 for 6 October 2023
 contract_symbol = ref_FOC.get_contract_symbol("AAPL",'2023-10-06','CALL',200.0)
 #fetch options contract with greeks
 options_contract = ref_FOC.get_options_price_data(contract_symbol)
 ```
-Fetch current price of the stock
----------------------------------
-To fetch the current price of a ticker symbol, you can
-simply use:
-
-``` {.sourceCode .python}
-#create instance
-ref_FOC = FOC()
-
-#fetch current stock price for AAPL
-stock_price = ref_FOC.get_stock_price("AAPL")
-```
 What else?
 ----------
 
 Let me know what other features would be useful to implement, create an issue on the repo or  [email me](mailto:benjaminchamwb@gmail.com).
 
 If you like my work, do consider supporting me so that i can dedicate more time and attention.
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E0NVBCJ)
```

### Comparing `freeoptionschain-0.0.2/setup.py` & `freeoptionschain-0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='freeoptionschain',
     
-    version='0.0.2',
+    version='0.01',
 
     description='This library module retrieves stock options data from NASDAQ.',
 
     long_description=long_description,
 
     long_description_content_type='text/markdown',
```


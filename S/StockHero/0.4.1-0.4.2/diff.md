# Comparing `tmp/StockHero-0.4.1.tar.gz` & `tmp/StockHero-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StockHero-0.4.1.tar", last modified: Wed Nov  2 16:16:44 2022, max compression
+gzip compressed data, was "StockHero-0.4.2.tar", last modified: Tue Aug  8 14:07:30 2023, max compression
```

## Comparing `StockHero-0.4.1.tar` & `StockHero-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 16:16:44.944296 StockHero-0.4.1/
--rw-rw-rw-   0        0        0    10729 2022-06-05 17:56:19.000000 StockHero-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     6737 2022-11-02 16:16:44.944296 StockHero-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6013 2022-11-01 14:05:38.000000 StockHero-0.4.1/README.md
--rw-rw-rw-   0        0        0      108 2021-09-09 14:56:17.000000 StockHero-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      707 2022-11-02 16:16:44.944296 StockHero-0.4.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-02 16:16:44.890434 StockHero-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2022-11-02 16:16:44.911368 StockHero-0.4.1/src/StockHero/
--rw-rw-rw-   0        0        0    26986 2022-08-26 08:41:13.000000 StockHero-0.4.1/src/StockHero/StockExchange.py
--rw-rw-rw-   0        0        0     4895 2022-08-26 08:41:18.000000 StockHero-0.4.1/src/StockHero/StockValuation.py
--rw-rw-rw-   0        0        0     1588 2022-08-29 19:02:29.000000 StockHero-0.4.1/src/StockHero/Ticker.py
-drwxrwxrwx   0        0        0        0 2022-11-02 16:16:44.944296 StockHero-0.4.1/src/StockHero/Ticker_Sources/
--rw-rw-rw-   0        0        0     2766 2022-08-26 07:59:09.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/GuruFocusRequest.py
--rw-rw-rw-   0        0        0    13572 2022-08-26 08:10:19.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/MorningStarRequest.py
--rw-rw-rw-   0        0        0    24854 2022-08-29 15:46:28.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/NASDAQRequest.py
--rw-rw-rw-   0        0        0      437 2022-08-26 07:55:09.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/TickerRequest.py
--rw-rw-rw-   0        0        0    42440 2022-10-26 09:42:33.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/TraderFoxRequest.py
--rw-rw-rw-   0        0        0    14446 2022-08-26 08:59:28.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/YahooRequest.py
--rw-rw-rw-   0        0        0        1 2022-07-06 06:39:05.000000 StockHero-0.4.1/src/StockHero/Ticker_Sources/__init__.py
--rw-rw-rw-   0        0        0      284 2022-07-04 13:35:58.000000 StockHero-0.4.1/src/StockHero/__init__.py
--rw-rw-rw-   0        0        0     2349 2022-11-02 16:02:53.000000 StockHero-0.4.1/src/StockHero/__version__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 16:16:44.937345 StockHero-0.4.1/src/StockHero.egg-info/
--rw-rw-rw-   0        0        0     6737 2022-11-02 16:16:44.000000 StockHero-0.4.1/src/StockHero.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2022-11-02 16:16:44.000000 StockHero-0.4.1/src/StockHero.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-02 16:16:44.000000 StockHero-0.4.1/src/StockHero.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-11-02 16:16:44.000000 StockHero-0.4.1/src/StockHero.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.350044 StockHero-0.4.2/
+-rw-rw-rw-   0        0        0    10729 2023-08-08 13:25:35.000000 StockHero-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     4653 2023-08-08 14:07:30.350545 StockHero-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4006 2023-08-08 13:55:38.000000 StockHero-0.4.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-09-09 14:56:17.000000 StockHero-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0      664 2023-08-08 14:07:30.351045 StockHero-0.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.311771 StockHero-0.4.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.328068 StockHero-0.4.2/src/StockHero/
+-rw-rw-rw-   0        0        0    26986 2022-08-26 08:41:13.000000 StockHero-0.4.2/src/StockHero/StockExchange.py
+-rw-rw-rw-   0        0        0     4895 2022-08-26 08:41:18.000000 StockHero-0.4.2/src/StockHero/StockValuation.py
+-rw-rw-rw-   0        0        0     1588 2022-08-29 19:02:29.000000 StockHero-0.4.2/src/StockHero/Ticker.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.347427 StockHero-0.4.2/src/StockHero/Ticker_Sources/
+-rw-rw-rw-   0        0        0     2766 2022-08-26 07:59:09.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/GuruFocusRequest.py
+-rw-rw-rw-   0        0        0    15960 2023-08-06 21:23:54.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/MorningStarRequest.py
+-rw-rw-rw-   0        0        0    24854 2022-08-29 15:46:28.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/NASDAQRequest.py
+-rw-rw-rw-   0        0        0      437 2022-08-26 07:55:09.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/TickerRequest.py
+-rw-rw-rw-   0        0        0    42440 2022-10-26 09:42:33.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/TraderFoxRequest.py
+-rw-rw-rw-   0        0        0    14446 2022-08-26 08:59:28.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/YahooRequest.py
+-rw-rw-rw-   0        0        0        1 2022-07-06 06:39:05.000000 StockHero-0.4.2/src/StockHero/Ticker_Sources/__init__.py
+-rw-rw-rw-   0        0        0      284 2022-07-04 13:35:58.000000 StockHero-0.4.2/src/StockHero/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-08-06 19:56:12.000000 StockHero-0.4.2/src/StockHero/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.335719 StockHero-0.4.2/src/StockHero.egg-info/
+-rw-rw-rw-   0        0        0     4653 2023-08-08 14:07:30.000000 StockHero-0.4.2/src/StockHero.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-08-08 14:07:30.000000 StockHero-0.4.2/src/StockHero.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 14:07:30.000000 StockHero-0.4.2/src/StockHero.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 14:07:30.000000 StockHero-0.4.2/src/StockHero.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 14:07:30.348873 StockHero-0.4.2/tests/
+-rw-rw-rw-   0        0        0     4652 2023-08-06 20:25:42.000000 StockHero-0.4.2/tests/test_all_ticker_requests.py
```

### Comparing `StockHero-0.4.1/LICENSE` & `StockHero-0.4.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-Copyright 2022 Robert Wenzel
+Copyright 2023 Robert Wenzel
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `StockHero-0.4.1/setup.cfg` & `StockHero-0.4.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 746f 636b 4865 726f 0d0a 7665   = StockHero..ve
-00000020: 7273 696f 6e20 3d20 302e 342e 310d 0a61  rsion = 0.4.1..a
+00000020: 7273 696f 6e20 3d20 302e 342e 320d 0a61  rsion = 0.4.2..a
 00000030: 7574 686f 7220 3d20 526f 6257 656e 0d0a  uthor = RobWen..
-00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2052  author_email = R
-00000050: 6f62 5765 6e2e 5374 6f63 6b48 6572 6f40  obWen.StockHero@
-00000060: 676d 6169 6c2e 636f 6d0d 0a6d 6169 6e74  gmail.com..maint
-00000070: 6169 6e65 7220 3d20 6173 7469 3230 350d  ainer = asti205.
-00000080: 0a64 6573 6372 6970 7469 6f6e 203d 204d  .description = M
-00000090: 6f72 6e69 6e67 7374 6172 2e63 6f6d 2c20  orningstar.com, 
-000000a0: 6669 6e61 6e63 652e 7961 686f 6f2e 636f  finance.yahoo.co
-000000b0: 6d20 616e 6420 4e61 7364 6171 2073 746f  m and Nasdaq sto
-000000c0: 636b 206d 6172 6b65 7420 6461 7461 2064  ck market data d
-000000d0: 6f77 6e6c 6f61 6465 720d 0a6c 6f6e 675f  ownloader..long_
-000000e0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000f0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000110: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000120: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000130: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-00000140: 7562 2e63 6f6d 2f52 6f62 5765 6e2f 5374  ub.com/RobWen/St
-00000150: 6f63 6b48 6572 6f0d 0a63 6c61 7373 6966  ockHero..classif
-00000160: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
-00000170: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000180: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
-00000190: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000001a0: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-000001b0: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-000001c0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-000001d0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000001e0: 7065 6e64 656e 740d 0a09 546f 7069 6320  pendent...Topic 
-000001f0: 3a3a 204f 6666 6963 652f 4275 7369 6e65  :: Office/Busine
-00000200: 7373 203a 3a20 4669 6e61 6e63 6961 6c20  ss :: Financial 
-00000210: 3a3a 2049 6e76 6573 746d 656e 740d 0a0d  :: Investment...
-00000220: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000230: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000240: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000250: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000260: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
-00000270: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000280: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000290: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002c0: 0a0d 0a                                  ...
+00000040: 6d61 696e 7461 696e 6572 203d 2061 7374  maintainer = ast
+00000050: 6932 3035 0d0a 6465 7363 7269 7074 696f  i205..descriptio
+00000060: 6e20 3d20 4d6f 726e 696e 6773 7461 722e  n = Morningstar.
+00000070: 636f 6d2c 2066 696e 616e 6365 2e79 6168  com, finance.yah
+00000080: 6f6f 2e63 6f6d 2061 6e64 204e 6173 6461  oo.com and Nasda
+00000090: 7120 7374 6f63 6b20 6d61 726b 6574 2064  q stock market d
+000000a0: 6174 6120 646f 776e 6c6f 6164 6572 0d0a  ata downloader..
+000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000c0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000d0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000e0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000000f0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000100: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+00000110: 2f67 6974 6875 622e 636f 6d2f 526f 6257  /github.com/RobW
+00000120: 656e 2f53 746f 636b 4865 726f 0d0a 636c  en/StockHero..cl
+00000130: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+00000140: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000150: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000160: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000170: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000180: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+00000190: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+000001a0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001b0: 2049 6e64 6570 656e 6465 6e74 0d0a 0954   Independent...T
+000001c0: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
+000001d0: 7573 696e 6573 7320 3a3a 2046 696e 616e  usiness :: Finan
+000001e0: 6369 616c 203a 3a20 496e 7665 7374 6d65  cial :: Investme
+000001f0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
+00000200: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000210: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+00000220: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000230: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000240: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
+00000250: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000260: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+00000270: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000280: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000290: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `StockHero-0.4.1/src/StockHero/StockExchange.py` & `StockHero-0.4.2/src/StockHero/StockExchange.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/StockValuation.py` & `StockHero-0.4.2/src/StockHero/StockValuation.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/Ticker.py` & `StockHero-0.4.2/src/StockHero/Ticker.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/Ticker_Sources/GuruFocusRequest.py` & `StockHero-0.4.2/src/StockHero/Ticker_Sources/GuruFocusRequest.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/Ticker_Sources/MorningStarRequest.py` & `StockHero-0.4.2/src/StockHero/Ticker_Sources/MorningStarRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
-Created on Fri Aug 26 09:55:42 2022
+Created on Fri Aug 06 22:46:42 2023
 
 @author: RobWen
-Version: 0.4.0
+Version: 0.4.2
 """
 
 # Packages
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 import numpy as np
@@ -27,14 +27,18 @@
     ################################
 
     @property
     def quote(self):
         return self.__morningstar_quote_abfrage()
 
     @property
+    def key_statistics(self):
+        return self.__morningstar_quote_abfrage_key_statistics()
+
+    @property
     def growth_rev(self):
         return self.__morningstar_quote_abfrage_growth_revenue()
     
     @property
     def growth_op_inc(self):
         return self.__morningstar_quote_abfrage_operating_income()
     
@@ -48,15 +52,15 @@
     
     ##########################
     ###                    ###
     ###  Morningstar Data  ###
     ###                    ###
     ##########################
     
-    # Dummy Abfrage
+    # Dummy Abfragen, um Fehler im Vorfeld abzufangen
     def __morningstar_quote_abfrage(self):
         
         ' Dummy Abfrage'
         if self.ticker is None or self.ticker == '':
             self.ticker = 'None'
             return None
         
@@ -145,15 +149,24 @@
                                         , 'ROE % TTM', 'Current Free Cash Flow']
                               , columns =[self.ticker + ' Ratio'])
             
             df_morningstar_quote = df_morningstar_quote.fillna(value=np.nan) # None mit NaN ersetzen für df
         
         return df_morningstar_quote
     
-    # Dummy Abfragen
+    # Dummy Abfragen, um Fehler im Vorfeld abzufangen
+    
+    def __morningstar_quote_abfrage_key_statistics(self):
+        
+        if self.ticker is None or self.ticker == '':
+            self.ticker = 'None'
+            return None
+        
+        return self.__morningstar_key_statistics_df()
+    
     def __morningstar_quote_abfrage_growth_revenue(self):
         
         if self.ticker is None or self.ticker == '':
             self.ticker = 'None'
             return None
         
         return self.__morningstar_growth_revenue_df()
@@ -178,14 +191,36 @@
         
         if self.ticker is None or self.ticker == '':
             self.ticker = 'None'
             return None
         
         return self.__morningstar_growth_eps_df()
     
+    # Eigentlichen Abfragen
+    
+    # Wird zur Generierung der Key Statistics verwendet
+    def __initialize_dataframe(self, columns, index):
+        df = pd.DataFrame([[''] * len(columns)], columns=columns, index=index)
+        return df
+    
+    def __morningstar_key_statistics_df(self):
+        
+        df1 = self.__morningstar_quote_abfrage_growth_revenue()
+        df2 = self.__morningstar_quote_abfrage_operating_income()
+        df3 = self.__morningstar_quote_abfrage_net_income()
+        df4 = self.__morningstar_quote_abfrage_growth_eps()
+        
+        df1_1 = self.__initialize_dataframe(df1.columns, ['Growth Revenue %'])
+        df2_1 = self.__initialize_dataframe(df2.columns, ['Operating Income %'])
+        df3_1 = self.__initialize_dataframe(df3.columns, ['Net Income %'])
+        df4_1 = self.__initialize_dataframe(df4.columns, ['EPS %'])
+        
+        morningstar_key_statistics_df = pd.concat([df1_1, df1, df2_1, df2 ,df3_1, df3, df4_1, df4], axis=0)
+        return morningstar_key_statistics_df
+    
     def __morningstar_growth_revenue_df(self):
         morningstar_performance_id = self.__morningstar_performance_id()
         
         if morningstar_performance_id is None:
             return None
         else:
             url = f'https://api-global.morningstar.com/sal-service/v1/stock/keyStats/growthTable/{morningstar_performance_id}?languageId=en&locale=en&clientId=undefined&component=sal-components-key-stats-growth-table&version=3.71.0'
@@ -208,15 +243,18 @@
             array_table = np.array(liste_values).transpose()
             
             morningstar_growth_revenue_df = pd.DataFrame(array_table
                                , index =['Year over Year', '3-Year Average', '5-Year Average', '10-Year Average']
                                , columns = columns
                                )
             
-            morningstar_growth_revenue_df = morningstar_growth_revenue_df.fillna(value=np.nan)
+            # Leere Zellen mit NaN auffüllen
+            # Werte auf die 2te Nachkommastelle runden
+            # Wie bei Morningstar dargestellt, ansonsten gibt es beim späteren Umwandeln in Markdown Probleme
+            morningstar_growth_revenue_df = morningstar_growth_revenue_df.fillna(value=np.nan).round(2)
         
         return morningstar_growth_revenue_df
     
     def __morningstar_operating_income_df(self):
         morningstar_performance_id = self.__morningstar_performance_id()
         
         if morningstar_performance_id is None:
@@ -242,15 +280,18 @@
             array_table = np.array(liste_values).transpose()
             
             morningstar_operating_income_df = pd.DataFrame(array_table
                                , index =['Year over Year', '3-Year Average', '5-Year Average', '10-Year Average']
                                , columns = columns
                                )
             
-            morningstar_operating_income_df = morningstar_operating_income_df.fillna(value=np.nan)
+            # Leere Zellen mit NaN auffüllen
+            # Werte auf die 2te Nachkommastelle runden
+            # Wie bei Morningstar dargestellt, ansonsten gibt es beim späteren Umwandeln in Markdown Probleme
+            morningstar_operating_income_df = morningstar_operating_income_df.fillna(value=np.nan).round(2)
         
         return morningstar_operating_income_df
     
     def __morningstar_net_income_df(self):
         morningstar_performance_id = self.__morningstar_performance_id()
         
         if morningstar_performance_id is None:
@@ -276,15 +317,18 @@
             array_table = np.array(liste_values).transpose()
             
             morningstar_net_income_df = pd.DataFrame(array_table
                                , index =['Year over Year', '3-Year Average', '5-Year Average', '10-Year Average']
                                , columns = columns
                                )
             
-            morningstar_net_income_df = morningstar_net_income_df.fillna(value=np.nan)
+            # Leere Zellen mit NaN auffüllen
+            # Werte auf die 2te Nachkommastelle runden
+            # Wie bei Morningstar dargestellt, ansonsten gibt es beim späteren Umwandeln in Markdown Probleme
+            morningstar_net_income_df = morningstar_net_income_df.fillna(value=np.nan).round(2)
         
         return morningstar_net_income_df
     
     def __morningstar_growth_eps_df(self):
         morningstar_performance_id = self.__morningstar_performance_id()
         
         if morningstar_performance_id is None:
@@ -310,10 +354,13 @@
             array_table = np.array(liste_values).transpose()
             
             morningstar_growth_eps_df = pd.DataFrame(array_table
                                , index =['Year over Year', '3-Year Average', '5-Year Average', '10-Year Average']
                                , columns = columns
                                )
             
-            morningstar_growth_eps_df = morningstar_growth_eps_df.fillna(value=np.nan)
+            # Leere Zellen mit NaN auffüllen
+            # Werte auf die 2te Nachkommastelle runden
+            # Wie bei Morningstar dargestellt, ansonsten gibt es beim späteren Umwandeln in Markdown Probleme
+            morningstar_growth_eps_df = morningstar_growth_eps_df.fillna(value=np.nan).round(2)
         
         return morningstar_growth_eps_df
```

### Comparing `StockHero-0.4.1/src/StockHero/Ticker_Sources/NASDAQRequest.py` & `StockHero-0.4.2/src/StockHero/Ticker_Sources/NASDAQRequest.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/Ticker_Sources/TraderFoxRequest.py` & `StockHero-0.4.2/src/StockHero/Ticker_Sources/TraderFoxRequest.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/Ticker_Sources/YahooRequest.py` & `StockHero-0.4.2/src/StockHero/Ticker_Sources/YahooRequest.py`

 * *Files identical despite different names*

### Comparing `StockHero-0.4.1/src/StockHero/__version__.py` & `StockHero-0.4.2/src/StockHero/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,28 @@
 #|  \__| $$  | $$|  \| $$__/ $$| $$_____ | $$$$$$\ | $$  | $$| $$$$$$$$| $$      | $$__/ $$
 # \$$    $$   \$$  $$ \$$    $$ \$$     \| $$  \$$\| $$  | $$ \$$     \| $$       \$$    $$
 #  \$$$$$$     \$$$$   \$$$$$$   \$$$$$$$ \$$   \$$ \$$   \$$  \$$$$$$$ \$$        \$$$$$$ 
 
 __title__ = 'StockHero'
 __description__ = 'stock market data downloader'
 __url__ = 'https://github.com/RobWen/StockHero'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = 'RobWen'
 __author_email__ = 'RobWen.StockHero@gmail.com'
 __license__ = 'Apache 2.0'
-__copyright__ = 'Copyright 2022'
+__copyright__ = 'Copyright 2023'
 __thanks__ = 'Thanks to my colleagues @Fraunhofer IIS'
 
 '''
 Release History
+0.4.2 (xx.08.2023)
+    - minor fixes morningstar
+
+0.4.1 (02.11.2022)
+    - added Traderfox
 
 0.4.0 (26.08.2022)
     - introducing a new architecture (again ^^)
 
 0.3.3 (06.07.2022)
     - Some Morningstar Features are up and running again
     - Morningstar is now also working with ISIN
```

### Comparing `StockHero-0.4.1/src/StockHero.egg-info/SOURCES.txt` & `StockHero-0.4.2/src/StockHero.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/StockHero.egg-info/top_level.txt
 src/StockHero/Ticker_Sources/GuruFocusRequest.py
 src/StockHero/Ticker_Sources/MorningStarRequest.py
 src/StockHero/Ticker_Sources/NASDAQRequest.py
 src/StockHero/Ticker_Sources/TickerRequest.py
 src/StockHero/Ticker_Sources/TraderFoxRequest.py
 src/StockHero/Ticker_Sources/YahooRequest.py
-src/StockHero/Ticker_Sources/__init__.py
+src/StockHero/Ticker_Sources/__init__.py
+tests/test_all_ticker_requests.py
```


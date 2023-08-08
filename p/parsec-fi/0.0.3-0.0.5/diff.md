# Comparing `tmp/parsec_fi-0.0.3.tar.gz` & `tmp/parsec_fi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsec_fi-0.0.3.tar", last modified: Tue Aug  8 01:53:02 2023, max compression
+gzip compressed data, was "parsec_fi-0.0.5.tar", last modified: Tue Aug  8 18:46:44 2023, max compression
```

## Comparing `parsec_fi-0.0.3.tar` & `parsec_fi-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 01:53:02.114570 parsec_fi-0.0.3/
--rw-r--r--   0 wilburforce   (501) staff       (20)      180 2023-08-08 01:53:02.114412 parsec_fi-0.0.3/PKG-INFO
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 01:53:02.108911 parsec_fi-0.0.3/lib/
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:38:30.000000 parsec_fi-0.0.3/lib/__init__.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      354 2023-08-07 17:39:28.000000 parsec_fi-0.0.3/lib/endpoints.py
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 01:53:02.113368 parsec_fi-0.0.3/lib/endpoints_list/
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:41:41.000000 parsec_fi-0.0.3/lib/endpoints_list/__init__.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      445 2023-08-07 19:03:39.000000 parsec_fi-0.0.3/lib/endpoints_list/candles.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      707 2023-08-07 18:02:37.000000 parsec_fi-0.0.3/lib/endpoints_list/conc_liquidity_positions.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      619 2023-08-02 00:34:13.000000 parsec_fi-0.0.3/lib/endpoints_list/contract_logs.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      577 2023-08-08 00:45:47.000000 parsec_fi-0.0.3/lib/endpoints_list/dex_trades.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      565 2023-08-02 01:08:59.000000 parsec_fi-0.0.3/lib/endpoints_list/lending_market.py
--rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-08-02 01:05:27.000000 parsec_fi-0.0.3/lib/endpoints_list/lending_positions.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      643 2023-08-07 17:54:50.000000 parsec_fi-0.0.3/lib/endpoints_list/liquidity_pools.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      435 2023-08-08 00:34:08.000000 parsec_fi-0.0.3/lib/endpoints_list/nft_collection.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      649 2023-08-08 00:34:06.000000 parsec_fi-0.0.3/lib/endpoints_list/nft_trades.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-02 01:04:23.000000 parsec_fi-0.0.3/lib/endpoints_list/token_acc.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      468 2023-08-02 01:01:34.000000 parsec_fi-0.0.3/lib/endpoints_list/token_holders.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      789 2023-08-07 17:35:20.000000 parsec_fi-0.0.3/lib/endpoints_list/transfers.py
--rw-r--r--   0 wilburforce   (501) staff       (20)      725 2023-08-02 20:13:48.000000 parsec_fi-0.0.3/lib/endpoints_list/trending_contracts.py
-drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 01:53:02.114165 parsec_fi-0.0.3/parsec_fi.egg-info/
--rw-r--r--   0 wilburforce   (501) staff       (20)      180 2023-08-08 01:53:02.000000 parsec_fi-0.0.3/parsec_fi.egg-info/PKG-INFO
--rw-r--r--   0 wilburforce   (501) staff       (20)      676 2023-08-08 01:53:02.000000 parsec_fi-0.0.3/parsec_fi.egg-info/SOURCES.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)        1 2023-08-08 01:53:02.000000 parsec_fi-0.0.3/parsec_fi.egg-info/dependency_links.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)        4 2023-08-08 01:53:02.000000 parsec_fi-0.0.3/parsec_fi.egg-info/top_level.txt
--rw-r--r--   0 wilburforce   (501) staff       (20)       38 2023-08-08 01:53:02.114631 parsec_fi-0.0.3/setup.cfg
--rw-r--r--   0 wilburforce   (501) staff       (20)      227 2023-08-08 01:52:50.000000 parsec_fi-0.0.3/setup.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 18:46:44.426900 parsec_fi-0.0.5/
+-rw-r--r--   0 wilburforce   (501) staff       (20)      180 2023-08-08 18:46:44.426771 parsec_fi-0.0.5/PKG-INFO
+-rw-r--r--   0 wilburforce   (501) staff       (20)       10 2023-08-08 18:42:49.000000 parsec_fi-0.0.5/README.md
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 18:46:44.422042 parsec_fi-0.0.5/lib/
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:38:30.000000 parsec_fi-0.0.5/lib/__init__.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      354 2023-08-07 17:39:28.000000 parsec_fi-0.0.5/lib/endpoints.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 18:46:44.425794 parsec_fi-0.0.5/lib/endpoints_list/
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-05-22 23:41:41.000000 parsec_fi-0.0.5/lib/endpoints_list/__init__.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      445 2023-08-07 19:03:39.000000 parsec_fi-0.0.5/lib/endpoints_list/candles.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      707 2023-08-07 18:02:37.000000 parsec_fi-0.0.5/lib/endpoints_list/conc_liquidity_positions.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      619 2023-08-02 00:34:13.000000 parsec_fi-0.0.5/lib/endpoints_list/contract_logs.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      577 2023-08-08 00:45:47.000000 parsec_fi-0.0.5/lib/endpoints_list/dex_trades.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      565 2023-08-02 01:08:59.000000 parsec_fi-0.0.5/lib/endpoints_list/lending_market.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)        0 2023-08-02 01:05:27.000000 parsec_fi-0.0.5/lib/endpoints_list/lending_positions.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      643 2023-08-07 17:54:50.000000 parsec_fi-0.0.5/lib/endpoints_list/liquidity_pools.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      435 2023-08-08 00:34:08.000000 parsec_fi-0.0.5/lib/endpoints_list/nft_collection.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      649 2023-08-08 00:34:06.000000 parsec_fi-0.0.5/lib/endpoints_list/nft_trades.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      663 2023-08-02 01:04:23.000000 parsec_fi-0.0.5/lib/endpoints_list/token_acc.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      468 2023-08-02 01:01:34.000000 parsec_fi-0.0.5/lib/endpoints_list/token_holders.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      789 2023-08-07 17:35:20.000000 parsec_fi-0.0.5/lib/endpoints_list/transfers.py
+-rw-r--r--   0 wilburforce   (501) staff       (20)      725 2023-08-02 20:13:48.000000 parsec_fi-0.0.5/lib/endpoints_list/trending_contracts.py
+drwxr-xr-x   0 wilburforce   (501) staff       (20)        0 2023-08-08 18:46:44.426581 parsec_fi-0.0.5/parsec_fi.egg-info/
+-rw-r--r--   0 wilburforce   (501) staff       (20)      180 2023-08-08 18:46:44.000000 parsec_fi-0.0.5/parsec_fi.egg-info/PKG-INFO
+-rw-r--r--   0 wilburforce   (501) staff       (20)      718 2023-08-08 18:46:44.000000 parsec_fi-0.0.5/parsec_fi.egg-info/SOURCES.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)        1 2023-08-08 18:46:44.000000 parsec_fi-0.0.5/parsec_fi.egg-info/dependency_links.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)       16 2023-08-08 18:46:44.000000 parsec_fi-0.0.5/parsec_fi.egg-info/requires.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)        4 2023-08-08 18:46:44.000000 parsec_fi-0.0.5/parsec_fi.egg-info/top_level.txt
+-rw-r--r--   0 wilburforce   (501) staff       (20)       38 2023-08-08 18:46:44.426946 parsec_fi-0.0.5/setup.cfg
+-rw-r--r--   0 wilburforce   (501) staff       (20)      294 2023-08-08 18:45:18.000000 parsec_fi-0.0.5/setup.py
```

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/conc_liquidity_positions.py` & `parsec_fi-0.0.5/lib/endpoints_list/conc_liquidity_positions.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/contract_logs.py` & `parsec_fi-0.0.5/lib/endpoints_list/contract_logs.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/dex_trades.py` & `parsec_fi-0.0.5/lib/endpoints_list/dex_trades.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/lending_market.py` & `parsec_fi-0.0.5/lib/endpoints_list/lending_market.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/liquidity_pools.py` & `parsec_fi-0.0.5/lib/endpoints_list/liquidity_pools.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/nft_trades.py` & `parsec_fi-0.0.5/lib/endpoints_list/nft_trades.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/token_acc.py` & `parsec_fi-0.0.5/lib/endpoints_list/token_acc.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/transfers.py` & `parsec_fi-0.0.5/lib/endpoints_list/transfers.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/lib/endpoints_list/trending_contracts.py` & `parsec_fi-0.0.5/lib/endpoints_list/trending_contracts.py`

 * *Files identical despite different names*

### Comparing `parsec_fi-0.0.3/parsec_fi.egg-info/SOURCES.txt` & `parsec_fi-0.0.5/parsec_fi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 lib/__init__.py
 lib/endpoints.py
 lib/endpoints_list/__init__.py
 lib/endpoints_list/candles.py
 lib/endpoints_list/conc_liquidity_positions.py
 lib/endpoints_list/contract_logs.py
@@ -14,8 +15,9 @@
 lib/endpoints_list/token_acc.py
 lib/endpoints_list/token_holders.py
 lib/endpoints_list/transfers.py
 lib/endpoints_list/trending_contracts.py
 parsec_fi.egg-info/PKG-INFO
 parsec_fi.egg-info/SOURCES.txt
 parsec_fi.egg-info/dependency_links.txt
+parsec_fi.egg-info/requires.txt
 parsec_fi.egg-info/top_level.txt
```


# Comparing `tmp/vtex-0.1.4.tar.gz` & `tmp/vtex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vtex-0.1.4.tar", last modified: Sun Oct  4 01:38:31 2020, max compression
+gzip compressed data, was "vtex-0.2.0.tar", last modified: Tue Aug  8 15:01:51 2023, max compression
```

## Comparing `vtex-0.1.4.tar` & `vtex-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/
--rw-r--r--   0 Meili      (501) staff       (20)      919 2020-10-04 01:38:31.000000 vtex-0.1.4/PKG-INFO
--rw-r--r--   0 Meili      (501) staff       (20)      477 2019-12-22 01:13:26.000000 vtex-0.1.4/README.md
--rw-r--r--   0 Meili      (501) staff       (20)       38 2020-10-04 01:38:31.000000 vtex-0.1.4/setup.cfg
--rw-r--r--   0 Meili      (501) staff       (20)      556 2020-10-04 01:37:58.000000 vtex-0.1.4/setup.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/tests/
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-26 01:27:03.000000 vtex-0.1.4/tests/__init__.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/tests/integration_tests/
--rw-r--r--   0 Meili      (501) staff       (20)      516 2019-12-01 13:07:59.000000 vtex-0.1.4/tests/integration_tests/__init__.py
--rw-r--r--   0 Meili      (501) staff       (20)     1837 2019-11-29 02:04:06.000000 vtex-0.1.4/tests/integration_tests/test_catalog_endpoint.py
--rw-r--r--   0 Meili      (501) staff       (20)     2811 2019-12-01 11:51:07.000000 vtex-0.1.4/tests/integration_tests/test_gift_card_endpoint.py
--rw-r--r--   0 Meili      (501) staff       (20)     1879 2020-10-04 01:30:34.000000 vtex-0.1.4/tests/integration_tests/test_master_data_endpoint.py
--rw-r--r--   0 Meili      (501) staff       (20)     1667 2020-07-30 11:05:33.000000 vtex-0.1.4/tests/integration_tests/test_order_management_endpoint.py
--rw-r--r--   0 Meili      (501) staff       (20)     1039 2019-12-01 12:32:56.000000 vtex-0.1.4/tests/integration_tests/test_payments_gateway_endpoint.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/tests/unit_tests/
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-29 01:35:15.000000 vtex-0.1.4/tests/unit_tests/__init__.py
--rw-r--r--   0 Meili      (501) staff       (20)      226 2019-11-26 01:37:19.000000 vtex-0.1.4/tests/unit_tests/test_imports.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex/
--rw-r--r--   0 Meili      (501) staff       (20)       54 2019-12-03 01:53:21.000000 vtex-0.1.4/vtex/__init__.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex/api_collections/
--rw-r--r--   0 Meili      (501) staff       (20)      240 2019-12-03 01:50:20.000000 vtex-0.1.4/vtex/api_collections/__init__.py
--rw-r--r--   0 Meili      (501) staff       (20)     1304 2019-12-03 03:08:52.000000 vtex-0.1.4/vtex/api_collections/base_api.py
--rw-r--r--   0 Meili      (501) staff       (20)     2026 2019-12-03 03:09:23.000000 vtex-0.1.4/vtex/api_collections/catalog.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:55:22.000000 vtex-0.1.4/vtex/api_collections/checkout.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-12-11 23:54:34.000000 vtex-0.1.4/vtex/api_collections/customer_credit.py
--rw-r--r--   0 Meili      (501) staff       (20)     4260 2019-12-03 03:12:25.000000 vtex-0.1.4/vtex/api_collections/gift_card.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:56:17.000000 vtex-0.1.4/vtex/api_collections/license_manager.py
--rw-r--r--   0 Meili      (501) staff       (20)      940 2019-12-03 03:11:49.000000 vtex-0.1.4/vtex/api_collections/logistics.py
--rw-r--r--   0 Meili      (501) staff       (20)     1710 2020-10-04 01:30:34.000000 vtex-0.1.4/vtex/api_collections/master_data.py
--rw-r--r--   0 Meili      (501) staff       (20)     6066 2020-07-30 11:05:33.000000 vtex-0.1.4/vtex/api_collections/order_management.py
--rw-r--r--   0 Meili      (501) staff       (20)      956 2019-12-03 03:04:34.000000 vtex-0.1.4/vtex/api_collections/payments_gateway.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:57:30.000000 vtex-0.1.4/vtex/api_collections/pricing_vault.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:57:43.000000 vtex-0.1.4/vtex/api_collections/rates_and_benefits.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:57:51.000000 vtex-0.1.4/vtex/api_collections/search.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:58:01.000000 vtex-0.1.4/vtex/api_collections/session_manager.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:58:12.000000 vtex-0.1.4/vtex/api_collections/subscriptions.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:58:23.000000 vtex-0.1.4/vtex/api_collections/suggestion.py
--rw-r--r--   0 Meili      (501) staff       (20)        0 2019-11-27 23:58:34.000000 vtex-0.1.4/vtex/api_collections/vtex_do.py
--rw-r--r--   0 Meili      (501) staff       (20)     2600 2019-12-03 02:13:51.000000 vtex-0.1.4/vtex/vtex.py
-drwxr-xr-x   0 Meili      (501) staff       (20)        0 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/
--rw-r--r--   0 Meili      (501) staff       (20)      919 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/PKG-INFO
--rw-r--r--   0 Meili      (501) staff       (20)     1226 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/SOURCES.txt
--rw-r--r--   0 Meili      (501) staff       (20)        1 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/dependency_links.txt
--rw-r--r--   0 Meili      (501) staff       (20)        9 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/requires.txt
--rw-r--r--   0 Meili      (501) staff       (20)       11 2020-10-04 01:38:31.000000 vtex-0.1.4/vtex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.252877 vtex-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 15:01:41.000000 vtex-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 15:01:51.248877 vtex-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 15:01:41.000000 vtex-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:01:51.252877 vtex-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-08 15:01:41.000000 vtex-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.244877 vtex-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.248877 vtex-0.2.0/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/test_catalog_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/test_gift_card_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/test_master_data_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/test_order_management_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/integration_tests/test_payments_gateway_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.248877 vtex-0.2.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 15:01:41.000000 vtex-0.2.0/tests/unit_tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.248877 vtex-0.2.0/vtex/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.248877 vtex-0.2.0/vtex/api_collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/customer_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/license_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/logistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/master_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/order_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/payments_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/pricing_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/rates_and_benefits.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/api_collections/vtex_do.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-08-08 15:01:41.000000 vtex-0.2.0/vtex/vtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:01:51.248877 vtex-0.2.0/vtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 15:01:51.000000 vtex-0.2.0/vtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 15:01:51.000000 vtex-0.2.0/vtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:01:51.000000 vtex-0.2.0/vtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 15:01:51.000000 vtex-0.2.0/vtex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 15:01:51.000000 vtex-0.2.0/vtex.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vtex-0.1.4/PKG-INFO` & `vtex-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: vtex
-Version: 0.1.4
+Version: 0.2.0
 Summary: VTEX API Wrapper for Python
 Home-page: https://github.com/lmeilibr/vtex
 Author: Leandro Meili
 Author-email: leandro.meili@gmail.com
 License: MIT
-Description: ![](https://github.com/lmeilibr/vtex/workflows/Python%20package/badge.svg)
-        
-        # VTEX
-        VTEX API Wrapper for Python
-        
-        # Example code
-        
-        You just need to pass your credentials to the Vtex instance,
-        and fetch the endpoints.
-        
-        ```python
-        from vtex import Vtex
-        
-        client = Vtex(account_name, environment, app_key, app_token)
-        result = client.logistics.get_all_carriers()
-        js = result.json
-        status_code = result.status_code
-        ```
-        result will be the json response from the get_all_carriers request
-        
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![](https://github.com/lmeilibr/vtex/workflows/Python%20package/badge.svg)
+
+# VTEX
+VTEX API Wrapper for Python
+
+# Example code
+
+You just need to pass your credentials to the Vtex instance,
+and fetch the endpoints.
+
+```python
+from vtex import Vtex
+
+client = Vtex(account_name, environment, app_key, app_token)
+result = client.logistics.get_all_carriers()
+js = result.json
+status_code = result.status_code
+```
+result will be the json response from the get_all_carriers request
+
+
```

### Comparing `vtex-0.1.4/setup.py` & `vtex-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from codecs import open
 
 with open('README.md', 'r', 'utf-8') as f:
     readme = f.read()
 
 setup(
     name='vtex',
-    version='0.1.4',
+    version='0.2.0',
     license="MIT",
     description='VTEX API Wrapper for Python',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Leandro Meili',
     author_email='leandro.meili@gmail.com',
     url='https://github.com/lmeilibr/vtex',
```

### Comparing `vtex-0.1.4/tests/integration_tests/__init__.py` & `vtex-0.2.0/tests/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/tests/integration_tests/test_catalog_endpoint.py` & `vtex-0.2.0/tests/integration_tests/test_catalog_endpoint.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/tests/integration_tests/test_gift_card_endpoint.py` & `vtex-0.2.0/tests/integration_tests/test_gift_card_endpoint.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/tests/integration_tests/test_master_data_endpoint.py` & `vtex-0.2.0/tests/integration_tests/test_master_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/tests/integration_tests/test_order_management_endpoint.py` & `vtex-0.2.0/tests/integration_tests/test_order_management_endpoint.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/tests/integration_tests/test_payments_gateway_endpoint.py` & `vtex-0.2.0/tests/integration_tests/test_payments_gateway_endpoint.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/base_api.py` & `vtex-0.2.0/vtex/api_collections/base_api.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/catalog.py` & `vtex-0.2.0/vtex/api_collections/catalog.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/gift_card.py` & `vtex-0.2.0/vtex/api_collections/gift_card.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/logistics.py` & `vtex-0.2.0/vtex/api_collections/logistics.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/master_data.py` & `vtex-0.2.0/vtex/api_collections/master_data.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/order_management.py` & `vtex-0.2.0/vtex/api_collections/order_management.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/api_collections/payments_gateway.py` & `vtex-0.2.0/vtex/api_collections/payments_gateway.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex/vtex.py` & `vtex-0.2.0/vtex/vtex.py`

 * *Files identical despite different names*

### Comparing `vtex-0.1.4/vtex.egg-info/PKG-INFO` & `vtex-0.2.0/vtex.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: vtex
-Version: 0.1.4
+Version: 0.2.0
 Summary: VTEX API Wrapper for Python
 Home-page: https://github.com/lmeilibr/vtex
 Author: Leandro Meili
 Author-email: leandro.meili@gmail.com
 License: MIT
-Description: ![](https://github.com/lmeilibr/vtex/workflows/Python%20package/badge.svg)
-        
-        # VTEX
-        VTEX API Wrapper for Python
-        
-        # Example code
-        
-        You just need to pass your credentials to the Vtex instance,
-        and fetch the endpoints.
-        
-        ```python
-        from vtex import Vtex
-        
-        client = Vtex(account_name, environment, app_key, app_token)
-        result = client.logistics.get_all_carriers()
-        js = result.json
-        status_code = result.status_code
-        ```
-        result will be the json response from the get_all_carriers request
-        
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![](https://github.com/lmeilibr/vtex/workflows/Python%20package/badge.svg)
+
+# VTEX
+VTEX API Wrapper for Python
+
+# Example code
+
+You just need to pass your credentials to the Vtex instance,
+and fetch the endpoints.
+
+```python
+from vtex import Vtex
+
+client = Vtex(account_name, environment, app_key, app_token)
+result = client.logistics.get_all_carriers()
+js = result.json
+status_code = result.status_code
+```
+result will be the json response from the get_all_carriers request
+
+
```

### Comparing `vtex-0.1.4/vtex.egg-info/SOURCES.txt` & `vtex-0.2.0/vtex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/integration_tests/__init__.py
 tests/integration_tests/test_catalog_endpoint.py
 tests/integration_tests/test_gift_card_endpoint.py
 tests/integration_tests/test_master_data_endpoint.py
```


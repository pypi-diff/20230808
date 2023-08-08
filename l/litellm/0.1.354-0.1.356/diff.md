# Comparing `tmp/litellm-0.1.354.tar.gz` & `tmp/litellm-0.1.356.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.354.tar", max compression
+gzip compressed data, was "litellm-0.1.356.tar", max compression
```

## Comparing `litellm-0.1.354.tar` & `litellm-0.1.356.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-07 19:09:15.501245 litellm-0.1.354/LICENSE
--rw-r--r--   0        0        0     2617 2023-08-07 19:09:15.501245 litellm-0.1.354/README.md
--rw-r--r--   0        0        0     6148 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/.DS_Store
--rw-r--r--   0        0        0     2134 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3548 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    14054 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2578 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4537 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5938 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/timeout.py
--rw-r--r--   0        0        0    23931 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-07 19:09:15.505245 litellm-0.1.354/pyproject.toml
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.354/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 04:36:01.540553 litellm-0.1.356/LICENSE
+-rw-r--r--   0        0        0     2617 2023-08-08 04:36:01.540553 litellm-0.1.356/README.md
+-rw-r--r--   0        0        0     6148 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/.DS_Store
+-rw-r--r--   0        0        0     2134 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    14054 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4537 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5938 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/timeout.py
+-rw-r--r--   0        0        0    23942 2023-08-08 04:36:01.544553 litellm-0.1.356/litellm/utils.py
+-rw-r--r--   0        0        0      532 2023-08-08 04:36:01.544553 litellm-0.1.356/pyproject.toml
+-rw-r--r--   0        0        0     3514 1970-01-01 00:00:00.000000 litellm-0.1.356/PKG-INFO
```

### Comparing `litellm-0.1.354/LICENSE` & `litellm-0.1.356/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/README.md` & `litellm-0.1.356/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/.DS_Store` & `litellm-0.1.356/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/__init__.py` & `litellm-0.1.356/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.356/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.356/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.356/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.356/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/aispend.py` & `litellm-0.1.356/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/berrispend.py` & `litellm-0.1.356/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/helicone.py` & `litellm-0.1.356/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/integrations/supabase.py` & `litellm-0.1.356/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/main.py` & `litellm-0.1.356/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.356/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_api_key_param.py` & `litellm-0.1.356/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_async_fn.py` & `litellm-0.1.356/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_bad_params.py` & `litellm-0.1.356/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.356/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_client.py` & `litellm-0.1.356/litellm/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 def test_bad_azure_embedding():
     try:
         response = embedding(model='chatgpt-test', input=[user_message], logger_fn=logger_fn)
         # Add any assertions here to check the response
         print(f"response: {str(response)[:50]}")
     except Exception as e:
         pass
-def test_good_azure_embedding():
-    try:
-        response = embedding(model='azure-embedding-model', input=[user_message], azure=True, logger_fn=logger_fn)
-        # Add any assertions here to check the response
-        print(f"response: {str(response)[:50]}")
-    except Exception as e:
-        pytest.fail(f"Error occurred: {e}")
+# def test_good_azure_embedding():
+#     try:
+#         response = embedding(model='azure-embedding-model', input=[user_message], azure=True, logger_fn=logger_fn)
+#         # Add any assertions here to check the response
+#         print(f"response: {str(response)[:50]}")
+#     except Exception as e:
+#         pytest.fail(f"Error occurred: {e}")
```

### Comparing `litellm-0.1.354/litellm/tests/test_completion.py` & `litellm-0.1.356/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_exceptions.py` & `litellm-0.1.356/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_helicone_integration.py` & `litellm-0.1.356/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_logging.py` & `litellm-0.1.356/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_model_fallback.py` & `litellm-0.1.356/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_no_client.py` & `litellm-0.1.356/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_secrets.py` & `litellm-0.1.356/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_supabase_integration.py` & `litellm-0.1.356/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/tests/test_timeout.py` & `litellm-0.1.356/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/timeout.py` & `litellm-0.1.356/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.354/litellm/utils.py` & `litellm-0.1.356/litellm/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import dotenv, json, traceback, threading
 import subprocess, os 
 import litellm, openai 
 import random, uuid, requests
 import datetime, time
 from anthropic import Anthropic
 import tiktoken
```

### Comparing `litellm-0.1.354/pyproject.toml` & `litellm-0.1.356/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.354"
+version = "0.1.356"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 openai = {extras = ["datalib"], version = "^0.27.8"}
 cohere = "^4.18.0"
 pytest = "^7.4.0"
+pydantic = "^2.1.1"
 anthropic = "^0.3.7"
 replicate = "^0.10.0"
 python-dotenv = "^1.0.0"
 tenacity = "^8.0.1"
 tiktoken = "^0.4.0"
 
 [build-system]
```

### Comparing `litellm-0.1.354/PKG-INFO` & `litellm-0.1.356/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.354
+Version: 0.1.356
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.3.7,<0.4.0)
 Requires-Dist: cohere (>=4.18.0,<5.0.0)
 Requires-Dist: openai[datalib] (>=0.27.8,<0.28.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: replicate (>=0.10.0,<0.11.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
```


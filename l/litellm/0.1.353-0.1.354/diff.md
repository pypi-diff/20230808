# Comparing `tmp/litellm-0.1.353.tar.gz` & `tmp/litellm-0.1.354.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.353.tar", max compression
+gzip compressed data, was "litellm-0.1.354.tar", max compression
```

## Comparing `litellm-0.1.353.tar` & `litellm-0.1.354.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1065 2023-08-07 18:33:49.640112 litellm-0.1.353/LICENSE
--rw-r--r--   0        0        0     2617 2023-08-07 18:33:49.640112 litellm-0.1.353/README.md
--rw-r--r--   0        0        0     6148 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/.DS_Store
--rw-r--r--   0        0        0     2134 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3548 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    14057 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0      920 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2578 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4537 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_completion.py
--rw-r--r--   0        0        0     5938 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-07 18:33:49.644112 litellm-0.1.353/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-07 18:33:49.648113 litellm-0.1.353/litellm/timeout.py
--rw-r--r--   0        0        0    23684 2023-08-07 18:33:49.648113 litellm-0.1.353/litellm/utils.py
--rw-r--r--   0        0        0      512 2023-08-07 18:33:49.648113 litellm-0.1.353/pyproject.toml
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.353/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-07 19:09:15.501245 litellm-0.1.354/LICENSE
+-rw-r--r--   0        0        0     2617 2023-08-07 19:09:15.501245 litellm-0.1.354/README.md
+-rw-r--r--   0        0        0     6148 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/.DS_Store
+-rw-r--r--   0        0        0     2134 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-07 19:09:15.501245 litellm-0.1.354/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3548 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    14054 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2578 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     4537 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0     5938 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/timeout.py
+-rw-r--r--   0        0        0    23931 2023-08-07 19:09:15.505245 litellm-0.1.354/litellm/utils.py
+-rw-r--r--   0        0        0      512 2023-08-07 19:09:15.505245 litellm-0.1.354/pyproject.toml
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 litellm-0.1.354/PKG-INFO
```

### Comparing `litellm-0.1.353/LICENSE` & `litellm-0.1.354/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/README.md` & `litellm-0.1.354/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/.DS_Store` & `litellm-0.1.354/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/__init__.py` & `litellm-0.1.354/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.354/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.354/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.354/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.354/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/aispend.py` & `litellm-0.1.354/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/berrispend.py` & `litellm-0.1.354/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/helicone.py` & `litellm-0.1.354/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/integrations/supabase.py` & `litellm-0.1.354/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/main.py` & `litellm-0.1.354/litellm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,14 @@
       if not get_secret("REPLICATE_API_TOKEN") and get_secret("REPLICATE_API_KEY"):
         replicate_api_token = get_secret("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
       elif api_key:
          os.environ["REPLICATE_API_TOKEN"] = api_key
       elif litellm.replicate_key:
          os.environ["REPLICATE_API_TOKEN"] = litellm.replicate_key
-
       prompt = " ".join([message["content"] for message in messages])
       input = {"prompt": prompt}
       if max_tokens != float('inf'):
         input["max_length"] = max_tokens # for t5 models 
         input["max_new_tokens"] = max_tokens # for llama2 models 
       ## LOGGING
       logging(model=model, input=input, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
@@ -195,15 +194,15 @@
         }
       response = model_response
     elif model in litellm.anthropic_models:
       #anthropic defaults to os.environ.get("ANTHROPIC_API_KEY")
       if api_key:
          os.environ["ANTHROPIC_API_KEY"] = api_key
       elif litellm.anthropic_key:
-         os.environ["ANTHROPIC_API_TOKEN"] = litellm.anthropic_key
+         os.environ["ANTHROPIC_API_KEY"] = litellm.anthropic_key
       prompt = f"{HUMAN_PROMPT}" 
       for message in messages:
         if "role" in message:
           if message["role"] == "user":
             prompt += f"{HUMAN_PROMPT}{message['content']}"
           else:
             prompt += f"{AI_PROMPT}{message['content']}"
```

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.354/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_api_key_param.py` & `litellm-0.1.354/litellm/tests/test_api_key_param.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,18 +11,31 @@
 
 def logger_fn(model_call_object: dict):
     print(f"model call details: {model_call_object}")
 
 user_message = "Hello, how are you?"
 messages = [{ "content": user_message,"role": "user"}]
 
-print(os.environ)
-temp_key = os.environ.get("OPENAI_API_KEY")
-os.environ["OPENAI_API_KEY"] = "bad-key"
+## Test 1: Setting key dynamically
+temp_key = os.environ.get("ANTHROPIC_API_KEY")
+os.environ["ANTHROPIC_API_KEY"] = "bad-key"
 # test on openai completion call 
 try:
-    response = completion(model="gpt-3.5-turbo", messages=messages, logger_fn=logger_fn, api_key=temp_key)
+    response = completion(model="claude-instant-1", messages=messages, logger_fn=logger_fn, api_key=temp_key)
     print(f"response: {response}")
 except:
     print(f"error occurred: {traceback.format_exc()}") 
     pass
-os.environ["OPENAI_API_KEY"] = temp_key
+os.environ["ANTHROPIC_API_KEY"] = temp_key
+
+
+## Test 2: Setting key via __init__ params
+litellm.anthropic_key = os.environ.get("ANTHROPIC_API_KEY")
+os.environ.pop("ANTHROPIC_API_KEY")
+# test on openai completion call 
+try:
+    response = completion(model="claude-instant-1", messages=messages, logger_fn=logger_fn)
+    print(f"response: {response}")
+except:
+    print(f"error occurred: {traceback.format_exc()}") 
+    pass
+os.environ["ANTHROPIC_API_KEY"] = temp_key
```

### Comparing `litellm-0.1.353/litellm/tests/test_async_fn.py` & `litellm-0.1.354/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_bad_params.py` & `litellm-0.1.354/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.354/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_client.py` & `litellm-0.1.354/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_completion.py` & `litellm-0.1.354/litellm/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_exceptions.py` & `litellm-0.1.354/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_helicone_integration.py` & `litellm-0.1.354/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_logging.py` & `litellm-0.1.354/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_model_fallback.py` & `litellm-0.1.354/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_no_client.py` & `litellm-0.1.354/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_secrets.py` & `litellm-0.1.354/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_supabase_integration.py` & `litellm-0.1.354/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/tests/test_timeout.py` & `litellm-0.1.354/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/timeout.py` & `litellm-0.1.354/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.353/litellm/utils.py` & `litellm-0.1.354/litellm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -413,25 +413,28 @@
         error_str = str(original_exception)
         if isinstance(original_exception, BaseException):
           exception_type = type(original_exception).__name__
         else:
           exception_type = ""
         logging(model=model, additional_args={"error_str": error_str, "exception_type": exception_type, "original_exception": original_exception}, logger_fn=user_logger_fn)
         if "claude" in model: #one of the anthropics
-          if "status_code" in original_exception:
+          if hasattr(original_exception, "status_code"):
             print_verbose(f"status_code: {original_exception.status_code}")
             if original_exception.status_code == 401:
               exception_mapping_worked = True
               raise AuthenticationError(f"AnthropicException - {original_exception.message}")
             elif original_exception.status_code == 400:
               exception_mapping_worked = True
               raise InvalidRequestError(f"AnthropicException - {original_exception.message}", f"{model}")
             elif original_exception.status_code == 429:
               exception_mapping_worked = True
               raise RateLimitError(f"AnthropicException - {original_exception.message}")
+          elif "Could not resolve authentication method. Expected either api_key or auth_token to be set." in error_str:
+            exception_mapping_worked = True
+            raise AuthenticationError(f"AnthropicException - {error_str}")
         elif "replicate" in model:
           if "Incorrect authentication token" in error_str:
             exception_mapping_worked = True
             raise AuthenticationError(f"ReplicateException - {error_str}")
           elif exception_type == "ModelError":
             exception_mapping_worked = True
             raise InvalidRequestError(f"ReplicateException - {error_str}", f"{model}")
```

### Comparing `litellm-0.1.353/pyproject.toml` & `litellm-0.1.354/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litellm"
-version = "0.1.353"
+version = "0.1.354"
 description = "Library to easily interface with LLM API providers"
 authors = ["BerriAI"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `litellm-0.1.353/PKG-INFO` & `litellm-0.1.354/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.353
+Version: 0.1.354
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


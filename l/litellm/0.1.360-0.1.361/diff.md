# Comparing `tmp/litellm-0.1.360.tar.gz` & `tmp/litellm-0.1.361.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.360.tar", max compression
+gzip compressed data, was "litellm-0.1.361.tar", max compression
```

## Comparing `litellm-0.1.360.tar` & `litellm-0.1.361.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1065 2023-08-08 18:37:15.105258 litellm-0.1.360/LICENSE
--rw-r--r--   0        0        0     2617 2023-08-08 18:37:15.105258 litellm-0.1.360/README.md
--rw-r--r--   0        0        0     6148 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/.DS_Store
--rw-r--r--   0        0        0     2105 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/__init__.py
--rw-r--r--   0        0        0       15 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__init__.py
--rw-r--r--   0        0        0      201 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4923 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__pycache__/aispend.cpython-311.pyc
--rw-r--r--   0        0        0     4690 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
--rw-r--r--   0        0        0     4567 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__pycache__/helicone.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/__pycache__/supabase.cpython-311.pyc
--rw-r--r--   0        0        0     5706 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/aispend.py
--rw-r--r--   0        0        0     5779 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/berrispend.py
--rw-r--r--   0        0        0     3556 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/helicone.py
--rw-r--r--   0        0        0     6294 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/integrations/supabase.py
--rw-r--r--   0        0        0    14297 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/main.py
--rw-r--r--   0        0        0     1580 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3738 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5895 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2732 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2352 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1468 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1289 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
--rw-r--r--   0        0        0       36 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/litellm_uuid.txt
--rw-r--r--   0        0        0     1372 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests/test_api_key_param.py
--rw-r--r--   0        0        0      629 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_async_fn.py
--rw-r--r--   0        0        0     1434 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_bad_params.py
--rw-r--r--   0        0        0      863 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_berrispend_integration.py
--rw-r--r--   0        0        0     2592 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_client.py
--rw-r--r--   0        0        0     4662 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_completion.py
--rw-r--r--   0        0        0      658 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_embedding.py
--rw-r--r--   0        0        0     5938 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_exceptions.py
--rw-r--r--   0        0        0      706 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_helicone_integration.py
--rw-r--r--   0        0        0     1703 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_logging.py
--rw-r--r--   0        0        0      852 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_model_fallback.py
--rw-r--r--   0        0        0      960 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_no_client.py
--rw-r--r--   0        0        0      506 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_proxy_api.py
--rw-r--r--   0        0        0     1682 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_secrets.py
--rw-r--r--   0        0        0      938 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_supabase_integration.py
--rw-r--r--   0        0        0      530 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/tests/test_timeout.py
--rw-r--r--   0        0        0        6 2023-08-08 18:37:15.105258 litellm-0.1.360/litellm/tests.txt
--rw-r--r--   0        0        0     2893 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/timeout.py
--rw-r--r--   0        0        0    24462 2023-08-08 18:37:15.109258 litellm-0.1.360/litellm/utils.py
--rw-r--r--   0        0        0      378 2023-08-08 18:37:15.109258 litellm-0.1.360/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 litellm-0.1.360/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 20:47:32.092622 litellm-0.1.361/LICENSE
+-rw-r--r--   0        0        0     2646 2023-08-08 20:47:32.092622 litellm-0.1.361/README.md
+-rw-r--r--   0        0        0     6148 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/.DS_Store
+-rw-r--r--   0        0        0     2131 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/__init__.py
+-rw-r--r--   0        0        0       15 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__init__.py
+-rw-r--r--   0        0        0      201 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4923 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/aispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4690 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/berrispend.cpython-311.pyc
+-rw-r--r--   0        0        0     4567 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/helicone.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/__pycache__/supabase.cpython-311.pyc
+-rw-r--r--   0        0        0     5706 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/aispend.py
+-rw-r--r--   0        0        0     5779 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/berrispend.py
+-rw-r--r--   0        0        0     3556 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/helicone.py
+-rw-r--r--   0        0        0     6294 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/integrations/supabase.py
+-rw-r--r--   0        0        0    15573 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/main.py
+-rw-r--r--   0        0        0     1580 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     3738 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     5895 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2732 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     2352 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1468 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0     1289 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0        0        0       36 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/litellm_uuid.txt
+-rw-r--r--   0        0        0     1372 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_api_key_param.py
+-rw-r--r--   0        0        0      629 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_async_fn.py
+-rw-r--r--   0        0        0     1434 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_bad_params.py
+-rw-r--r--   0        0        0      863 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_berrispend_integration.py
+-rw-r--r--   0        0        0     2592 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_client.py
+-rw-r--r--   0        0        0     5111 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_completion.py
+-rw-r--r--   0        0        0      658 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_embedding.py
+-rw-r--r--   0        0        0     5938 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_exceptions.py
+-rw-r--r--   0        0        0      706 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_helicone_integration.py
+-rw-r--r--   0        0        0     1703 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_logging.py
+-rw-r--r--   0        0        0      852 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_model_fallback.py
+-rw-r--r--   0        0        0      960 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_no_client.py
+-rw-r--r--   0        0        0      506 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_proxy_api.py
+-rw-r--r--   0        0        0     1682 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_secrets.py
+-rw-r--r--   0        0        0      938 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_supabase_integration.py
+-rw-r--r--   0        0        0      530 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/tests/test_timeout.py
+-rw-r--r--   0        0        0        6 2023-08-08 20:47:32.092622 litellm-0.1.361/litellm/tests.txt
+-rw-r--r--   0        0        0     2893 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/timeout.py
+-rw-r--r--   0        0        0    24462 2023-08-08 20:47:32.096622 litellm-0.1.361/litellm/utils.py
+-rw-r--r--   0        0        0      378 2023-08-08 20:47:32.096622 litellm-0.1.361/pyproject.toml
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 litellm-0.1.361/PKG-INFO
```

### Comparing `litellm-0.1.360/LICENSE` & `litellm-0.1.361/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/README.md` & `litellm-0.1.361/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
 [![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.345-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
-[![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere-blue?color=green)](https://github.com/BerriAI/litellm)
+[![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere%7CReplicate%7CHugging%20Face-blue?color=green)](https://github.com/BerriAI/litellm)
 
 Get Support / Join the community 👉 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
```

### Comparing `litellm-0.1.360/litellm/.DS_Store` & `litellm-0.1.361/litellm/.DS_Store`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/__init__.py` & `litellm-0.1.361/litellm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 max_tokens = 256 # OpenAI Defaults
 retry = True
 openai_key = None 
 azure_key = None 
 anthropic_key = None 
 replicate_key = None 
 cohere_key = None 
+
+hugging_api_token = None
 ####### THREAD-SPECIFIC DATA ###################
 class MyLocal(threading.local):
     def __init__(self):
         self.user = "Hello World"
 
 _thread_context = MyLocal()
 def identify(event_details):
```

### Comparing `litellm-0.1.360/litellm/integrations/__pycache__/aispend.cpython-311.pyc` & `litellm-0.1.361/litellm/integrations/__pycache__/aispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/__pycache__/berrispend.cpython-311.pyc` & `litellm-0.1.361/litellm/integrations/__pycache__/berrispend.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/__pycache__/helicone.cpython-311.pyc` & `litellm-0.1.361/litellm/integrations/__pycache__/helicone.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/__pycache__/supabase.cpython-311.pyc` & `litellm-0.1.361/litellm/integrations/__pycache__/supabase.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/aispend.py` & `litellm-0.1.361/litellm/integrations/aispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/berrispend.py` & `litellm-0.1.361/litellm/integrations/berrispend.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/helicone.py` & `litellm-0.1.361/litellm/integrations/helicone.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/integrations/supabase.py` & `litellm-0.1.361/litellm/integrations/supabase.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/main.py` & `litellm-0.1.361/litellm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="", deployment_id=None,
     # Optional liteLLM function params
-    *, return_async=False, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False
+    *, return_async=False, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False,
+    hugging_face = False
   ):
   try:
     global new_response
     model_response = deepcopy(new_response) # deep copy the default response format so we can mutate it and it's thread-safe. 
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
@@ -269,14 +270,40 @@
       model_response["model"] = model
       model_response["usage"] = {
           "prompt_tokens": prompt_tokens,
           "completion_tokens": completion_tokens,
           "total_tokens": prompt_tokens + completion_tokens
         }
       response = model_response
+    elif hugging_face == True:
+      import requests
+      API_URL = f"https://api-inference.huggingface.co/models/{model}"
+      HF_TOKEN = get_secret("HF_TOKEN")
+      headers = {"Authorization": f"Bearer {HF_TOKEN}"}
+
+      prompt = " ".join([message["content"] for message in messages])
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
+      input_payload = {"inputs": prompt}
+      response = requests.post(API_URL, headers=headers, json=input_payload)
+  
+      completion_response = response.json()[0]['generated_text']
+      ## LOGGING
+      logging(model=model, input=prompt, azure=azure, additional_args={"max_tokens": max_tokens, "original_response": completion_response}, logger_fn=logger_fn)
+      prompt_tokens = len(encoding.encode(prompt))
+      completion_tokens = len(encoding.encode(completion_response))
+      ## RESPONSE OBJECT
+      model_response["choices"][0]["message"]["content"] = completion_response
+      model_response["created"] = time.time()
+      model_response["model"] = model
+      model_response["usage"] = {
+          "prompt_tokens": prompt_tokens,
+          "completion_tokens": completion_tokens,
+          "total_tokens": prompt_tokens + completion_tokens
+        }
     else: 
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
```

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_bad_params.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_client.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_completion.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_exceptions.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_logging.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_model_fallback.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc` & `litellm-0.1.361/litellm/tests/__pycache__/test_timeout.cpython-311-pytest-7.4.0.pyc`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_api_key_param.py` & `litellm-0.1.361/litellm/tests/test_api_key_param.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_async_fn.py` & `litellm-0.1.361/litellm/tests/test_async_fn.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_bad_params.py` & `litellm-0.1.361/litellm/tests/test_bad_params.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_berrispend_integration.py` & `litellm-0.1.361/litellm/tests/test_berrispend_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_client.py` & `litellm-0.1.361/litellm/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_completion.py` & `litellm-0.1.361/litellm/tests/test_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,24 @@
     try:
         response = completion(model="claude-instant-1", messages=messages, logger_fn=logger_fn)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
 
+def test_completion_hf_api():
+    try:
+        user_message = "write some code to find the sum of two numbers"
+        messages = [{ "content": user_message,"role": "user"}]
+        response = completion(model="stabilityai/stablecode-completion-alpha-3b-4k", messages=messages, hugging_face=True)
+        # Add any assertions here to check the response
+        print(response)
+    except Exception as e:
+        pytest.fail(f"Error occurred: {e}")
+
 def test_completion_cohere():
     try:
         response = completion(model="command-nightly", messages=messages, max_tokens=500)
         # Add any assertions here to check the response
         print(response)
     except Exception as e:
         pytest.fail(f"Error occurred: {e}")
```

### Comparing `litellm-0.1.360/litellm/tests/test_embedding.py` & `litellm-0.1.361/litellm/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_exceptions.py` & `litellm-0.1.361/litellm/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_helicone_integration.py` & `litellm-0.1.361/litellm/tests/test_helicone_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_logging.py` & `litellm-0.1.361/litellm/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_model_fallback.py` & `litellm-0.1.361/litellm/tests/test_model_fallback.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_no_client.py` & `litellm-0.1.361/litellm/tests/test_no_client.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_secrets.py` & `litellm-0.1.361/litellm/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_supabase_integration.py` & `litellm-0.1.361/litellm/tests/test_supabase_integration.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/tests/test_timeout.py` & `litellm-0.1.361/litellm/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/timeout.py` & `litellm-0.1.361/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/litellm/utils.py` & `litellm-0.1.361/litellm/utils.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.360/PKG-INFO` & `litellm-0.1.361/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litellm
-Version: 0.1.360
+Version: 0.1.361
 Summary: Library to easily interface with LLM API providers
 License: MIT
 Author: BerriAI
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
 [![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.345-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
-[![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere-blue?color=green)](https://github.com/BerriAI/litellm)
+[![litellm](https://img.shields.io/badge/%20%F0%9F%9A%85%20liteLLM-OpenAI%7CAzure%7CAnthropic%7CPalm%7CCohere%7CReplicate%7CHugging%20Face-blue?color=green)](https://github.com/BerriAI/litellm)
 
 Get Support / Join the community 👉 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
```


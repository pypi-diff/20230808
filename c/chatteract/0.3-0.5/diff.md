# Comparing `tmp/chatteract-0.3.tar.gz` & `tmp/chatteract-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatteract-0.3.tar", last modified: Sun Aug  6 15:29:04 2023, max compression
+gzip compressed data, was "chatteract-0.5.tar", last modified: Tue Aug  8 18:58:53 2023, max compression
```

## Comparing `chatteract-0.3.tar` & `chatteract-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:29:04.735931 chatteract-0.3/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-06 15:29:04.735272 chatteract-0.3/PKG-INFO
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     7728 2023-08-06 15:21:10.000000 chatteract-0.3/README.md
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:29:04.720325 chatteract-0.3/chatteract/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      120 2023-08-02 11:44:07.000000 chatteract-0.3/chatteract/__init__.py
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     5730 2023-08-06 15:10:03.000000 chatteract-0.3/chatteract/handle_openai_response_and_execute_functions.py
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     2816 2023-08-01 17:29:49.000000 chatteract-0.3/chatteract/send_api_request.py
-drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-06 15:29:04.734116 chatteract-0.3/chatteract.egg-info/
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-06 15:29:04.000000 chatteract-0.3/chatteract.egg-info/PKG-INFO
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)      300 2023-08-06 15:29:04.000000 chatteract-0.3/chatteract.egg-info/SOURCES.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)        1 2023-08-06 15:29:04.000000 chatteract-0.3/chatteract.egg-info/dependency_links.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       18 2023-08-06 15:29:04.000000 chatteract-0.3/chatteract.egg-info/requires.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       11 2023-08-06 15:29:04.000000 chatteract-0.3/chatteract.egg-info/top_level.txt
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)       38 2023-08-06 15:29:04.736155 chatteract-0.3/setup.cfg
--rw-r--r--   0 mattias.aspelund   (501) staff       (20)     1730 2023-08-06 15:27:28.000000 chatteract-0.3/setup.py
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-08 18:58:53.336227 chatteract-0.5/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-08 18:58:53.335618 chatteract-0.5/PKG-INFO
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     7728 2023-08-06 15:21:10.000000 chatteract-0.5/README.md
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-08 18:58:53.323433 chatteract-0.5/chatteract/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      155 2023-08-08 14:21:16.000000 chatteract-0.5/chatteract/__init__.py
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     5936 2023-08-08 18:52:29.000000 chatteract-0.5/chatteract/handle_openai_response_and_execute_functions.py
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     2849 2023-08-06 15:32:47.000000 chatteract-0.5/chatteract/send_api_request.py
+drwxr-xr-x   0 mattias.aspelund   (501) staff       (20)        0 2023-08-08 18:58:53.334602 chatteract-0.5/chatteract.egg-info/
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      978 2023-08-08 18:58:53.000000 chatteract-0.5/chatteract.egg-info/PKG-INFO
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)      300 2023-08-08 18:58:53.000000 chatteract-0.5/chatteract.egg-info/SOURCES.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)        1 2023-08-08 18:58:53.000000 chatteract-0.5/chatteract.egg-info/dependency_links.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       18 2023-08-08 18:58:53.000000 chatteract-0.5/chatteract.egg-info/requires.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       11 2023-08-08 18:58:53.000000 chatteract-0.5/chatteract.egg-info/top_level.txt
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)       38 2023-08-08 18:58:53.336410 chatteract-0.5/setup.cfg
+-rw-r--r--   0 mattias.aspelund   (501) staff       (20)     1730 2023-08-08 18:54:21.000000 chatteract-0.5/setup.py
```

### Comparing `chatteract-0.3/PKG-INFO` & `chatteract-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatteract
-Version: 0.3
+Version: 0.5
 Summary: A package to handle OpenAI responses and execute function calls.
 Home-page: https://github.com/aspelund/chatter-act
 Author: Mattias Aspelund
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `chatteract-0.3/README.md` & `chatteract-0.5/README.md`

 * *Files identical despite different names*

### Comparing `chatteract-0.3/chatteract/handle_openai_response_and_execute_functions.py` & `chatteract-0.5/chatteract/handle_openai_response_and_execute_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 
 def is_function_call(response):
     if response["role"] == "assistant" and "function_call" in response and response["function_call"] is not None:
         return True
     else:
         return False
 
+def execute_function_call_on_pipeline(ai_functions, message):
+    pipeline = prepare_pipeline(ai_functions)
+
+    return execute_function_call(
+        message, pipeline['processes'])
 
 def handle_openai_response_and_execute_functions(messages, ai_functions, api_settings):
     pipeline = prepare_pipeline(ai_functions)
     new_messages = []
     max_retries = api_settings.get("max_retries", 3)
     max_consecutive_function_calls = api_settings.get("max_consecutive_function_calls", 3)
     num_cons_function_calls = 0
     while True:
         if num_cons_function_calls >= max_consecutive_function_calls:
-            raise AIFunctionCallsExceedingMaxConsecutiveError()
+            raise AIFunctionCallsExceedingMaxConsecutiveError(num_cons_function_calls)
         for i in range(max_retries):
             try:
                 with (open("logs/messages.txt", "w")) as f:
                     f.write(json.dumps(messages, indent=2))
                 o_response = send_api_request(
                     messages, api_settings, pipeline['descriptions'])
                 o_response['content'] = "" if o_response['content'] is None else o_response['content']
```

### Comparing `chatteract-0.3/chatteract/send_api_request.py` & `chatteract-0.5/chatteract/send_api_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# chatteract/send_api_request.py
 import requests
 import os
 import time
 import json
 import tiktoken
```

### Comparing `chatteract-0.3/chatteract.egg-info/PKG-INFO` & `chatteract-0.5/chatteract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatteract
-Version: 0.3
+Version: 0.5
 Summary: A package to handle OpenAI responses and execute function calls.
 Home-page: https://github.com/aspelund/chatter-act
 Author: Mattias Aspelund
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `chatteract-0.3/setup.py` & `chatteract-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chatteract',  # The name of your package
-    version='0.3',  # The current version of your package
+    version='0.5',  # The current version of your package
     packages=find_packages(),  # List of all python packages to include. find_packages() automatically detects all packages and subpackages.
     author='Mattias Aspelund',  # Your name    
     description='A package to handle OpenAI responses and execute function calls.',  # A brief description of your package
     long_description="""ChatterAct is a Python package developed to streamline the integration of OpenAI\'s GPT-4 function calling capabilities into your applications. Its primary goal is to provide a simplified, yet flexible mechanism for exposing numerous functions to the AI model with minimal effort. ChatterAct handles the execution and piping, enabling you to start simple with one or two AI functions and expand as the complexity of your project grows.
 
 Basically, what you need to do to get started is to follow a simple pattern for the functions that you want to expose to GPT, and to use the wrapper for the GPT calling.""",
     url='https://github.com/aspelund/chatter-act',  # Link to the github repo or website
```


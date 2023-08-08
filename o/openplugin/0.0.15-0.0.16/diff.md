# Comparing `tmp/openplugin-0.0.15.tar.gz` & `tmp/openplugin-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-0.0.15.tar", max compression
+gzip compressed data, was "openplugin-0.0.16.tar", max compression
```

## Comparing `openplugin-0.0.15.tar` & `openplugin-0.0.16.tar`

### file list

```diff
@@ -1,20 +1,24 @@
--rw-r--r--   0        0        0      117 2023-07-22 20:21:23.014758 openplugin-0.0.15/README.md
--rw-r--r--   0        0        0      936 2023-07-19 18:30:45.938182 openplugin-0.0.15/openplugin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-06 13:54:56.177098 openplugin-0.0.15/openplugin/__main__.py
--rw-r--r--   0        0        0     1254 2023-07-18 17:26:28.236218 openplugin-0.0.15/openplugin/api/__init__.py
--rw-r--r--   0        0        0      855 2023-06-06 13:54:56.177760 openplugin-0.0.15/openplugin/api/auth.py
--rw-r--r--   0        0        0     1624 2023-07-18 17:31:07.672783 openplugin-0.0.15/openplugin/api/genric_selector.py
--rw-r--r--   0        0        0      277 2023-06-01 21:26:45.277312 openplugin-0.0.15/openplugin/api/http_error.py
--rw-r--r--   0        0        0     1015 2023-07-18 18:17:45.860867 openplugin-0.0.15/openplugin/api/imprompt.py
--rw-r--r--   0        0        0     1027 2023-07-18 18:23:39.434879 openplugin-0.0.15/openplugin/api/langchain.py
--rw-r--r--   0        0        0     1015 2023-07-18 18:17:45.853531 openplugin-0.0.15/openplugin/api/openai.py
--rw-r--r--   0        0        0     1179 2023-07-18 21:10:07.516382 openplugin-0.0.15/openplugin/api/openplugin.py
--rw-r--r--   0        0        0     9095 2023-07-19 20:49:24.249838 openplugin-0.0.15/openplugin/bindings/imprompt/imprompt_plugin_selector.py
--rw-r--r--   0        0        0     8711 2023-07-19 20:49:24.252426 openplugin-0.0.15/openplugin/bindings/langchain/langchain_plugin_selector.py
--rw-r--r--   0        0        0     3944 2023-07-19 20:51:31.168500 openplugin-0.0.15/openplugin/bindings/openai/openai_plugin_selector.py
--rw-r--r--   0        0        0    17837 2023-07-19 20:53:46.967081 openplugin-0.0.15/openplugin/interfaces/plugin_selector.py
--rw-r--r--   0        0        0      906 2023-07-10 17:27:33.053788 openplugin-0.0.15/openplugin/main.py
--rw-r--r--   0        0        0     2917 2023-07-19 20:49:24.246254 openplugin-0.0.15/openplugin/utils/manifest_handler.py
--rw-r--r--   0        0        0     1230 2023-06-06 13:54:56.181740 openplugin-0.0.15/openplugin/utils/run_plugin_selector.py
--rw-r--r--   0        0        0      728 2023-07-24 14:58:54.227775 openplugin-0.0.15/pyproject.toml
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 openplugin-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-08-08 21:07:12.002338 openplugin-0.0.16/README.md
+-rw-r--r--   0        0        0     1610 2023-08-08 21:07:12.010338 openplugin-0.0.16/openplugin/__init__.py
+-rw-r--r--   0        0        0       49 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/__main__.py
+-rw-r--r--   0        0        0     1138 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/api/__init__.py
+-rw-r--r--   0        0        0     1657 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/api/api_signature_selector.py
+-rw-r--r--   0        0        0      856 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/api/auth.py
+-rw-r--r--   0        0        0      277 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/api/http_error.py
+-rw-r--r--   0        0        0     1753 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/api/plugin_selector.py
+-rw-r--r--   0        0        0     8944 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/imprompt/imprompt_api_signature_selector.py
+-rw-r--r--   0        0        0     8919 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/imprompt/imprompt_plugin_selector.py
+-rw-r--r--   0        0        0     6451 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/langchain/langchain_api_signature_selector.py
+-rw-r--r--   0        0        0     2133 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/langchain/langchain_helpers.py
+-rw-r--r--   0        0        0     6717 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/langchain/langchain_plugin_selector.py
+-rw-r--r--   0        0        0     3966 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/openai/openai_api_signature_selector.py
+-rw-r--r--   0        0        0      454 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/openai/openai_helpers.py
+-rw-r--r--   0        0        0     3821 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/bindings/openai/openai_plugin_selector.py
+-rw-r--r--   0        0        0     1538 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/interfaces/api_signature_selector.py
+-rw-r--r--   0        0        0    16935 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/interfaces/models.py
+-rw-r--r--   0        0        0     1693 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/interfaces/plugin_selector.py
+-rw-r--r--   0        0        0      906 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/main.py
+-rw-r--r--   0        0        0     2927 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/utils/manifest_handler.py
+-rw-r--r--   0        0        0     1237 2023-08-08 21:07:12.014339 openplugin-0.0.16/openplugin/utils/run_plugin_selector.py
+-rw-r--r--   0        0        0      855 2023-08-08 21:07:12.014339 openplugin-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 openplugin-0.0.16/PKG-INFO
```

### Comparing `openplugin-0.0.15/openplugin/api/__init__.py` & `openplugin-0.0.16/openplugin/api/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import os
-from openplugin.api import langchain
-from openplugin.api import openai
-from openplugin.api import imprompt
 from fastapi import FastAPI
 from fastapi import APIRouter
+from openplugin.api import plugin_selector
 from .http_error import http_error_handler
 from starlette.exceptions import HTTPException
 from fastapi.middleware.cors import CORSMiddleware
-from openplugin.api import genric_selector
+from openplugin.api import api_signature_selector, plugin_selector
 
 API_PREFIX = "/api"
 ENVIRONMENT = os.environ.get('ENVIRONMENT', 'development')
 
+
 def create_app() -> FastAPI:
     app = FastAPI(
         title="OpenPlugin",
         openapi_url=f"{API_PREFIX}/openapi.json",
         docs_url=f"{API_PREFIX}/docs"
     )
     if ENVIRONMENT == 'production':
         app.root_path = "/openplugin/"
 
     # add routes
     router = APIRouter()
-    # router.include_router(langchain.router)
-    # router.include_router(imprompt.router)
-    # router.include_router(openai.router)
-    router.include_router(genric_selector.router)
+    router.include_router(plugin_selector.router)
+    router.include_router(api_signature_selector.router)
     app.include_router(router, prefix=API_PREFIX)
 
     app.add_exception_handler(HTTPException, http_error_handler)
     # Allow CORS
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
```

### Comparing `openplugin-0.0.15/openplugin/api/auth.py` & `openplugin-0.0.16/openplugin/api/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dotenv import load_dotenv
 from fastapi import Security, HTTPException
 from starlette.status import HTTP_403_FORBIDDEN
 from fastapi.security.api_key import APIKeyHeader
 
 keys = set()
 load_dotenv()
+
 if os.environ.get("USER_ACCESS_KEYS_FILE_PATH") is not None:
     load_dotenv(os.environ.get("USER_ACCESS_KEYS_FILE_PATH"))
 for key in os.environ:
     if key.startswith("user_access_key_"):
         keys.add(os.environ[key])
 api_key_header = APIKeyHeader(name="x-api-key", auto_error=False)
```

### Comparing `openplugin-0.0.15/openplugin/api/genric_selector.py` & `openplugin-0.0.16/openplugin/api/plugin_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,25 @@
         messages: List[Message],
         tool_selector_config: ToolSelectorConfig,
         plugins: List[Plugin],
         config: Config,
         llm: LLM,
         api_key: APIKey = Depends(auth.get_api_key)
 ):
-    if tool_selector_config.provider == ToolSelectorProvider.Imprompt:
-        selector = ImpromptPluginSelector(tool_selector_config, plugins, config, llm)
-    elif tool_selector_config.provider == ToolSelectorProvider.Langchain:
-        selector = LangchainPluginSelector(tool_selector_config, plugins, config, llm)
-    elif tool_selector_config.provider == ToolSelectorProvider.OpenAI:
-        selector = OpenAIPluginSelector(tool_selector_config, plugins, config, llm)
-    else:
-        return JSONResponse(status_code=400,
-                            content={"message": "Incorrect ToolSelectorProvider"})
     try:
+        if tool_selector_config.provider == ToolSelectorProvider.Imprompt:
+            selector = ImpromptPluginSelector(tool_selector_config, plugins, config,
+                                              llm)
+        elif tool_selector_config.provider == ToolSelectorProvider.Langchain:
+            selector = LangchainPluginSelector(tool_selector_config, plugins, config,
+                                               llm)
+        elif tool_selector_config.provider == ToolSelectorProvider.OpenAI:
+            selector = OpenAIPluginSelector(tool_selector_config, plugins, config, llm)
+        else:
+            return JSONResponse(status_code=400,
+                                content={"message": "Incorrect ToolSelectorProvider"})
         response = selector.run(messages)
         return response
     except Exception as e:
         print(e)
         return JSONResponse(status_code=500,
                             content={"message": "Failed to run plugin"})
```

### Comparing `openplugin-0.0.15/openplugin/bindings/imprompt/imprompt_plugin_selector.py` & `openplugin-0.0.16/openplugin/bindings/imprompt/imprompt_plugin_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Set
 import openai, json, re, time, os
 from urllib.parse import urlparse, parse_qs
-from openplugin import MessageType, PluginSelector, PluginDetected, Response, Message, \
-    LLM, Plugin, \
-    ToolSelectorConfig, Config, LLMProvider
+from openplugin import MessageType, PluginSelector, PluginDetected, \
+    SelectedPluginsResponse, Message, \
+    LLM, Plugin, ToolSelectorConfig, Config, LLMProvider
 
 plugin_prompt = """
 {name_for_model}: Call this tool to get the OpenAPI spec (and usage guide) for interacting with the {name_for_model} API. 
 You should only call this ONCE! 
 
 What is the {name_for_model} API useful for? {description_for_model}.
 """
@@ -56,30 +56,21 @@
             tool_selector_config: ToolSelectorConfig,
             plugins: List[Plugin],
             config: Optional[Config],
             llm: Optional[LLM]):
         super().__init__(tool_selector_config, plugins, config, llm)
         self.llm = llm
         self.total_tokens_used = 0
-
-    def initialize_tool_selector(
-            self,
-            tool_selector_config: ToolSelectorConfig,
-            plugins: List[Plugin],
-            config: Optional[Config],
-            llm: LLM
-    ):
         openai.api_key = os.environ[
             "OPENAI_API_KEY"] if config.openai_api_key is None else config.openai_api_key
-        pass
 
-    def run(self, messages: List[Message]) -> Response:
+    def run(self, messages: List[Message]) -> SelectedPluginsResponse:
         start_test_case_time = time.time()
         plugin_operations = self.get_detected_plugin_with_operations(messages)
-        response = Response(
+        response = SelectedPluginsResponse(
             run_completed=True,
             final_text_response=None,
             detected_plugin_operations=plugin_operations,
             response_time=round(time.time() - start_test_case_time, 2),
             tokens_used=self.total_tokens_used,
             llm_api_cost=0
         )
```

### Comparing `openplugin-0.0.15/openplugin/bindings/openai/openai_plugin_selector.py` & `openplugin-0.0.16/openplugin/bindings/openai/openai_plugin_selector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,73 @@
 import os
 import json
 import time
-import openai
 from typing import List, Optional
+from .openai_helpers import chat_completion_with_backoff
 from openplugin import Config, ToolSelectorConfig, PluginDetected, Plugin, \
-    PluginSelector, LLMProvider, Message, Response, LLM, Function, Functions
-
-from tenacity import (
-    retry,
-    stop_after_attempt,
-    wait_random_exponential,
-)  #
-
-
-@retry(wait=wait_random_exponential(min=1, max=60), stop=stop_after_attempt(4))
-def chat_completion_with_backoff(**kwargs):
-    return openai.ChatCompletion.create(**kwargs)
+    PluginSelector, Message, SelectedPluginsResponse, LLM, Functions
 
 
 class OpenAIPluginSelector(PluginSelector):
     def __init__(
             self,
             tool_selector_config: ToolSelectorConfig,
             plugins: List[Plugin],
             config: Optional[Config],
             llm: Optional[LLM]):
         super().__init__(tool_selector_config, plugins, config, llm)
-
-    def initialize_tool_selector(
-            self,
-            tool_selector_config: ToolSelectorConfig,
-            plugins: List[Plugin],
-            config: Config,
-            llm: LLM
-    ):
         if config.openai_api_key is not None:
-            openai.api_key = config.openai_api_key
+            self.openai_api_key = config.openai_api_key
         else:
-            openai.api_key = os.environ["OPENAI_API_KEY"]
+            self.openai_api_key = os.environ["OPENAI_API_KEY"]
 
-    def run(self, messages: List[Message]) -> Response:
+    def run(self, messages: List[Message]) -> SelectedPluginsResponse:
         start_test_case_time = time.time()
         f_messages = [msg.get_openai_message() for msg in messages if
                       msg.get_openai_message() is not None]
         functions = Functions()
         for plugin in self.plugins:
             functions.add_from_plugin(plugin)
-        helper_pre_prompt = functions.get_helper_pre_prompt()
+        if len(functions.functions) == 0:
+            return SelectedPluginsResponse(
+                run_completed=True,
+                final_text_response="No functions found",
+                detected_plugin_operations=[],
+                response_time=round(time.time() - start_test_case_time, 2),
+                tokens_used=0,
+                llm_api_cost=0
+            )
+        helper_pre_prompt = functions.get_examples_prompt()
         if helper_pre_prompt and len(helper_pre_prompt) > 0:
             f_messages.insert(0, {"role": "assistant", "content": helper_pre_prompt})
-
         function_json = functions.get_json()
         count = 0
         is_a_function_call = True
         final_text_response = None
         total_tokens = 0
         detected_plugin_operations = []
         # while is_a_function_call and count < 5:
         count += 1
-        print(f_messages)
         response = chat_completion_with_backoff(
+            openai_api_key=self.openai_api_key,
             model=self.llm.model_name,
             messages=f_messages,
             functions=function_json,
             function_call="auto"
         )
         message = response["choices"][0]["message"]
         if message.get("function_call"):
             is_a_function_call = True
             function_name = message["function_call"]["name"]
             detected_plugin = functions.get_plugin_from_func_name(function_name)
             detected_function = functions.get_function_from_func_name(function_name)
-            arguments = json.loads(message["function_call"]["arguments"])
             p_detected = PluginDetected(
                 plugin=detected_plugin,
                 api_called=detected_function.get_api_url(),
-                method=detected_function.get_api_method(),
-                mapped_operation_parameters=arguments
+                method=detected_function.get_api_method()
             )
             detected_plugin_operations.append(p_detected)
             f_messages.append(message)
             # function_response = str(detected_function.call_api(arguments))
             function_response = f"This is a response from function {function_name}"
             f_messages.append({
                 "role": "function",
@@ -89,15 +76,15 @@
             })
         else:
             is_a_function_call = False
             final_text_response = response.get("choices")[0].get("message").get(
                 "content")
         total_tokens += response.get("usage").get("total_tokens")
 
-        response_obj = Response(
+        response_obj = SelectedPluginsResponse(
             run_completed=True,
             final_text_response=final_text_response,
             detected_plugin_operations=detected_plugin_operations,
             response_time=round(time.time() - start_test_case_time, 2),
             tokens_used=total_tokens,
             llm_api_cost=0
         )
```

### Comparing `openplugin-0.0.15/openplugin/interfaces/plugin_selector.py` & `openplugin-0.0.16/openplugin/interfaces/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import requests
+import json, yaml
 from enum import Enum
-from abc import ABC, abstractmethod
 from typing import List, Optional, Set, Dict
 from pydantic import BaseModel, validator, root_validator
-import json, yaml
-from pydantic.json import pydantic_encoder
 
 
 class PluginAuth(BaseModel):
     type: Optional[str]
     authorization_type: Optional[str]
     verification_tokens: Optional[Dict]
     scope: Optional[str]
@@ -19,15 +17,16 @@
 
 
 class PluginOperation(BaseModel):
     """
     Represents the result of a plugin operation.
     """
     human_usage_examples: Optional[List[str]] = []
-    prompt_helpers: Optional[List[str]] = []
+    prompt_signature_helpers: Optional[List[str]] = []
+    plugin_cleanup_helpers: Optional[List[str]] = []
 
 
 class Plugin(BaseModel):
     """
     Represents a plugin configuration.
     """
     manifest_url: str
@@ -107,15 +106,15 @@
 
     def get_plugin_pre_prompts(self):
         pre_prompt = ""
         index = 1
         if self.plugin_operations:
             for value in self.plugin_operations.values():
                 for val in value.values():
-                    for helper in val.prompt_helpers:
+                    for helper in val.prompt_signature_helpers:
                         pre_prompt += f"{index}: {helper}\n"
                         index = index + 1
                     for example in val.human_usage_examples:
                         pre_prompt += f"{index}: {example}\n"
                         index = index + 1
         if index > 1:
             pre_prompt = f"For plugin: {self.name}:\n" + pre_prompt
@@ -125,14 +124,17 @@
 class PluginDetected(BaseModel):
     """
     Represents the result of a plugin operation.
     """
     plugin: Plugin
     api_called: Optional[str]
     method: Optional[str]
+
+
+class PluginDetectedParams(PluginDetected):
     mapped_operation_parameters: Optional[Dict[str, str]] = None
 
 
 class Config(BaseModel):
     """
     Represents the API configuration for a plugin.
     """
@@ -165,15 +167,15 @@
 class Function(BaseModel):
     name: Optional[str]
     api: Optional[API]
     description: Optional[str]
     param_type: Optional[str]
     param_properties: Optional[List[FunctionProperty]]
     human_usage_examples: Optional[List[str]] = []
-    prompt_helpers: Optional[List[str]] = []
+    prompt_signature_helpers: Optional[List[str]] = []
 
     def get_api_url(self):
         return self.api.url
 
     def get_api_method(self):
         return self.api.method
 
@@ -229,42 +231,65 @@
 
     def add_from_plugin(self, plugin: Plugin):
         self.add_from_manifest(plugin.manifest_url, plugin)
 
     def add_from_manifest(self, manifest_url: str, plugin: Plugin = None):
         manifest_obj = requests.get(manifest_url).json()
         open_api_spec_url = manifest_obj.get("openapi_doc_url")
+        valid_operations = []
+        for key in manifest_obj.get("plugin_operations"):
+            methods = manifest_obj.get("plugin_operations").get(key).keys()
+            for method in methods:
+                valid_operations.append(key + "_" + method)
         self.add_from_openapi_spec(open_api_spec_url, plugin=plugin,
                                    plugin_operations_map=manifest_obj.get(
-                                       "plugin_operations"))
+                                       "plugin_operations"),
+                                   valid_operations=valid_operations)
 
-    def get_helper_pre_prompt(self):
+    def get_prompt_signatures_prompt(self):
         prompt = ""
-        index=1
+        index = 1
         for function in self.functions:
-            for helper in function.prompt_helpers:
-                prompt += f"prompt helper= {helper} \n"
+            for helper in function.prompt_signature_helpers:
+                prompt += f"{helper} "
                 index = index + 1
+        prompt = prompt.strip()
+        if len(prompt) > 0:
+            prompt = "The prompt signature helper prompts to help map API parameters:  " + prompt
+        return prompt.strip()
+
+    def get_examples_prompt(self):
+        prompt = ""
+        index = 1
+        for function in self.functions:
             for example in function.human_usage_examples:
                 prompt += f"example= {example} \n"
                 index = index + 1
+        prompt = prompt.strip()
+        if len(prompt) > 0:
+            prompt = "The usage examples to predict the plugin:  " + prompt
         return prompt.strip()
 
     def add_from_openapi_spec(self, open_api_spec_url: str, plugin: Plugin = None,
-                              header: dict = None, plugin_operations_map: dict = None):
+                              header: dict = None, plugin_operations_map: dict = None,
+                              valid_operations: List[str] = None):
         openapi_doc_json = requests.get(open_api_spec_url).json()
         if openapi_doc_json is None:
             return ValueError("Could not get OpenAPI spec from URL")
         server_url = openapi_doc_json.get("servers")[0].get("url")
         api_endpoints = []
         paths = openapi_doc_json.get("paths")
         functions = []
+
         for path in paths:
             api_endpoints.append(f"{server_url}{path}")
             for method in paths[path]:
+                if valid_operations is not None:
+                    if f"{path}_{method}" not in valid_operations:
+                        continue
                 details = paths[path][method]
                 function_values = {}
                 function_values["api"] = API(url=f"{server_url}{path}", method=method,
                                              header=header)
                 function_values["name"] = f"{method}{path.replace('/', '_')}"
                 function_values["description"] = details.get("summary")
                 function_values["param_type"] = "object"
@@ -305,18 +330,19 @@
                             properties_values["is_required"] = False
                         properties.append(properties_values)
                 function_values["param_properties"] = properties
                 human_usage_examples = plugin_operations_map.get(path, {}).get(method,
                                                                                {}).get(
                     "human_usage_examples", [])
                 function_values["human_usage_examples"] = human_usage_examples
-                prompt_helpers = plugin_operations_map.get(path, {}).get(method,
-                                                                         {}).get(
-                    "prompt_helpers", [])
-                function_values["prompt_helpers"] = prompt_helpers
+                prompt_signature_helpers = plugin_operations_map.get(path, {}).get(
+                    method,
+                    {}).get(
+                    "prompt_signature_helpers", [])
+                function_values["prompt_signature_helpers"] = prompt_signature_helpers
                 func = Function(**function_values)
                 if plugin:
                     self.plugin_map[func.name] = plugin
                 self.function_map[func.name] = func
                 functions.append(func)
         self.functions.extend(functions)
 
@@ -381,26 +407,38 @@
     """
     Represents the configuration for a Tool Selector.
     """
     provider: ToolSelectorProvider
     pipeline_name: str
 
 
-class Response(BaseModel):
+class SelectedPluginsResponse(BaseModel):
     """
     Represents the response from executing prompts.
     """
     run_completed: bool
     final_text_response: Optional[str]
     detected_plugin_operations: Optional[List[PluginDetected]]
     response_time: Optional[float]
     tokens_used: Optional[int]
     llm_api_cost: Optional[float]
 
 
+class SelectedApiSignatureResponse(BaseModel):
+    """
+    Represents the response from executing prompts.
+    """
+    run_completed: bool
+    final_text_response: Optional[str]
+    detected_plugin_operations: Optional[List[PluginDetectedParams]]
+    response_time: Optional[float]
+    tokens_used: Optional[int]
+    llm_api_cost: Optional[float]
+
+
 class MessageType(str, Enum):
     HumanMessage = "HumanMessage"
     AIMessage = "AIMessage"
     SystemMessage = "SystemMessage"
     FunctionMessage = "FunctionMessage"
 
 
@@ -414,70 +452,7 @@
     def get_openai_message(self):
         if self.message_type == MessageType.HumanMessage:
             return {"role": "user", "content": self.content}
         elif self.message_type == MessageType.AIMessage:
             return {"role": "assistant", "content": self.content}
         elif self.message_type == MessageType.SystemMessage:
             return {"role": "system", "content": self.content}
-
-
-class PluginSelector(ABC):
-    """Abstract base class for plugin selectors."""
-
-    def __init__(
-            self,
-            tool_selector_config: ToolSelectorConfig,
-            plugins: List[Plugin],
-            config: Optional[Config],
-            llm: Optional[LLM]
-    ):
-        """
-        Initialize the plugin selector.
-        Args:
-            tool_selector_config (ToolSelectorConfig): Configuration for the tool selector.
-            plugins (List[Plugin]): List of plugins to be used by the plugin selector.
-            config (Optional[Config]): Additional configuration for the plugin selector.
-            llm (Optional[LLM]): Additional language model for the plugin selector.
-        """
-        self.plugins = plugins
-        self.llm = llm
-        self.initialize_tool_selector(tool_selector_config, plugins, config, llm)
-
-    def get_plugin_by_name(self, name: str):
-        for plugin in self.plugins:
-            if plugin.name == name:
-                return plugin
-        return None
-
-    @abstractmethod
-    def initialize_tool_selector(
-            self,
-            tool_selector_config: ToolSelectorConfig,
-            plugins: Optional[List[Plugin]],
-            config: Optional[Config],
-            llm: Optional[LLM],
-    ):
-        """
-        Initialize the plugin selector with the provided configuration.
-        This method should be implemented by the derived classes.
-        Args:
-            tool_selector_config (ToolSelectorConfig): Configuration for the plugin selector.
-            plugins (Optional[List[Plugin]]): List of plugins to be used by the plugin selector.
-            config (Optional[Config]): Additional configuration for the plugin selector.
-            llm (Optional[LLM]): Additional language model for the plugin selector.
-        """
-        pass
-
-    @abstractmethod
-    def run(
-            self,
-            messages: List[Message]
-    ) -> Response:
-        """
-        Run the plugin selector on the given list of messages and return a response.
-        This method should be implemented by the derived classes.
-        Args:
-            messages (List[Message]): List of messages to be processed by the plugin selector.
-        Returns:
-            Response: The response generated by the plugin selector.
-        """
-        pass
```

### Comparing `openplugin-0.0.15/openplugin/main.py` & `openplugin-0.0.16/openplugin/main.py`

 * *Files identical despite different names*

### Comparing `openplugin-0.0.15/openplugin/utils/manifest_handler.py` & `openplugin-0.0.16/openplugin/utils/manifest_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             for method in paths.get(key):
                 api_endpoints.append(f"{server_url}{key}")
                 plugin_operations[key] = {}
                 plugin_operations[key][method] = PluginOperation(
                     path=key,
                     method=method,
                     human_usage_examples=["hello", "world"],
-                    prompt_helpers=["hello", "world"]
+                    prompt_signature_helpers=["hello", "world"]
                 )
     if selected_operations and len(selected_operations) > 0:
         plugin_operations = selected_operations
     plugin_obj = Plugin(
         manifest_url=manifest_url,
         schema_version=schema_version,
         name=name,
```

### Comparing `openplugin-0.0.15/openplugin/utils/run_plugin_selector.py` & `openplugin-0.0.16/openplugin/utils/run_plugin_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import json
-from openplugin.interfaces.plugin_selector import Message, Plugin, Config, ToolSelectorConfig, LLM, ToolSelectorProvider
+from openplugin import Message, Plugin, Config, ToolSelectorConfig, \
+    LLM, ToolSelectorProvider
 
 
 def run_plugin_selector(inp_json):
     if type(inp_json) == str:
         inp_json = json.loads(inp_json)
     messages = [Message(**m) for m in inp_json["messages"]]
     plugins = [Plugin(**p) for p in inp_json["plugins"]]
     config = Config(**inp_json["config"])
     tool_selector_config = ToolSelectorConfig(**inp_json["tool_selector_config"])
     llm = LLM(**inp_json["llm"])
 
     if tool_selector_config.provider == ToolSelectorProvider.Imprompt:
-        from openplugin.bindings.imprompt.imprompt_plugin_selector import ImpromptPluginSelector
+        from openplugin.bindings.imprompt.imprompt_plugin_selector import \
+            ImpromptPluginSelector
         selector = ImpromptPluginSelector(tool_selector_config, plugins, config, llm)
         response = selector.run(messages)
         return response.dict()
     elif tool_selector_config.provider == ToolSelectorProvider.Langchain:
-        from openplugin.bindings.langchain.langchain_plugin_selector import LangchainPluginSelector
+        from openplugin.bindings.langchain.langchain_plugin_selector import \
+            LangchainPluginSelector
         selector = LangchainPluginSelector(tool_selector_config, plugins, config, llm)
         response = selector.run(messages)
         return response.dict()
     raise Exception("Unknown tool selector provider")
```

### Comparing `openplugin-0.0.15/pyproject.toml` & `openplugin-0.0.16/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openplugin"
-version = "0.0.15"
+version = "0.0.16"
 description = ""
 authors = ["shrikant <shrikant.pm14@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "^0.0.178"
@@ -22,13 +22,20 @@
 sphinx-autobuild = "^2021.3.14"
 sphinx = "6.2.1"
 sphinx-book-theme = "^1.0.1"
 toml = "^0.10.2"
 sphinx-copybutton = "^0.5.2"
 sphinx-tabs = "^3.4.1"
 
+
+[tool.poetry.group.test.dependencies]
+poethepoet = "^0.21.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 openplugin = "openplugin.main:app"
+
+[tool.poe.tasks]
+build_docs = "sphinx-build docs/source _build"
```

### Comparing `openplugin-0.0.15/PKG-INFO` & `openplugin-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin
-Version: 0.0.15
+Version: 0.0.16
 Summary: 
 Author: shrikant
 Author-email: shrikant.pm14@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


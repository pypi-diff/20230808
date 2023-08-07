# Comparing `tmp/im_openai-0.7.3.tar.gz` & `tmp/im_openai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.7.3.tar", last modified: Fri Jul 28 00:48:46 2023, max compression
+gzip compressed data, was "im_openai-0.8.0.tar", last modified: Mon Aug  7 22:43:29 2023, max compression
```

## Comparing `im_openai-0.7.3.tar` & `im_openai-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.694106 im_openai-0.7.3/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.7.3/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.7.3/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.7.3/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.7.3/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-07-28 00:48:46.695011 im_openai-0.7.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4315 2023-07-26 22:37:33.000000 im_openai-0.7.3/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.566681 im_openai-0.7.3/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.7.3/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.7.3/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.7.3/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.589998 im_openai-0.7.3/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-28 00:48:07.000000 im_openai-0.7.3/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5671 2023-07-28 00:44:13.000000 im_openai-0.7.3/im_openai/client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.641518 im_openai-0.7.3/im_openai/langchain/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.7.3/im_openai/langchain/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17280 2023-07-26 22:18:17.000000 im_openai-0.7.3/im_openai/langchain/callbacks.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.7.3/im_openai/langchain/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7888 2023-07-25 03:35:20.000000 im_openai-0.7.3/im_openai/langchain/util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4003 2023-07-28 00:45:25.000000 im_openai-0.7.3/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.7.3/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.621863 im_openai-0.7.3/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6621 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-28 00:48:46.000000 im_openai-0.7.3/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.7.3/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-28 00:48:46.697580 im_openai-0.7.3/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-28 00:48:07.000000 im_openai-0.7.3/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 00:48:46.688904 im_openai-0.7.3/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.7.3/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.7.3/tests/test_im_openai.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9375 2023-07-20 01:08:51.000000 im_openai-0.7.3/tests/test_langchain.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13484 2023-07-25 03:36:46.000000 im_openai-0.7.3/tests/test_langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-07-21 22:42:02.000000 im_openai-0.7.3/tests/test_patch.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.567117 im_openai-0.8.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.8.0/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.8.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.8.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6721 2023-08-07 22:43:29.568252 im_openai-0.8.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4342 2023-08-07 22:15:43.000000 im_openai-0.8.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.487520 im_openai-0.8.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.8.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.8.0/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.8.0/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.504422 im_openai-0.8.0/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-08-07 22:43:03.000000 im_openai-0.8.0/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6022 2023-08-07 22:32:32.000000 im_openai-0.8.0/im_openai/client.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.541690 im_openai-0.8.0/im_openai/langchain/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.8.0/im_openai/langchain/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17507 2023-08-07 22:15:43.000000 im_openai-0.8.0/im_openai/langchain/callbacks.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.8.0/im_openai/langchain/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7888 2023-07-25 03:35:20.000000 im_openai-0.8.0/im_openai/langchain/util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4003 2023-07-28 00:45:25.000000 im_openai-0.8.0/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.8.0/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.526000 im_openai-0.8.0/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6721 2023-08-07 22:43:29.000000 im_openai-0.8.0/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2023-08-07 22:43:29.000000 im_openai-0.8.0/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-08-07 22:43:29.000000 im_openai-0.8.0/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-08-07 22:43:29.000000 im_openai-0.8.0/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-08-07 22:43:29.000000 im_openai-0.8.0/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.8.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-08-07 22:43:29.570938 im_openai-0.8.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-08-07 22:43:03.000000 im_openai-0.8.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-07 22:43:29.564483 im_openai-0.8.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.8.0/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4471 2023-08-07 22:40:16.000000 im_openai-0.8.0/tests/test_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.8.0/tests/test_im_openai.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9453 2023-08-07 22:15:43.000000 im_openai-0.8.0/tests/test_langchain.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13562 2023-08-07 22:15:43.000000 im_openai-0.8.0/tests/test_langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2980 2023-08-07 22:15:43.000000 im_openai-0.8.0/tests/test_patch.py
```

### Comparing `im_openai-0.7.3/CONTRIBUTING.rst` & `im_openai-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/LICENSE` & `im_openai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/PKG-INFO` & `im_openai-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.7.3
+Version: 0.8.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -32,15 +32,15 @@
 monitor
 
 -   Free software: MIT license
 -   Documentation: <https://im-openai.readthedocs.io>.
 
 ## Features
 
--   Patches the openai library to allow user to set an ip_project_key
+-   Patches the openai library to allow user to set an ip_api_key and ip_api_name
     for each request
 -   Works out of the box with langchain
 
 ## Get Started
 
 ### OpenAI
 
@@ -48,23 +48,23 @@
 following code:
 
 ```python
 from im_openai import patch_openai
 patch_openai()
 ```
 
-Then, set the `ip_project_key` and `ip_api_name` for each request:
+Then, set the `ip_api_key` and `ip_api_name` for each request:
 
 ```python
 import openai
 
 completion = openai.ChatCompletion.create(
     engine="davinci",
     prompt="Show me an emoji that matches the sport: soccer",
-    ip_project_key="emojification",
+    ip_api_key="6a0ea966-8e4d-45ef-b7bf-9577ab73a60d",
     ip_api_name="sport-emoji",
     ip_template_params={"sport": "soccer"},
     ip_template_chat=[{"role": "user", "content": "Show me an emoji that matches the sport: {sport}" }]
 )
 ```
 
 ### Langchain
@@ -219,7 +219,11 @@
 ## 0.7.1
 
 -   Pass along model params to the server
 
 ## 0.7.3
 
 -   add explicit support for api_key
+
+## 0.8.0
+
+-   switch to api_key, pretend project_key isn't even a thing
```

### Comparing `im_openai-0.7.3/README.md` & `im_openai-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 monitor
 
 -   Free software: MIT license
 -   Documentation: <https://im-openai.readthedocs.io>.
 
 ## Features
 
--   Patches the openai library to allow user to set an ip_project_key
+-   Patches the openai library to allow user to set an ip_api_key and ip_api_name
     for each request
 -   Works out of the box with langchain
 
 ## Get Started
 
 ### OpenAI
 
@@ -26,23 +26,23 @@
 following code:
 
 ```python
 from im_openai import patch_openai
 patch_openai()
 ```
 
-Then, set the `ip_project_key` and `ip_api_name` for each request:
+Then, set the `ip_api_key` and `ip_api_name` for each request:
 
 ```python
 import openai
 
 completion = openai.ChatCompletion.create(
     engine="davinci",
     prompt="Show me an emoji that matches the sport: soccer",
-    ip_project_key="emojification",
+    ip_api_key="6a0ea966-8e4d-45ef-b7bf-9577ab73a60d",
     ip_api_name="sport-emoji",
     ip_template_params={"sport": "soccer"},
     ip_template_chat=[{"role": "user", "content": "Show me an emoji that matches the sport: {sport}" }]
 )
 ```
 
 ### Langchain
```

### Comparing `im_openai-0.7.3/docs/Makefile` & `im_openai-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/docs/conf.py` & `im_openai-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/docs/installation.rst` & `im_openai-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/docs/make.bat` & `im_openai-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/im_openai/client.py` & `im_openai-0.8.0/im_openai/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+"""Utilities for sending events to Imaginary Dev."""
 import asyncio
+import logging
 import os
 import time
 import uuid
 import warnings
 from contextlib import asynccontextmanager
 from typing import Any, Dict, List, TypedDict
 
 import aiohttp
 
+logger = logging.getLogger(__name__)
+
 
 async def send_event(
     session: aiohttp.ClientSession,
-    project_key: str,
     api_key: str | None,
     *,
+    project_key: str | None = None,
     api_name: str | None,
-    prompt_event_id: str | None,
-    prompt_template_text: str | None,
-    prompt_template_chat: List | None,
-    prompt_params: Dict | None,
-    chat_id: str | None,
+    prompt_event_id: str | None = None,
+    prompt_template_text: str | None = None,
+    prompt_template_chat: List | None = None,
+    prompt_params: Dict | None = None,
+    chat_id: str | None = None,
     response: str | None = None,
     response_time: float | None = None,
     prompt: Any | None = None,
     parent_event_id: str | None = None,
     model_params: Dict | None = None,
 ) -> str | None:
     """Send an event to Imaginary Dev. Returns the id of the event that was added on the server."""
@@ -34,19 +38,24 @@
         "apiName": api_name,
         "params": {},
         "prompt": prompt or {},
         "promptEventId": prompt_event_id,
         "modelParameters": model_params or {},
     }
 
+    logger.debug(f"Sending event to {PROMPT_REPORTING_URL}")
     if project_key is not None:
         event["projectKey"] = project_key
     if api_key is not None:
         event["apiKey"] = api_key
 
+    if not api_key and not project_key:
+        logger.warn("No project key or api key set, not sending event")
+        return
+
     if prompt_template_text is not None:
         if isinstance(prompt_template_text, str):
             # first default template to just the raw text
             event["promptTemplateText"] = prompt_template_text
             if prompt_params is None and getattr(prompt_template_text, "params", None):
                 # Can be TemplateString or any other
                 prompt_params = prompt_template_text.params  # type: ignore
@@ -85,15 +94,15 @@
     json = await result.json()
     if isinstance(json, dict):
         return json.get("id")
 
 
 @asynccontextmanager
 async def event_session(
-    project_key: str,
+    project_key: str | None,
     api_key: str | None,
     api_name: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     model_params: Dict | None = None,
     chat_id: str | None = None,
     prompt_template_params: dict | None = None,
```

### Comparing `im_openai-0.7.3/im_openai/langchain/callbacks.py` & `im_openai-0.8.0/im_openai/langchain/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
 logger = logging.getLogger(__name__)
 
 from functools import wraps
 
 
 class PromptWatchCallbacks(BaseCallbackHandler):
-    project_key: str
+    api_key: str
+    project_key: str | None
     api_name: str
 
     template_chat: List[Dict] | None
     template_text: str | None
 
     runs: Dict[UUID, Dict[str, Any]] = {}
     """A dictionary of information about a run, keyed by run_id"""
@@ -45,32 +46,35 @@
     server_event_ids: Dict[UUID, str | None] = {}
     """Mapping of run_id to server event id"""
 
     valid_namespaces: List[str] | None = None
 
     def __init__(
         self,
-        project_key: str,
+        api_key: str,
         api_name: str,
         *,
+        project_key: Optional[str] = None,
         template_text: Optional[str] = None,
         template_chat: Optional[List[Union[BaseMessagePromptTemplate, BaseMessage]]] = None,
         valid_namespaces: Optional[List[str]] = None,
     ):
         """Initialize the callback handler
 
         Args:
+            api_key (str): The Imaginary Programming API key
             project_key (str): The Imaginary Programming project key
             api_name (str): The Imaginary Programming API name
             template_text (Optional[str], optional): The template to use for completion events. Defaults to None.
             template_chat (Optional[List[Union[BaseMessagePromptTemplate, BaseMessage]]], optional): The template to use for chat events. Defaults to None.
         """
-        self.project_key = project_key or os.environ.get("PROMPT_PROJECT_KEY", "")
-        if not self.project_key:
-            raise ValueError("project_key must be provided")
+        self.project_key = project_key or os.environ.get("PROMPT_PROJECT_KEY", None)
+        self.api_key = api_key or os.environ.get("PROMPT_API_KEY", "")
+        if not self.api_key:
+            raise ValueError("api_key must be provided")
         self.valid_namespaces = valid_namespaces
         self.runs = {}
         self.api_name = api_name
         if template_text is not None:
             self.template_text = template_text
         elif template_chat is not None:
             self.template_chat = util.format_chat_template(template_chat)
@@ -367,14 +371,15 @@
                     prompt_template_chat = None
 
                 # TODO: gather these up and send them all at once
                 prompt_event_id = self._get_server_event_id(run_id)
                 id = await client.send_event(
                     session,
                     project_key=self.project_key,
+                    api_key=self.api_key,
                     api_name=self.api_name,
                     prompt_template_text=prompt_template_text,  # type: ignore
                     prompt_template_chat=prompt_template_chat,  # type: ignore
                     prompt_params=json_inputs,
                     prompt_event_id=prompt_event_id,
                     model_params=model_params,
                     chat_id=None,
@@ -482,14 +487,14 @@
 def prompt_watch_tracing(*args, **kwargs):
     """Inject a tracing callback into langchain to watch for prompts.
 
     Note that this hijacks the v2 tracing callback, so if you're using that for something else, this will break it.
 
     usage::
 
-        with prompt_watch_tracing(project_key, api_name, template_text="Hello {name}"):
+        with prompt_watch_tracing(api_key, api_name, template_text="Hello {name}"):
             chain = LLMChain(llm=...)
             chain.run("Hello world", inputs={"name": "world"})
     """
     old_tracing_v2_callback = enable_prompt_watch_tracing(*args, **kwargs)
     yield
     disable_prompt_watch_tracing(old_tracing_v2_callback)
```

### Comparing `im_openai-0.7.3/im_openai/langchain/patch.py` & `im_openai-0.8.0/im_openai/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/im_openai/langchain/util.py` & `im_openai-0.8.0/im_openai/langchain/util.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/im_openai/patch.py` & `im_openai-0.8.0/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/im_openai.egg-info/PKG-INFO` & `im_openai-0.8.0/im_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.7.3
+Version: 0.8.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -32,15 +32,15 @@
 monitor
 
 -   Free software: MIT license
 -   Documentation: <https://im-openai.readthedocs.io>.
 
 ## Features
 
--   Patches the openai library to allow user to set an ip_project_key
+-   Patches the openai library to allow user to set an ip_api_key and ip_api_name
     for each request
 -   Works out of the box with langchain
 
 ## Get Started
 
 ### OpenAI
 
@@ -48,23 +48,23 @@
 following code:
 
 ```python
 from im_openai import patch_openai
 patch_openai()
 ```
 
-Then, set the `ip_project_key` and `ip_api_name` for each request:
+Then, set the `ip_api_key` and `ip_api_name` for each request:
 
 ```python
 import openai
 
 completion = openai.ChatCompletion.create(
     engine="davinci",
     prompt="Show me an emoji that matches the sport: soccer",
-    ip_project_key="emojification",
+    ip_api_key="6a0ea966-8e4d-45ef-b7bf-9577ab73a60d",
     ip_api_name="sport-emoji",
     ip_template_params={"sport": "soccer"},
     ip_template_chat=[{"role": "user", "content": "Show me an emoji that matches the sport: {sport}" }]
 )
 ```
 
 ### Langchain
@@ -219,7 +219,11 @@
 ## 0.7.1
 
 -   Pass along model params to the server
 
 ## 0.7.3
 
 -   add explicit support for api_key
+
+## 0.8.0
+
+-   switch to api_key, pretend project_key isn't even a thing
```

### Comparing `im_openai-0.7.3/im_openai.egg-info/SOURCES.txt` & `im_openai-0.8.0/im_openai.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,11 +26,12 @@
 im_openai.egg-info/not-zip-safe
 im_openai.egg-info/top_level.txt
 im_openai/langchain/__init__.py
 im_openai/langchain/callbacks.py
 im_openai/langchain/patch.py
 im_openai/langchain/util.py
 tests/__init__.py
+tests/test_client.py
 tests/test_im_openai.py
 tests/test_langchain.py
 tests/test_langchain_util.py
 tests/test_patch.py
```

### Comparing `im_openai-0.7.3/setup.py` & `im_openai-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.7.3",
+    version="0.8.0",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.7.3/tests/test_im_openai.py` & `im_openai-0.8.0/tests/test_im_openai.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.3/tests/test_langchain.py` & `im_openai-0.8.0/tests/test_langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     StringPromptTemplate,
     SystemMessagePromptTemplate,
 )
 from langchain.schema import Generation, HumanMessage, LLMResult, SystemMessage
 
 from im_openai import langchain as langchain_util
 
-project_key = "abc"
+api_key = "abc"
 api_name = "def"
 
 
 @pytest.fixture(autouse=True)
 def openai_api_key():
     os.environ["OPENAI_API_KEY"] = "abc"
     yield
@@ -47,31 +47,32 @@
     asyncio.set_event_loop(loop)
     yield loop
     loop.close()
 
 
 @pytest.fixture()
 def pwc():
-    return langchain_util.PromptWatchCallbacks(project_key=project_key, api_name=api_name)
+    return langchain_util.PromptWatchCallbacks(api_key=api_key, api_name=api_name)
 
 
 def test_llm_start(pwc: langchain_util.PromptWatchCallbacks, mock_send_event: MagicMock):
     run_id = uuid.uuid4()
     parent_run_id = uuid.uuid4()
     prompt = PromptTemplate.from_template("What is a good name for a company that makes {product}?")
     chain = LLMChain(
         llm=OpenAI(client=None, model="text-davinci-003", temperature=0.5),
         prompt=prompt,
     )
     run_llm_start(pwc, mock_send_event, run_id, parent_run_id, chain)
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text="What is a good name for a company that makes {product}?",
         prompt_template_chat=None,
         prompt_params={"product": "socks"},
         prompt_event_id=None,
         chat_id=None,
         model_params={"modelType": "completion", "temperature": 0.5, "model": "text-davinci-003"},
         response=None,
@@ -108,16 +109,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
                 "role": "system",
             },
             {"content": "{text}", "role": "user"},
@@ -154,16 +156,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=None,
         prompt_params=template_args,
         prompt_event_id=None,
         chat_id=None,
         response=None,
         response_time=None,
@@ -214,16 +217,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "role": "system",
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
             }
         ],
@@ -242,16 +246,17 @@
         LLMResult(generations=[[Generation(text="hi")]]),
         run_id=run_id,
         parent_run_id=parent_run_id,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "role": "system",
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
             }
         ],
```

### Comparing `im_openai-0.7.3/tests/test_langchain_util.py` & `im_openai-0.8.0/tests/test_langchain_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     LLMResult,
     SystemMessage,
 )
 
 from im_openai.langchain import callbacks as langchain_callbacks
 from im_openai.langchain import util as langchain_util
 
-project_key = "abc"
+api_key = "abc"
 api_name = "def"
 
 
 @pytest.fixture(autouse=True)
 def openai_api_key():
     os.environ["OPENAI_API_KEY"] = "abc"
     yield
@@ -56,31 +56,32 @@
     asyncio.set_event_loop(loop)
     yield loop
     loop.close()
 
 
 @pytest.fixture()
 def pwc():
-    return langchain_callbacks.PromptWatchCallbacks(project_key=project_key, api_name=api_name)
+    return langchain_callbacks.PromptWatchCallbacks(api_key=api_key, api_name=api_name)
 
 
 def test_llm_start(pwc: langchain_callbacks.PromptWatchCallbacks, mock_send_event: MagicMock):
     run_id = uuid.uuid4()
     parent_run_id = uuid.uuid4()
     prompt = PromptTemplate.from_template("What is a good name for a company that makes {product}?")
     chain = LLMChain(
         llm=OpenAI(client=None, model="text-davinci-003", temperature=0.5),
         prompt=prompt,
     )
     run_llm_start(pwc, mock_send_event, run_id, parent_run_id, chain)
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text="What is a good name for a company that makes {product}?",
         prompt_template_chat=None,
         prompt_params={"product": "socks"},
         prompt_event_id=None,
         chat_id=None,
         model_params={"modelType": "completion", "temperature": 0.5, "model": "text-davinci-003"},
         response=None,
@@ -119,16 +120,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
                 "role": "system",
             },
             {"content": "{text}", "role": "user"},
@@ -165,16 +167,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=None,
         prompt_params=template_args,
         prompt_event_id=None,
         chat_id=None,
         response=None,
         response_time=None,
@@ -225,16 +228,17 @@
         parent_run_id,
         chain,
         template_args,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "role": "system",
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
             }
         ],
@@ -253,16 +257,17 @@
         LLMResult(generations=[[Generation(text="hi")]]),
         run_id=run_id,
         parent_run_id=parent_run_id,
     )
 
     mock_send_event.assert_called_once_with(
         ANY,
-        project_key=project_key,
+        api_key=api_key,
         api_name=api_name,
+        project_key=None,
         prompt_template_text=None,
         prompt_template_chat=[
             {
                 "role": "system",
                 "content": "You are a helpful assistant that translates {input_language} to {output_language}.",
             }
         ],
```

### Comparing `im_openai-0.7.3/tests/test_patch.py` & `im_openai-0.8.0/tests/test_patch.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,38 +29,39 @@
 def test_chat_completion(mock_chat, mock_send_event: MagicMock, do_patch_openai):
     template = "Send a greeting to our new user named {name}"
     ip_template_params = {"name": "Alec"}
     prompt_text = template.format(**ip_template_params)
 
     chat_messages = [{"role": "user", "content": prompt_text}]
     chat_template = [{"role": "user", "content": template}]
-    project_key = "alecf-local-playground"
+    api_key = "alecf-local-playground"
     api_name = "test-from-apitest-chat"
     event_id = uuid.uuid4()
     parent_event_id = uuid.uuid4()
     chat_id = uuid.uuid4()
     openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=chat_messages,
         temperature=0.4,
-        ip_project_key=project_key,
+        ip_api_key=api_key,
         ip_api_name=api_name,
         ip_template_chat=chat_template,
         ip_template_params=ip_template_params,
         ip_parent_event_id=parent_event_id,
         ip_event_id=event_id,
         ip_chat_id=chat_id,
     )
 
     assert tuple(mock_send_event.call_args_list[0]) == (
         (),
         dict(
             session=ANY,
-            project_key=project_key,
+            api_key=api_key,
             api_name=api_name,
+            project_key=None,
             prompt_event_id=event_id,
             prompt_template_text=None,
             prompt_template_chat=[
                 {"role": "user", "content": "Send a greeting to our new user named {name}"}
             ],
             prompt_params=ip_template_params,
             chat_id=chat_id,
@@ -73,16 +74,17 @@
             },
         ),
     )
     assert tuple(mock_send_event.call_args_list[1]) == (
         (),
         dict(
             session=ANY,
-            project_key="alecf-local-playground",
+            api_key=api_key,
             api_name="test-from-apitest-chat",
+            project_key=None,
             prompt_event_id=event_id,
             prompt_template_text=None,
             prompt_template_chat=[
                 {"role": "user", "content": "Send a greeting to our new user named {name}"}
             ],
             prompt_params=ip_template_params,
             chat_id=chat_id,
```


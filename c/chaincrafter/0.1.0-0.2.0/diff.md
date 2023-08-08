# Comparing `tmp/chaincrafter-0.1.0.tar.gz` & `tmp/chaincrafter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaincrafter-0.1.0.tar", last modified: Mon Aug  7 13:44:10 2023, max compression
+gzip compressed data, was "chaincrafter-0.2.0.tar", last modified: Tue Aug  8 13:17:57 2023, max compression
```

## Comparing `chaincrafter-0.1.0.tar` & `chaincrafter-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-07 13:44:10.096815 chaincrafter-0.1.0/
--rw-r--r--   0 rudolfo    (501) staff       (20)     1058 2023-07-20 13:30:22.000000 chaincrafter-0.1.0/LICENSE
--rw-r--r--   0 rudolfo    (501) staff       (20)     1860 2023-08-07 13:44:10.096698 chaincrafter-0.1.0/PKG-INFO
--rw-r--r--   0 rudolfo    (501) staff       (20)      965 2023-08-07 13:39:00.000000 chaincrafter-0.1.0/README.md
-drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-07 13:44:10.096113 chaincrafter-0.1.0/chaincrafter/
--rw-r--r--   0 rudolfo    (501) staff       (20)      268 2023-07-22 16:22:56.000000 chaincrafter-0.1.0/chaincrafter/__init__.py
--rw-r--r--   0 rudolfo    (501) staff       (20)     2103 2023-08-05 02:51:56.000000 chaincrafter-0.1.0/chaincrafter/chains.py
--rw-r--r--   0 rudolfo    (501) staff       (20)     3571 2023-08-06 03:16:03.000000 chaincrafter-0.1.0/chaincrafter/experiments.py
--rw-r--r--   0 rudolfo    (501) staff       (20)     5434 2023-08-04 10:07:26.000000 chaincrafter-0.1.0/chaincrafter/models.py
--rw-r--r--   0 rudolfo    (501) staff       (20)     2989 2023-08-06 00:10:15.000000 chaincrafter-0.1.0/chaincrafter/prompts.py
-drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-07 13:44:10.096561 chaincrafter-0.1.0/chaincrafter.egg-info/
--rw-r--r--   0 rudolfo    (501) staff       (20)     1860 2023-08-07 13:44:10.000000 chaincrafter-0.1.0/chaincrafter.egg-info/PKG-INFO
--rw-r--r--   0 rudolfo    (501) staff       (20)      308 2023-08-07 13:44:10.000000 chaincrafter-0.1.0/chaincrafter.egg-info/SOURCES.txt
--rw-r--r--   0 rudolfo    (501) staff       (20)        1 2023-08-07 13:44:10.000000 chaincrafter-0.1.0/chaincrafter.egg-info/dependency_links.txt
--rw-r--r--   0 rudolfo    (501) staff       (20)       13 2023-08-07 13:44:10.000000 chaincrafter-0.1.0/chaincrafter.egg-info/top_level.txt
--rw-r--r--   0 rudolfo    (501) staff       (20)      808 2023-08-07 13:43:40.000000 chaincrafter-0.1.0/pyproject.toml
--rw-r--r--   0 rudolfo    (501) staff       (20)       38 2023-08-07 13:44:10.096854 chaincrafter-0.1.0/setup.cfg
--rw-r--r--   0 rudolfo    (501) staff       (20)      734 2023-08-07 13:43:12.000000 chaincrafter-0.1.0/setup.py
+drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-08 13:17:57.461087 chaincrafter-0.2.0/
+-rw-r--r--   0 rudolfo    (501) staff       (20)     1058 2023-07-20 13:30:22.000000 chaincrafter-0.2.0/LICENSE
+-rw-r--r--   0 rudolfo    (501) staff       (20)     2027 2023-08-08 13:17:57.460941 chaincrafter-0.2.0/PKG-INFO
+-rw-r--r--   0 rudolfo    (501) staff       (20)     1132 2023-08-07 13:49:11.000000 chaincrafter-0.2.0/README.md
+drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-08 13:17:57.460010 chaincrafter-0.2.0/chaincrafter/
+-rw-r--r--   0 rudolfo    (501) staff       (20)      268 2023-07-22 16:22:56.000000 chaincrafter-0.2.0/chaincrafter/__init__.py
+-rw-r--r--   0 rudolfo    (501) staff       (20)     2513 2023-08-08 00:14:28.000000 chaincrafter-0.2.0/chaincrafter/chains.py
+-rw-r--r--   0 rudolfo    (501) staff       (20)     3571 2023-08-06 03:16:03.000000 chaincrafter-0.2.0/chaincrafter/experiments.py
+-rw-r--r--   0 rudolfo    (501) staff       (20)     5448 2023-08-08 13:15:41.000000 chaincrafter-0.2.0/chaincrafter/models.py
+-rw-r--r--   0 rudolfo    (501) staff       (20)     2989 2023-08-07 23:16:21.000000 chaincrafter-0.2.0/chaincrafter/prompts.py
+drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-08 13:17:57.460645 chaincrafter-0.2.0/chaincrafter.egg-info/
+-rw-r--r--   0 rudolfo    (501) staff       (20)     2027 2023-08-08 13:17:57.000000 chaincrafter-0.2.0/chaincrafter.egg-info/PKG-INFO
+-rw-r--r--   0 rudolfo    (501) staff       (20)      332 2023-08-08 13:17:57.000000 chaincrafter-0.2.0/chaincrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 rudolfo    (501) staff       (20)        1 2023-08-08 13:17:57.000000 chaincrafter-0.2.0/chaincrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 rudolfo    (501) staff       (20)       13 2023-08-08 13:17:57.000000 chaincrafter-0.2.0/chaincrafter.egg-info/top_level.txt
+-rw-r--r--   0 rudolfo    (501) staff       (20)      808 2023-08-08 13:16:55.000000 chaincrafter-0.2.0/pyproject.toml
+-rw-r--r--   0 rudolfo    (501) staff       (20)       38 2023-08-08 13:17:57.461123 chaincrafter-0.2.0/setup.cfg
+-rw-r--r--   0 rudolfo    (501) staff       (20)      734 2023-08-08 13:16:50.000000 chaincrafter-0.2.0/setup.py
+drwxr-xr-x   0 rudolfo    (501) staff       (20)        0 2023-08-08 13:17:57.460763 chaincrafter-0.2.0/tests/
+-rw-r--r--   0 rudolfo    (501) staff       (20)      791 2023-08-08 13:15:41.000000 chaincrafter-0.2.0/tests/test_mock_chat.py
```

### Comparing `chaincrafter-0.1.0/LICENSE` & `chaincrafter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaincrafter-0.1.0/PKG-INFO` & `chaincrafter-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaincrafter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Seamless integration and composability for large language model apps.
 Home-page: https://github.com/rudolfolah/chaincrafter
 Author: Rudolf Olah
 Author-email: Rudolf Olah <rudolf.olah.to@gmail.com>
 Project-URL: Homepage, https://rudolfolah.github.io/chaincrafter/
 Project-URL: Bug Tracker, https://github.com/rudolfolah/chaincrafter/issues
 Project-URL: Repository, https://github.com/rudolfolah/chaincrafter
@@ -33,14 +33,17 @@
 
 The imports for the models should be part of the `__init__` or the `complete` method of the `ChatModel` class.
 
 ## Build and Publish
 
 * [Update classifiers in `pyproject.toml` and `setup.py`](https://pypi.org/classifiers/)
 * [Update project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata)
+* [Create an API token](https://pypi.org/manage/account/)
+  * Set your username to `__token__`
+  * Set your password to the token value, including the `pypi-` prefix 
 
 ```bash
 cd /path/to/chaincrafter/python
 pip install build
 python -m build
 
 pip install twine
```

### Comparing `chaincrafter-0.1.0/README.md` & `chaincrafter-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 The imports for the models should be part of the `__init__` or the `complete` method of the `ChatModel` class.
 
 ## Build and Publish
 
 * [Update classifiers in `pyproject.toml` and `setup.py`](https://pypi.org/classifiers/)
 * [Update project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata)
+* [Create an API token](https://pypi.org/manage/account/)
+  * Set your username to `__token__`
+  * Set your password to the token value, including the `pypi-` prefix 
 
 ```bash
 cd /path/to/chaincrafter/python
 pip install build
 python -m build
 
 pip install twine
```

### Comparing `chaincrafter-0.1.0/chaincrafter/chains.py` & `chaincrafter-0.2.0/chaincrafter/chains.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from collections import deque
+import logging
 from typing import TypedDict
 
 from chaincrafter.models import ChatModel
 from chaincrafter.prompts import Prompt
 
 
 Message = TypedDict('Message', {'role': str, 'content': str})
@@ -19,28 +20,38 @@
             in.
         """
         self._system_prompt = system_prompt
         self._prompts_and_output_keys = prompts_and_output_keys
 
     def run(self, chat_model: ChatModel, starting_input_vars: dict = {}) -> [Message]:
         """
-        Runs the chain.
+        Runs the chain. The output of each prompt is passed to the next prompt as a starting input variable.
+
+        Ensure that the keys of the starting input variables and the output are unique or they will be overwritten.
+
         :param chat_model: The LLM chat model to use.
         :param starting_input_vars: The starting input variables that are passed to the first prompt
             (not the system prompt)
         :return: The messages that were sent back and forth between the user and the system.
         """
         queue = deque(self._prompts_and_output_keys)
+
         input_vars = {key: value for key, value in starting_input_vars.items()}
+        logging.debug(f"Starting input variables: {input_vars}")
+
         messages = [
             {"role": "system", "content": self._system_prompt.build(**input_vars)}
         ]
         while queue:
             human_prompt, output_key = queue.popleft()
             messages.append({"role": "user", "content": human_prompt.build(**input_vars)})
             response = chat_model.complete(messages)
-            input_vars = {output_key: response}
+
+            if output_key in input_vars:
+                logging.warning(f"Overwriting input variable {output_key}")
+
+            input_vars.update({output_key: response})
             messages.append({"role": "assistant", "content": response})
         return messages
 
     async def async_run(self, chat_model: ChatModel, starting_input_vars: dict = {}) -> [Message]:
         return await asyncio.to_thread(self.run, chat_model, starting_input_vars)
```

### Comparing `chaincrafter-0.1.0/chaincrafter/experiments.py` & `chaincrafter-0.2.0/chaincrafter/experiments.py`

 * *Files identical despite different names*

### Comparing `chaincrafter-0.1.0/chaincrafter/models.py` & `chaincrafter-0.2.0/chaincrafter/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 # Mock Models
 class MockChat(ChatModel):
     def __init__(self, temperature, model_name):
         self._temperature = temperature
         self._model_name = model_name
         self._mock_responses = []
 
-    def mock_responses(self, messages: [dict]):
+    def mock_responses(self, messages: [str]):
         self._mock_responses = messages
 
-    def complete(self, messages):
+    def complete(self, messages: [dict]) -> str:
         return self._mock_responses.pop(0)
 
 
 # Integration Models
 class LlamaCppChat(ChatModel):
     """
     A chat model that uses the llama.cpp library.
```

### Comparing `chaincrafter-0.1.0/chaincrafter/prompts.py` & `chaincrafter-0.2.0/chaincrafter/prompts.py`

 * *Files identical despite different names*

### Comparing `chaincrafter-0.1.0/chaincrafter.egg-info/PKG-INFO` & `chaincrafter-0.2.0/chaincrafter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaincrafter
-Version: 0.1.0
+Version: 0.2.0
 Summary: Seamless integration and composability for large language model apps.
 Home-page: https://github.com/rudolfolah/chaincrafter
 Author: Rudolf Olah
 Author-email: Rudolf Olah <rudolf.olah.to@gmail.com>
 Project-URL: Homepage, https://rudolfolah.github.io/chaincrafter/
 Project-URL: Bug Tracker, https://github.com/rudolfolah/chaincrafter/issues
 Project-URL: Repository, https://github.com/rudolfolah/chaincrafter
@@ -33,14 +33,17 @@
 
 The imports for the models should be part of the `__init__` or the `complete` method of the `ChatModel` class.
 
 ## Build and Publish
 
 * [Update classifiers in `pyproject.toml` and `setup.py`](https://pypi.org/classifiers/)
 * [Update project metadata](https://packaging.python.org/en/latest/specifications/declaring-project-metadata/#declaring-project-metadata)
+* [Create an API token](https://pypi.org/manage/account/)
+  * Set your username to `__token__`
+  * Set your password to the token value, including the `pypi-` prefix 
 
 ```bash
 cd /path/to/chaincrafter/python
 pip install build
 python -m build
 
 pip install twine
```

### Comparing `chaincrafter-0.1.0/pyproject.toml` & `chaincrafter-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chaincrafter"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Rudolf Olah", email="rudolf.olah.to@gmail.com" },
 ]
 description = "Seamless integration and composability for large language model apps."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `chaincrafter-0.1.0/setup.py` & `chaincrafter-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chaincrafter",
-    version="0.1.0",
+    version="0.2.0",
     description="Seamless integration and composability for large language model apps.",
     long_description="Seamless integration and composability for large language model apps.",
     author="Rudolf Olah",
     author_email="rudolf.olah.to@gmail.com",
     url="https://github.com/rudolfolah/chaincrafter",
     packages=find_packages(),
     classifiers=[
```


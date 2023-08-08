# Comparing `tmp/easycompletion-0.3.6.tar.gz` & `tmp/easycompletion-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.3.6.tar", last modified: Thu Aug  3 05:54:32 2023, max compression
+gzip compressed data, was "easycompletion-0.4.0.tar", last modified: Tue Aug  8 02:50:20 2023, max compression
```

## Comparing `easycompletion-0.3.6.tar` & `easycompletion-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 05:54:20.000000 easycompletion-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 05:54:32.375574 easycompletion-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-08-03 05:54:20.000000 easycompletion-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-08-03 05:54:20.000000 easycompletion-0.3.6/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 05:54:32.375574 easycompletion-0.3.6/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 05:54:32.000000 easycompletion-0.3.6/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 05:54:32.375574 easycompletion-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-03 05:54:20.000000 easycompletion-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:50:20.446068 easycompletion-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 02:50:10.000000 easycompletion-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-08 02:50:20.446068 easycompletion-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-08-08 02:50:10.000000 easycompletion-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:50:20.446068 easycompletion-0.4.0/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-08 02:50:10.000000 easycompletion-0.4.0/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 02:50:10.000000 easycompletion-0.4.0/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-08 02:50:10.000000 easycompletion-0.4.0/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-08-08 02:50:10.000000 easycompletion-0.4.0/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-08-08 02:50:10.000000 easycompletion-0.4.0/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:50:20.446068 easycompletion-0.4.0/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-08 02:50:20.000000 easycompletion-0.4.0/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-08 02:50:20.000000 easycompletion-0.4.0/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:50:20.000000 easycompletion-0.4.0/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 02:50:20.000000 easycompletion-0.4.0/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 02:50:20.000000 easycompletion-0.4.0/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:50:20.446068 easycompletion-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-08 02:50:10.000000 easycompletion-0.4.0/setup.py
```

### Comparing `easycompletion-0.3.6/LICENSE` & `easycompletion-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.6/PKG-INFO` & `easycompletion-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.6
+Version: 0.4.0
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -50,14 +50,24 @@
 # Call the function
 response = function_completion(text="Write a song about AI", functions=[test_function], function_call="write_song")
 
 # Print the response
 print(response["arguments"]["lyrics"])
 ```
 
+# Using With Llama v2 and Local Models
+easycompletion has been tested with LocalAI [LocalAI](https://localai.io/) which replicates the OpenAI API with local models, including Llama v2.
+
+Follow instructions for setting up LocalAI and then set the following environment variable:
+
+```bash
+export EASYCOMPLETION_API_ENDPOINT=localhost:8000
+```
+
+
 # Basic Usage
 
 ## Compose Prompt
 
 You can compose a prompt using {{handlebars}} syntax
 
 ```python
@@ -218,15 +228,15 @@
     "total_tokens": "number"
   },
   "finish_reason": "string",
   "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
@@ -234,23 +244,23 @@
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `count_tokens(prompt, model=TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `get_tokens(prompt, model=TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
 
@@ -260,21 +270,21 @@
 
 ```python
 prompt = compose_prompt("Hello {{name}}!", {"name": "John"})
 ```
 
 ## A note about models
 
-You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `OPENAI_MODEL` environment variable.
+You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `EASYCOMPLETION_TEXT_MODEL` environment variable.
 
 Default model is gpt-turbo-3.5-0613.
 
 ## A note about API keys
 
-You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `OPENAI_API_KEY` environment variable will be checked.
+You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `EASYCOMPLETION_API_KEY` environment variable will be checked.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
 ```
```

### Comparing `easycompletion-0.3.6/README.md` & `easycompletion-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 # Call the function
 response = function_completion(text="Write a song about AI", functions=[test_function], function_call="write_song")
 
 # Print the response
 print(response["arguments"]["lyrics"])
 ```
 
+# Using With Llama v2 and Local Models
+easycompletion has been tested with LocalAI [LocalAI](https://localai.io/) which replicates the OpenAI API with local models, including Llama v2.
+
+Follow instructions for setting up LocalAI and then set the following environment variable:
+
+```bash
+export EASYCOMPLETION_API_ENDPOINT=localhost:8000
+```
+
+
 # Basic Usage
 
 ## Compose Prompt
 
 You can compose a prompt using {{handlebars}} syntax
 
 ```python
@@ -202,15 +212,15 @@
     "total_tokens": "number"
   },
   "finish_reason": "string",
   "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
@@ -218,23 +228,23 @@
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `count_tokens(prompt, model=TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `get_tokens(prompt, model=TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
 
@@ -244,21 +254,21 @@
 
 ```python
 prompt = compose_prompt("Hello {{name}}!", {"name": "John"})
 ```
 
 ## A note about models
 
-You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `OPENAI_MODEL` environment variable.
+You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `EASYCOMPLETION_TEXT_MODEL` environment variable.
 
 Default model is gpt-turbo-3.5-0613.
 
 ## A note about API keys
 
-You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `OPENAI_API_KEY` environment variable will be checked.
+You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `EASYCOMPLETION_API_KEY` environment variable will be checked.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
 ```
```

#### html2text {}

```diff
@@ -9,45 +9,49 @@
 from easycompletion import function_completion, text_completion, compose_prompt
 # Compose a function object test_function = compose_function
 ( name="write_song", description="Write a song about AI", properties=
 { "lyrics": { "type": "string", "description": "The lyrics for the song", } },
 required_properties: ["lyrics"], ) # Call the function response =
 function_completion(text="Write a song about AI", functions=[test_function],
 function_call="write_song") # Print the response print(response["arguments"]
-["lyrics"]) ``` # Basic Usage ## Compose Prompt You can compose a prompt using
-{{handlebars}} syntax ```python test_prompt = "Don't forget your {{object}}"
-test_dict = {"object": "towel"} prompt = compose_prompt(test_prompt, test_dict)
-# prompt = "Don't forget your towel" ``` ## Text Completion Send text, get a
-response as a text string ```python from easycompletion import text_completion
-response = text_completion("Hello, how are you?") # response["text"] = "As an
-AI language model, I don't have feelings, but..."" ``` ## Compose a Function
-Compose a function to pass into the function calling API ```python from
-easycompletion import compose_function test_function = compose_function
-( name="write_song", description="Write a song about AI", properties=
-{ "lyrics": { "type": "string", "description": "The lyrics for the song", } },
-required_properties: ["lyrics"], ) ``` ## Function Completion Send text and a
-list of functions and get a response as a function call ```python from
-easycompletion import function_completion, compose_function # NOTE:
-test_function is a function object created using compose_function in the
-example above... response = function_completion(text="Write a song about AI",
-functions=[test_function], function_call="write_song") # Response structure is
-{ "text": string, "function_name": string, "arguments": dict } print(response
-["arguments"]["lyrics"]) ``` # Advanced Usage ### `compose_function(name,
-description, properties, required_properties)` Composes a function object for
-function completions. ```python summarization_function = compose_function
-( name="summarize_text", description="Summarize the text. Include the topic,
-subtopics.", properties={ "summary": { "type": "string", "description":
-"Detailed summary of the text.", }, }, required_properties=["summary"], ) ```
-### `chat_completion(text, model_failure_retries=5, model=None,
-chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)` Send a list of messages as a
-chat and returns a text response. ```python response = chat_completion
-( messages = [{ "user": "Hello, how are you?"}], system_message = "You are a
-towel. Respond as a towel.", model_failure_retries=3, model='gpt-3.5-turbo',
-chunk_length=1024, api_key='your_openai_api_key' ) ``` The response object
-looks like this: ```json { "text": "string", "usage": { "prompt_tokens":
+["lyrics"]) ``` # Using With Llama v2 and Local Models easycompletion has been
+tested with LocalAI [LocalAI](https://localai.io/) which replicates the OpenAI
+API with local models, including Llama v2. Follow instructions for setting up
+LocalAI and then set the following environment variable: ```bash export
+EASYCOMPLETION_API_ENDPOINT=localhost:8000 ``` # Basic Usage ## Compose Prompt
+You can compose a prompt using {{handlebars}} syntax ```python test_prompt =
+"Don't forget your {{object}}" test_dict = {"object": "towel"} prompt =
+compose_prompt(test_prompt, test_dict) # prompt = "Don't forget your towel" ```
+## Text Completion Send text, get a response as a text string ```python from
+easycompletion import text_completion response = text_completion("Hello, how
+are you?") # response["text"] = "As an AI language model, I don't have
+feelings, but..."" ``` ## Compose a Function Compose a function to pass into
+the function calling API ```python from easycompletion import compose_function
+test_function = compose_function( name="write_song", description="Write a song
+about AI", properties={ "lyrics": { "type": "string", "description": "The
+lyrics for the song", } }, required_properties: ["lyrics"], ) ``` ## Function
+Completion Send text and a list of functions and get a response as a function
+call ```python from easycompletion import function_completion, compose_function
+# NOTE: test_function is a function object created using compose_function in
+the example above... response = function_completion(text="Write a song about
+AI", functions=[test_function], function_call="write_song") # Response
+structure is { "text": string, "function_name": string, "arguments": dict }
+print(response["arguments"]["lyrics"]) ``` # Advanced Usage ###
+`compose_function(name, description, properties, required_properties)` Composes
+a function object for function completions. ```python summarization_function =
+compose_function( name="summarize_text", description="Summarize the text.
+Include the topic, subtopics.", properties={ "summary": { "type": "string",
+"description": "Detailed summary of the text.", }, }, required_properties=
+["summary"], ) ``` ### `chat_completion(text, model_failure_retries=5,
+model=None, chunk_length=DEFAULT_CHUNK_LENGTH, api_key=None)` Send a list of
+messages as a chat and returns a text response. ```python response =
+chat_completion( messages = [{ "user": "Hello, how are you?"}], system_message
+= "You are a towel. Respond as a towel.", model_failure_retries=3, model='gpt-
+3.5-turbo', chunk_length=1024, api_key='your_openai_api_key' ) ``` The response
+object looks like this: ```json { "text": "string", "usage": { "prompt_tokens":
 "number", "completion_tokens": "number", "total_tokens": "number" }, "error":
 "string|None", "finish_reason": "string" } ``` ### `text_completion(text,
 model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH,
 api_key=None)` Sends text to the model and returns a text response. ```python
 response = text_completion( "Hello, how are you?", model_failure_retries=3,
 model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key' ) ```
 The response object looks like this: ```json { "text": "string", "usage":
@@ -62,34 +66,35 @@
 call. If messages are provided, the "text" becomes the last user message in the
 list. ```python function = { 'name': 'function1', 'parameters': {'param1':
 'value1'} } response = function_completion("Call the function.", function) ```
 The response object looks like this: ```json { "text": "string",
 "function_name": "string", "arguments": "dict", "usage": { "prompt_tokens":
 "number", "completion_tokens": "number", "total_tokens": "number" },
 "finish_reason": "string", "error": "string|None" } ``` ### `trim_prompt(text,
-max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
-Trim the given text to a maximum number of tokens. ```python trimmed_text =
-trim_prompt("This is a test.", 3, preserve_top=True) ``` ### `chunk_prompt
-(prompt, chunk_length=DEFAULT_CHUNK_LENGTH)` Split the given prompt into chunks
-where each chunk has a maximum number of tokens. ```python prompt_chunks =
+max_tokens=DEFAULT_CHUNK_LENGTH, model=TEXT_MODEL, preserve_top=True)` Trim the
+given text to a maximum number of tokens. ```python trimmed_text = trim_prompt
+("This is a test.", 3, preserve_top=True) ``` ### `chunk_prompt(prompt,
+chunk_length=DEFAULT_CHUNK_LENGTH)` Split the given prompt into chunks where
+each chunk has a maximum number of tokens. ```python prompt_chunks =
 chunk_prompt("This is a test. I am writing a function.", 4) ``` ###
-`count_tokens(prompt, model=DEFAULT_TEXT_MODEL)` Count the number of tokens in
-a string. ```python num_tokens = count_tokens("This is a test.") ``` ###
-`get_tokens(prompt, model=DEFAULT_TEXT_MODEL)` Returns a list of tokens in a
-string. ```python tokens = get_tokens("This is a test.") ``` ###
-`compose_prompt(prompt_template, parameters)` Composes a prompt using a
-template and parameters. Parameter keys are enclosed in double curly brackets
-and replaced with parameter values. ```python prompt = compose_prompt("Hello {
-{name}}!", {"name": "John"}) ``` ## A note about models You can pass in a model
-using the `model` parameter of either function_completion or text_completion.
-If you do not pass in a model, the default model will be used. You can also
-override this by setting the environment model via `OPENAI_MODEL` environment
+`count_tokens(prompt, model=TEXT_MODEL)` Count the number of tokens in a
+string. ```python num_tokens = count_tokens("This is a test.") ``` ###
+`get_tokens(prompt, model=TEXT_MODEL)` Returns a list of tokens in a string.
+```python tokens = get_tokens("This is a test.") ``` ### `compose_prompt
+(prompt_template, parameters)` Composes a prompt using a template and
+parameters. Parameter keys are enclosed in double curly brackets and replaced
+with parameter values. ```python prompt = compose_prompt("Hello {{name}}!",
+{"name": "John"}) ``` ## A note about models You can pass in a model using the
+`model` parameter of either function_completion or text_completion. If you do
+not pass in a model, the default model will be used. You can also override this
+by setting the environment model via `EASYCOMPLETION_TEXT_MODEL` environment
 variable. Default model is gpt-turbo-3.5-0613. ## A note about API keys You can
 pass in an API key using the `api_key` parameter of either function_completion
-or text_completion. If you do not pass in an API key, the `OPENAI_API_KEY`
-environment variable will be checked. # Publishing ```bash bash publish.sh --
-version= --username= --password= ``` # Contributions Welcome If you like this
-library and want to contribute in any way, please feel free to submit a PR and
-I will review it. Please note that the goal here is simplicity and
-accesibility, using common language and few dependencies. # Questions,
-Comments, Concerns If you have any questions, please feel free to reach out to
-me on [Twitter](https://twitter.com/spatialweeb) or Discord @new.moon
+or text_completion. If you do not pass in an API key, the
+`EASYCOMPLETION_API_KEY` environment variable will be checked. # Publishing
+```bash bash publish.sh --version= --username= --password= ``` # Contributions
+Welcome If you like this library and want to contribute in any way, please feel
+free to submit a PR and I will review it. Please note that the goal here is
+simplicity and accesibility, using common language and few dependencies. #
+Questions, Comments, Concerns If you have any questions, please feel free to
+reach out to me on [Twitter](https://twitter.com/spatialweeb) or Discord
+@new.moon
```

### Comparing `easycompletion-0.3.6/easycompletion/__init__.py` & `easycompletion-0.4.0/easycompletion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     chunk_prompt,
     count_tokens,
     compose_function,
     get_tokens,
 )
 
 from .constants import (
-    DEFAULT_TEXT_MODEL,
+    TEXT_MODEL,
     DEFAULT_CHUNK_LENGTH,
 )
 
 __all__ = [
     "function_completion",
     "text_completion",
     "chat_completion",
@@ -29,10 +29,10 @@
     "openai_text_call",
     "compose_prompt",
     "compose_function",
     "trim_prompt",
     "chunk_prompt",
     "count_tokens",
     "get_tokens",
-    "DEFAULT_TEXT_MODEL",
+    "TEXT_MODEL",
     "DEFAULT_CHUNK_LENGTH",
 ]
```

### Comparing `easycompletion-0.3.6/easycompletion/constants.py` & `easycompletion-0.4.0/easycompletion/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()  # take environment variables from .env.
 
-DEFAULT_TEXT_MODEL = os.getenv("OPENAI_MODEL")
-if DEFAULT_TEXT_MODEL == None or DEFAULT_TEXT_MODEL == "":
-    DEFAULT_TEXT_MODEL = "gpt-3.5-turbo-0613"
-LONG_TEXT_MODEL = os.getenv("OPENAI_MODEL_16K")
+TEXT_MODEL = os.getenv("EASYCOMPLETION_TEXT_MODEL")
+if TEXT_MODEL == None or TEXT_MODEL == "":
+    TEXT_MODEL = "gpt-3.5-turbo-0613"
+LONG_TEXT_MODEL = os.getenv("EASYCOMPLETION_LONG_TEXT_MODEL")
 if LONG_TEXT_MODEL == None or LONG_TEXT_MODEL == "":
     LONG_TEXT_MODEL = "gpt-3.5-turbo-16k"
 
-OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
+EASYCOMPLETION_API_KEY = os.getenv("OPENAI_API_KEY") or os.getenv("EASYCOMPLETION_API_KEY")
 
-DEBUG = os.environ.get("DEBUG") == "true" or os.environ.get("DEBUG") == "True"
+EASYCOMPLETION_API_ENDPOINT = os.getenv("EASYCOMPLETION_API_ENDPOINT") or "https://api.openai.com/v1"
+
+DEBUG = os.environ.get("EASYCOMPLETION_DEBUG") == "true" or os.environ.get("EASYCOMPLETION_DEBUG") == "True"
 
 DEFAULT_CHUNK_LENGTH = 4096 * 3 / 4  # 3/4ths of the context window size
```

### Comparing `easycompletion-0.3.6/easycompletion/logger.py` & `easycompletion-0.4.0/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.6/easycompletion/model.py` & `easycompletion-0.4.0/easycompletion/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 from dotenv import load_dotenv
 
 # Load environment variables from .env file
 load_dotenv()
 
 from .constants import (
-    DEFAULT_TEXT_MODEL,
+    EASYCOMPLETION_API_ENDPOINT,
+    TEXT_MODEL,
     LONG_TEXT_MODEL,
-    OPENAI_API_KEY,
+    EASYCOMPLETION_API_KEY,
     DEFAULT_CHUNK_LENGTH,
     DEBUG,
 )
 
 from .logger import log
 
 from .prompt import count_tokens
 
-# Set the OpenAI API key
-openai.api_key = OPENAI_API_KEY
-
+openai.api_key = EASYCOMPLETION_API_KEY
+openai.api_base = EASYCOMPLETION_API_ENDPOINT
 
 def parse_arguments(arguments, debug=DEBUG):
     """
     Parses arguments that are expected to be either a JSON string, dictionary, or a list.
 
     Parameters:
         arguments (str or dict or list): Arguments in string or dictionary or list format.
@@ -166,15 +166,15 @@
 ):
     """
     Function for sending chat messages and returning a chat response.
 
     Parameters:
         messages (str): Messages to send to the model. In the form {<role>: string, <content>: string} - roles are "user" and "assistant"
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
-        model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
+        model (str, optional): The model to use. Default is the TEXT_MODEL defined in constants.py.
         chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
         api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
     Returns:
         str: The response content from the model.
 
     Example:
@@ -183,15 +183,15 @@
 
     # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
     # Use the default model if no model is specified
     if model == None:
-        model = DEFAULT_TEXT_MODEL
+        model = TEXT_MODEL
 
     # Count tokens in the input text
     total_tokens = count_tokens(messages, model=model)
 
     # If text is longer than chunk_length and model is not for long texts, switch to the long text model
     if total_tokens > chunk_length and "16k" not in model:
         model = LONG_TEXT_MODEL
@@ -261,15 +261,15 @@
 ):
     """
     Function for sending text and returning a text completion response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
-        model (str, optional): The model to use. Default is the DEFAULT_TEXT_MODEL defined in constants.py.
+        model (str, optional): The model to use. Default is the TEXT_MODEL defined in constants.py.
         chunk_length (int, optional): Maximum length of text chunk to process. Default is defined in constants.py.
         api_key (str, optional): OpenAI API key. If not provided, it uses the one defined in constants.py.
 
     Returns:
         str: The response content from the model.
 
     Example:
@@ -278,15 +278,15 @@
 
     # Override the API key if provided as parameter
     if api_key is not None:
         openai.api_key = api_key
 
     # Use the default model if no model is specified
     if model == None:
-        model = DEFAULT_TEXT_MODEL
+        model = TEXT_MODEL
 
     # Count tokens in the input text
     total_tokens = count_tokens(text, model=model)
 
     # If text is longer than chunk_length and model is not for long texts, switch to the long text model
     if total_tokens > chunk_length and "16k" not in model:
         model = LONG_TEXT_MODEL
@@ -372,16 +372,16 @@
     Args:
         text (str): Text that will be sent as the user message to the model.
         functions (list[dict] | dict | None): List of functions or a single function dictionary to be sent to the model.
         model_failure_retries (int): Number of times to retry the request if it fails (default is 5).
         function_call (str | dict | None): 'auto' to let the model decide, or a function name or a dictionary containing the function name (default is "auto").
         function_failure_retries (int): Number of times to retry the request if the function call is invalid (default is 10).
         chunk_length (int): The length of each chunk to be processed.
-        model (str | None): The model to use (default is the DEFAULT_TEXT_MODEL, i.e. gpt-3.5-turbo).
-        api_key (str | None): If you'd like to pass in a key to override the environment variable OPENAI_API_KEY.
+        model (str | None): The model to use (default is the TEXT_MODEL, i.e. gpt-3.5-turbo).
+        api_key (str | None): If you'd like to pass in a key to override the environment variable EASYCOMPLETION_API_KEY.
 
     Returns:
         dict: On most errors, returns a dictionary with an "error" key. On success, returns a dictionary containing
         "text" (response from the model), "function_name" (name of the function called), "arguments" (arguments for the function), "error" (None).
 
     Example:
         >>> function = {'name': 'function1', 'parameters': {'param1': 'value1'}}
@@ -444,15 +444,15 @@
             log("function_call must have a name property", type="error", log=debug)
             return {
                 "error": "function_call had an invalid name. Should be a string of the function name or an object with a name property"
             }
 
     # Use the default text model if no model is specified
     if model is None:
-        model = DEFAULT_TEXT_MODEL
+        model = TEXT_MODEL
 
     # Count the number of tokens in the message
     message_tokens = count_tokens(text, model=model)
     total_tokens = message_tokens
 
     function_call_tokens = count_tokens(functions, model=model)
     total_tokens += function_call_tokens + 3  # Additional tokens for the user
```

### Comparing `easycompletion-0.3.6/easycompletion/prompt.py` & `easycompletion-0.4.0/easycompletion/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 import tiktoken
 
-from .constants import DEFAULT_TEXT_MODEL, DEFAULT_CHUNK_LENGTH, DEBUG
+from .constants import TEXT_MODEL, DEFAULT_CHUNK_LENGTH, DEBUG
 from .logger import log
 
 
 def trim_prompt(
     text,
     max_tokens=DEFAULT_CHUNK_LENGTH,
-    model=DEFAULT_TEXT_MODEL,
+    model=TEXT_MODEL,
     preserve_top=True,
     debug=DEBUG,
 ):
     """
     Trim the given text to a maximum number of tokens.
 
     Args:
@@ -89,15 +89,15 @@
         type="warning",
         log=debug,
     )
 
     return prompt_chunks
 
 
-def count_tokens(prompt: str, model=DEFAULT_TEXT_MODEL) -> int:
+def count_tokens(prompt: str, model=TEXT_MODEL) -> int:
     """
     Count the number of tokens in a string.
 
     Args:
         prompt: The string to be tokenized.
         model: The model to use for tokenization.
 
@@ -114,15 +114,15 @@
     encoding = tiktoken.encoding_for_model(model)
     length = len(
         encoding.encode(prompt)
     )  # Encoding the text into tokens and counting the number of tokens.
     return length
 
 
-def get_tokens(prompt: str, model=DEFAULT_TEXT_MODEL) -> list:
+def get_tokens(prompt: str, model=TEXT_MODEL) -> list:
     """
     Returns a list of tokens in a string.
 
     Args:
         prompt: The string to be tokenized.
         model: The model to use for tokenization.
```

### Comparing `easycompletion-0.3.6/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.4.0/easycompletion.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.6
+Version: 0.4.0
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -50,14 +50,24 @@
 # Call the function
 response = function_completion(text="Write a song about AI", functions=[test_function], function_call="write_song")
 
 # Print the response
 print(response["arguments"]["lyrics"])
 ```
 
+# Using With Llama v2 and Local Models
+easycompletion has been tested with LocalAI [LocalAI](https://localai.io/) which replicates the OpenAI API with local models, including Llama v2.
+
+Follow instructions for setting up LocalAI and then set the following environment variable:
+
+```bash
+export EASYCOMPLETION_API_ENDPOINT=localhost:8000
+```
+
+
 # Basic Usage
 
 ## Compose Prompt
 
 You can compose a prompt using {{handlebars}} syntax
 
 ```python
@@ -218,15 +228,15 @@
     "total_tokens": "number"
   },
   "finish_reason": "string",
   "error": "string|None"
 }
 ```
 
-### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
+### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH, model=TEXT_MODEL, preserve_top=True)`
 
 Trim the given text to a maximum number of tokens.
 
 ```python
 trimmed_text = trim_prompt("This is a test.", 3, preserve_top=True)
 ```
 
@@ -234,23 +244,23 @@
 
 Split the given prompt into chunks where each chunk has a maximum number of tokens.
 
 ```python
 prompt_chunks = chunk_prompt("This is a test. I am writing a function.", 4)
 ```
 
-### `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `count_tokens(prompt, model=TEXT_MODEL)`
 
 Count the number of tokens in a string.
 
 ```python
 num_tokens = count_tokens("This is a test.")
 ```
 
-### `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)`
+### `get_tokens(prompt, model=TEXT_MODEL)`
 
 Returns a list of tokens in a string.
 
 ```python
 tokens = get_tokens("This is a test.")
 ```
 
@@ -260,21 +270,21 @@
 
 ```python
 prompt = compose_prompt("Hello {{name}}!", {"name": "John"})
 ```
 
 ## A note about models
 
-You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `OPENAI_MODEL` environment variable.
+You can pass in a model using the `model` parameter of either function_completion or text_completion. If you do not pass in a model, the default model will be used. You can also override this by setting the environment model via `EASYCOMPLETION_TEXT_MODEL` environment variable.
 
 Default model is gpt-turbo-3.5-0613.
 
 ## A note about API keys
 
-You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `OPENAI_API_KEY` environment variable will be checked.
+You can pass in an API key using the `api_key` parameter of either function_completion or text_completion. If you do not pass in an API key, the `EASYCOMPLETION_API_KEY` environment variable will be checked.
 
 # Publishing
 
 ```bash
 bash publish.sh --version=<version> --username=<pypi_username> --password=<pypi_password>
 ```
```

### Comparing `easycompletion-0.3.6/setup.py` & `easycompletion-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.3.6',
+    version='0.4.0',
     description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```


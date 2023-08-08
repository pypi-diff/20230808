# Comparing `tmp/bandolier-0.1.2.tar.gz` & `tmp/bandolier-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandolier-0.1.2.tar", last modified: Sun Aug  6 16:11:34 2023, max compression
+gzip compressed data, was "bandolier-0.1.3.tar", last modified: Tue Aug  8 02:07:46 2023, max compression
```

## Comparing `bandolier-0.1.2.tar` & `bandolier-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 16:11:34.070922 bandolier-0.1.2/
--rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.1.2/LICENSE
--rw-r--r--   0 jlb        (501) staff       (20)     4227 2023-08-06 16:11:34.070791 bandolier-0.1.2/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)     3560 2023-08-06 16:09:11.000000 bandolier-0.1.2/README.md
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 16:11:34.069952 bandolier-0.1.2/bandolier/
--rw-r--r--   0 jlb        (501) staff       (20)       87 2023-08-04 08:58:50.000000 bandolier-0.1.2/bandolier/__init__.py
--rw-r--r--   0 jlb        (501) staff       (20)     4693 2023-08-06 16:10:53.000000 bandolier-0.1.2/bandolier/bandolier.py
-drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-06 16:11:34.070588 bandolier-0.1.2/bandolier.egg-info/
--rw-r--r--   0 jlb        (501) staff       (20)     4227 2023-08-06 16:11:34.000000 bandolier-0.1.2/bandolier.egg-info/PKG-INFO
--rw-r--r--   0 jlb        (501) staff       (20)      235 2023-08-06 16:11:34.000000 bandolier-0.1.2/bandolier.egg-info/SOURCES.txt
--rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-06 16:11:34.000000 bandolier-0.1.2/bandolier.egg-info/dependency_links.txt
--rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-06 16:11:34.000000 bandolier-0.1.2/bandolier.egg-info/requires.txt
--rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-06 16:11:34.000000 bandolier-0.1.2/bandolier.egg-info/top_level.txt
--rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-06 16:11:34.070962 bandolier-0.1.2/setup.cfg
--rw-r--r--   0 jlb        (501) staff       (20)     1190 2023-08-06 16:11:10.000000 bandolier-0.1.2/setup.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-08 02:07:46.081811 bandolier-0.1.3/
+-rw-r--r--   0 jlb        (501) staff       (20)     1082 2023-08-04 06:08:50.000000 bandolier-0.1.3/LICENSE
+-rw-r--r--   0 jlb        (501) staff       (20)     4157 2023-08-08 02:07:46.081561 bandolier-0.1.3/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)     3491 2023-08-07 17:22:28.000000 bandolier-0.1.3/README.md
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-08 02:07:46.080480 bandolier-0.1.3/bandolier/
+-rw-r--r--   0 jlb        (501) staff       (20)      150 2023-08-07 17:15:48.000000 bandolier-0.1.3/bandolier/__init__.py
+-rw-r--r--   0 jlb        (501) staff       (20)     1401 2023-08-07 16:33:50.000000 bandolier-0.1.3/bandolier/annotations.py
+-rw-r--r--   0 jlb        (501) staff       (20)     3470 2023-08-07 17:15:38.000000 bandolier-0.1.3/bandolier/bandolier.py
+-rw-r--r--   0 jlb        (501) staff       (20)     1251 2023-08-07 17:15:13.000000 bandolier-0.1.3/bandolier/conversation.py
+drwxr-xr-x   0 jlb        (501) staff       (20)        0 2023-08-08 02:07:46.081291 bandolier-0.1.3/bandolier.egg-info/
+-rw-r--r--   0 jlb        (501) staff       (20)     4157 2023-08-08 02:07:46.000000 bandolier-0.1.3/bandolier.egg-info/PKG-INFO
+-rw-r--r--   0 jlb        (501) staff       (20)      286 2023-08-08 02:07:46.000000 bandolier-0.1.3/bandolier.egg-info/SOURCES.txt
+-rw-r--r--   0 jlb        (501) staff       (20)        1 2023-08-08 02:07:46.000000 bandolier-0.1.3/bandolier.egg-info/dependency_links.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       47 2023-08-08 02:07:46.000000 bandolier-0.1.3/bandolier.egg-info/requires.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       10 2023-08-08 02:07:46.000000 bandolier-0.1.3/bandolier.egg-info/top_level.txt
+-rw-r--r--   0 jlb        (501) staff       (20)       38 2023-08-08 02:07:46.081899 bandolier-0.1.3/setup.cfg
+-rw-r--r--   0 jlb        (501) staff       (20)     1190 2023-08-08 02:07:38.000000 bandolier-0.1.3/setup.py
```

### Comparing `bandolier-0.1.2/LICENSE` & `bandolier-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bandolier-0.1.2/PKG-INFO` & `bandolier-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandolier
-Version: 0.1.2
+Version: 0.1.3
 Summary: A helper for OpenAI functions
 Home-page: https://github.com/johnnysands/bandolier
 Author: Johnny Sands
 Author-email: johnnysands@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -17,37 +17,31 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # Bandolier
 
 Bandolier is a library to make it easier to deal with OpenAI ChatGPT functions.
 
-To expose functions to OpenAI GPT services, we need to tell OpenAI about the
-functions.  Ideally we could simply inspect the functions and use that information
-to communicate to OpenAI, but unfortunately all the information we need isn't
-available.
-
-Type annotations could get us part of the way there, but they don't solve the
-whole problem, and they can't represent some of more complex data structures
-it's possible to use with ChatGPT.
-
-Bandolier uses decorators to add annotations to functions with the missing
-information.  These annotations are also validated against the information
-that we can get via introspection, helping your code and configuration
-stay in sync.
+There are two key classes:
 
-Bandolier also provides some convenience functions for working with OpenAI's APIs.
-It helps you manage message history and process requests for function calls automatically.
+Bandolier tracks the information on your functions and helps you build the
+prompts you need to expose the functions to the chat interface.
+
+Conversation stores your message history.  Bandolier uses the Conversation to
+build prompts with appropriate history. You can use a different Conversation
+in each call to Bandolier to make it easier to manage multiple conversation
+streams.
 
 ## Example
 
 ```python
-from bandolier import Bandolier, annotate_arguments, annotate_description
+from bandolier import Bandolier, Conversation, annotate_arguments, annotate_description
 
 
+# First set up your functions
 @annotate_arguments(
     {
         "location": {
             "type": "string",
             "description": "The city and state, e.g. San Francisco, CA.",
         },
         "unit": {
@@ -55,46 +49,54 @@
             "description": "The unit to return the temperature in, e.g. F or C.",
             "default": "F",
         },
     }
 )
 @annotate_description("Get the weather for a location.")
 def get_weather(location, unit="F"):
+    # api call here...
     return {"temperature": 72, unit: unit, "conditions": ["sunny", "windy"]}
 
 
 # can also use docstring for description
 def get_location():
     """Get the user's location."""
+    # api call here...
     return "San Francisco, CA"
 
 
 def main():
+    # Set up the bandolier function configuration
     bandolier = Bandolier()
     bandolier.add_function(get_weather)
     bandolier.add_function(get_location)
-    bandolier.add_system_message("You are a helpful assistant.")
+
+    # create a new conversational conversation
+    conversation = Conversation()
+    conversation.add_system_message("You are a helpful assistant.")
 
     while True:
         user_input = input("You: ")
-        bandolier.add_user_message(user_input)
-        messages = bandolier.run()
-        for messages in messages:
+        conversation.add_user_message(user_input)
+
+        # the messages returned here are for UI purposes.  The conversation has already been
+        # updated with new messages.
+        messages = bandolier.run(conversation)
+        for message in messages:
+            # this message indicates function output, and you probably don't need to do anything with it.
             if message.role == "function":
                 continue
-            # message can have either or both of content and function_call
+
+            # messages from the server can have content and/or function_call both
             if message.content:
                 print(f"{message.role}: {message.content}")
             if "function_call" in message:
                 print(f"{message.role}: {message.function_call.name}")
 
 
-        print(f"{message.role}: {message.content}")
-
-
 if __name__ == "__main__":
     main()
 ```
 
 If you want more control, there are two other ways to use the Library. You can specify
 a different model version:
 
@@ -102,25 +104,26 @@
 bandolier = Bandolier(model="gpt-4")
 ```
 Or you can specify your own completion function.
 
 
 ```python
 def completion(model, messages, functions=None):
-    response = openai.ChatCompletion.create(
-        model=model,
-        messages=messages,
-        functions=functions,
-        temperature=0.0,
-    )
+    request = {
+        "model": model,
+        "messages": messages,
+        "temperature": 0.0,
+    }
+    if functions:
+        request["functions"] = functions
 
+    response = openai.ChatCompletion.create(**request)
     return response["choices"][0]
 
-# the model should be specified to bandolier as well so it can do
-# the correct token accounting when maintaining history.
+
 bandolier = Bandolier(completion_fn=completion)
 
 ```
 
 Or you can handle all the communication yourself, and only use Bandolier
 as a way to annotate your functions.
```

### Comparing `bandolier-0.1.2/README.md` & `bandolier-0.1.3/bandolier.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,47 @@
+Metadata-Version: 2.1
+Name: bandolier
+Version: 0.1.3
+Summary: A helper for OpenAI functions
+Home-page: https://github.com/johnnysands/bandolier
+Author: Johnny Sands
+Author-email: johnnysands@users.noreply.github.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Bandolier
 
 Bandolier is a library to make it easier to deal with OpenAI ChatGPT functions.
 
-To expose functions to OpenAI GPT services, we need to tell OpenAI about the
-functions.  Ideally we could simply inspect the functions and use that information
-to communicate to OpenAI, but unfortunately all the information we need isn't
-available.
-
-Type annotations could get us part of the way there, but they don't solve the
-whole problem, and they can't represent some of more complex data structures
-it's possible to use with ChatGPT.
-
-Bandolier uses decorators to add annotations to functions with the missing
-information.  These annotations are also validated against the information
-that we can get via introspection, helping your code and configuration
-stay in sync.
+There are two key classes:
+
+Bandolier tracks the information on your functions and helps you build the
+prompts you need to expose the functions to the chat interface.
 
-Bandolier also provides some convenience functions for working with OpenAI's APIs.
-It helps you manage message history and process requests for function calls automatically.
+Conversation stores your message history.  Bandolier uses the Conversation to
+build prompts with appropriate history. You can use a different Conversation
+in each call to Bandolier to make it easier to manage multiple conversation
+streams.
 
 ## Example
 
 ```python
-from bandolier import Bandolier, annotate_arguments, annotate_description
+from bandolier import Bandolier, Conversation, annotate_arguments, annotate_description
 
 
+# First set up your functions
 @annotate_arguments(
     {
         "location": {
             "type": "string",
             "description": "The city and state, e.g. San Francisco, CA.",
         },
         "unit": {
@@ -36,46 +49,54 @@
             "description": "The unit to return the temperature in, e.g. F or C.",
             "default": "F",
         },
     }
 )
 @annotate_description("Get the weather for a location.")
 def get_weather(location, unit="F"):
+    # api call here...
     return {"temperature": 72, unit: unit, "conditions": ["sunny", "windy"]}
 
 
 # can also use docstring for description
 def get_location():
     """Get the user's location."""
+    # api call here...
     return "San Francisco, CA"
 
 
 def main():
+    # Set up the bandolier function configuration
     bandolier = Bandolier()
     bandolier.add_function(get_weather)
     bandolier.add_function(get_location)
-    bandolier.add_system_message("You are a helpful assistant.")
+
+    # create a new conversational conversation
+    conversation = Conversation()
+    conversation.add_system_message("You are a helpful assistant.")
 
     while True:
         user_input = input("You: ")
-        bandolier.add_user_message(user_input)
-        messages = bandolier.run()
-        for messages in messages:
+        conversation.add_user_message(user_input)
+
+        # the messages returned here are for UI purposes.  The conversation has already been
+        # updated with new messages.
+        messages = bandolier.run(conversation)
+        for message in messages:
+            # this message indicates function output, and you probably don't need to do anything with it.
             if message.role == "function":
                 continue
-            # message can have either or both of content and function_call
+
+            # messages from the server can have content and/or function_call both
             if message.content:
                 print(f"{message.role}: {message.content}")
             if "function_call" in message:
                 print(f"{message.role}: {message.function_call.name}")
 
 
-        print(f"{message.role}: {message.content}")
-
-
 if __name__ == "__main__":
     main()
 ```
 
 If you want more control, there are two other ways to use the Library. You can specify
 a different model version:
 
@@ -83,25 +104,26 @@
 bandolier = Bandolier(model="gpt-4")
 ```
 Or you can specify your own completion function.
 
 
 ```python
 def completion(model, messages, functions=None):
-    response = openai.ChatCompletion.create(
-        model=model,
-        messages=messages,
-        functions=functions,
-        temperature=0.0,
-    )
+    request = {
+        "model": model,
+        "messages": messages,
+        "temperature": 0.0,
+    }
+    if functions:
+        request["functions"] = functions
 
+    response = openai.ChatCompletion.create(**request)
     return response["choices"][0]
 
-# the model should be specified to bandolier as well so it can do
-# the correct token accounting when maintaining history.
+
 bandolier = Bandolier(completion_fn=completion)
 
 ```
 
 Or you can handle all the communication yourself, and only use Bandolier
 as a way to annotate your functions.
 
@@ -116,8 +138,8 @@
 functions = Bandolier.get_function_metadata()
 
 result = openai.ChatCompletion.create({
     "messages": ...
     "functions": functions,
     ...
 })
-```
+```
```

### Comparing `bandolier-0.1.2/bandolier/bandolier.py` & `bandolier-0.1.3/bandolier/bandolier.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,52 +3,33 @@
 from box import Box
 import inspect
 import openai
 import json
 import tiktoken
 
 
-# openai helper
 def completion(model, messages, functions=None):
     request = {
         "model": model,
         "messages": messages,
         "temperature": 0.0,
     }
     if functions:
         request["functions"] = functions
 
     response = openai.ChatCompletion.create(**request)
-
     return response["choices"][0]
 
 
-def annotate_description(description):
-    def decorator(function):
-        function.__doc__ = description
-        return function
-
-    return decorator
-
-
-def annotate_arguments(properties):
-    def decorator(function):
-        function.__properties__ = properties
-        return function
-
-    return decorator
-
-
 class Bandolier:
     def __init__(
         self, completion_fn=completion, model="gpt-3.5-turbo", max_tokens=3000
     ):
         self.functions = {}
         self.function_metadata = []
-        self.messages = []
         self.completion_fn = completion_fn
         self.model = model
         self.max_tokens = max_tokens
         self.encoding = tiktoken.encoding_for_model(model)
 
     def add_function(self, function):
         name = function.__name__
@@ -75,70 +56,50 @@
             "description": description,
             "parameters": {"type": "object", "properties": properties},
             "required": required,
         }
         self.functions[name] = function
         self.function_metadata.append(metadata)
 
-    def add_message(self, message):
-        self.messages.append(Box(message))
-        self._trim_messages()
-
-    def add_system_message(self, content):
-        "convience method for adding a system message"
-        self.add_message({"role": "system", "content": content})
-
-    def add_user_message(self, content):
-        "convience method for adding a user message"
-        self.add_message({"role": "user", "content": content})
-
     def call(self, function_name, arguments):
         arguments = json.loads(arguments)
         function = self.functions[function_name]
         return Box(
             {
                 "role": "function",
                 "name": function_name,
                 "content": json.dumps(function(**arguments)),
             }
         )
 
-    def get_function_metadata(self):
-        return self.function_metadata
+    def run(self, conversation):
+        """Run the chatbot using the supplied conversation.
+        returns a list of all new messages."""
 
-    def run(self):
         response = self.completion_fn(
-            self.model, self.messages, self.get_function_metadata()
+            self.model, conversation.messages, self.function_metadata
         )
-        message = response.message
-        self.add_message(message)
+        conversation.add_message(response.message)
 
-        # TODO FIXME this code makes the assumption that function call will not have message content,
-        # but that's not actually true.  It's possible to return a mesage with both content and a function call.
-        # This needs to be refactored so that run can return multiple messages.
-        messages = [message]
+        # maintain conversation at a usable size.
+        conversation.trim_messages(self.encoding, self.max_tokens)
+
+        messages = [response.message]
         while response.finish_reason == "function_call":
-            message = self.call(
-                message.function_call.name, message.function_call.arguments
+            # call function and store message
+            fn_message = self.call(
+                response.message.function_call.name,
+                response.message.function_call.arguments,
             )
-            self.add_message(message)
-            messages.append(message)
+            conversation.add_message(fn_message)
+            messages.append(fn_message)
 
+            # return response from function
             response = self.completion_fn(
-                self.model, self.messages, self.get_function_metadata()
+                self.model, conversation.messages, self.function_metadata
             )
-            message = response.message
-            self.add_message(message)
-            messages.append(message)
+            conversation.add_message(response.message)
+            messages.append(response.message)
 
         if response.finish_reason != "stop":
             raise Exception(f"Unexpected finish reason: {response.finish_reason}")
         return messages
-
-    def _trim_messages(self):
-        # I'm not sure how accurate this is, but I encode each message to json and then count
-        # the tokens in the result.
-
-        token_count = sum(len(self.encoding.encode(m.to_json())) for m in self.messages)
-        while token_count > self.max_tokens:
-            removed_message = self.messages.pop(0)
-            token_count -= len(self.encoding.encode(removed_message.to_json()))
```

### Comparing `bandolier-0.1.2/setup.py` & `bandolier-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
     readme = readme.split("\n")
     readme = [line for line in readme if "<img" not in line]
     readme = "\n".join(readme)
 
 setup(
     name="bandolier",
-    version="0.1.2",
+    version="0.1.3",
     description="A helper for OpenAI functions",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/johnnysands/bandolier",
     author="Johnny Sands",
     author_email="johnnysands@users.noreply.github.com",
     license="MIT",
```


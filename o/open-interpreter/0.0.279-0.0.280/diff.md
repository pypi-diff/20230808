# Comparing `tmp/open_interpreter-0.0.279.tar.gz` & `tmp/open_interpreter-0.0.280.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.279.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.280.tar", max compression
```

## Comparing `open_interpreter-0.0.279.tar` & `open_interpreter-0.0.280.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.279/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.279/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.279/interpreter/__init__.py
--rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.279/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.279/interpreter/code_block.py
--rw-r--r--   0        0        0     8410 2023-08-07 19:48:01.908489 open_interpreter-0.0.279/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13860 2023-08-07 17:21:10.873094 open_interpreter-0.0.279/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.279/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.279/interpreter/message_block.py
--rw-r--r--   0        0        0     1915 2023-08-07 17:40:06.855841 open_interpreter-0.0.279/interpreter/system_message.txt
--rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.279/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-07 21:30:02.343054 open_interpreter-0.0.279/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.279/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.280/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.280/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.280/interpreter/__init__.py
+-rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.280/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.280/interpreter/code_block.py
+-rw-r--r--   0        0        0     8410 2023-08-07 19:48:01.908489 open_interpreter-0.0.280/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13873 2023-08-07 21:38:42.723843 open_interpreter-0.0.280/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.280/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.280/interpreter/message_block.py
+-rw-r--r--   0        0        0     1915 2023-08-07 17:40:06.855841 open_interpreter-0.0.280/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.280/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-07 21:39:53.999482 open_interpreter-0.0.280/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.280/PKG-INFO
```

### Comparing `open_interpreter-0.0.279/LICENSE` & `open_interpreter-0.0.280/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/README.md` & `open_interpreter-0.0.280/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/__init__.py` & `open_interpreter-0.0.280/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/cli.py` & `open_interpreter-0.0.280/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/code_block.py` & `open_interpreter-0.0.280/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/code_interpreter.py` & `open_interpreter-0.0.280/interpreter/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/interpreter.py` & `open_interpreter-0.0.280/interpreter/interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
   def __init__(self):
     self.messages = []
     self.temperature = 0.01
     self.api_key = None
     self.auto_run = False
     self.local = False
+    self.model = "gpt-4-0613"
 
     # Get default system message
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, 'system_message.txt'), 'r') as f:
       self.system_message = f.read().strip()
 
     # Store Code Interpreter instances for each language
@@ -215,18 +216,17 @@
     # overwrite the system message with a tiny, performant one.
     if self.local:
       system_message = "You are an AI that executes Python code. Use ```python to run it."
 
     # Make LLM call
     if not self.local:
       # GPT-4
-      model = "gpt-4-0613"
       response = openai.ChatCompletion.create(
-        model=model,
-        messages=tt.trim(self.messages, model, system_message=system_message),
+        model=self.model,
+        messages=tt.trim(self.messages, self.model, system_message=system_message),
         functions=[function_schema],
         stream=True,
         temperature=self.temperature,
       )
     elif self.local:
       # Llama-2
```

### Comparing `open_interpreter-0.0.279/interpreter/llama_2.py` & `open_interpreter-0.0.280/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/message_block.py` & `open_interpreter-0.0.280/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/system_message.txt` & `open_interpreter-0.0.280/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/interpreter/utils.py` & `open_interpreter-0.0.280/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.279/pyproject.toml` & `open_interpreter-0.0.280/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.279"
+version = "0.0.280"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.279/PKG-INFO` & `open_interpreter-0.0.280/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.279
+Version: 0.0.280
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


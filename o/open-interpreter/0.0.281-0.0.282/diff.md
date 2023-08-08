# Comparing `tmp/open_interpreter-0.0.281.tar.gz` & `tmp/open_interpreter-0.0.282.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.281.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.282.tar", max compression
```

## Comparing `open_interpreter-0.0.281.tar` & `open_interpreter-0.0.282.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.281/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.281/README.md
--rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.281/interpreter/__init__.py
--rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.281/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.281/interpreter/code_block.py
--rw-r--r--   0        0        0     8505 2023-08-08 19:19:12.155668 open_interpreter-0.0.281/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13873 2023-08-07 21:38:42.723843 open_interpreter-0.0.281/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.281/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.281/interpreter/message_block.py
--rw-r--r--   0        0        0     2274 2023-08-08 19:48:17.198630 open_interpreter-0.0.281/interpreter/system_message.txt
--rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.281/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-08 19:48:30.159840 open_interpreter-0.0.281/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.281/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.282/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.282/README.md
+-rw-r--r--   0        0        0      865 2023-08-06 05:27:12.168319 open_interpreter-0.0.282/interpreter/__init__.py
+-rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.282/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.282/interpreter/code_block.py
+-rw-r--r--   0        0        0     8511 2023-08-08 19:50:06.232812 open_interpreter-0.0.282/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13873 2023-08-07 21:38:42.723843 open_interpreter-0.0.282/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.282/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.282/interpreter/message_block.py
+-rw-r--r--   0        0        0     2274 2023-08-08 19:48:17.198630 open_interpreter-0.0.282/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.282/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-08 19:50:58.521695 open_interpreter-0.0.282/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.282/PKG-INFO
```

### Comparing `open_interpreter-0.0.281/LICENSE` & `open_interpreter-0.0.282/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/README.md` & `open_interpreter-0.0.282/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/__init__.py` & `open_interpreter-0.0.282/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/cli.py` & `open_interpreter-0.0.282/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/code_block.py` & `open_interpreter-0.0.282/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/code_interpreter.py` & `open_interpreter-0.0.282/interpreter/code_interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,20 +124,20 @@
         return self.output
         
       code = fix_code_indentation(code)
 
     # Add end command (we'll be listening for this so we know when it ends)
     code += "\n\n" + self.print_cmd.format('END_OF_EXECUTION') + "\n"
 
-    
+    """
     # Debug
     print("Running code:")
     print(code)
     print("---")
-    
+    """
 
     # Reset self.done so we can .wait() for it
     self.done = threading.Event()
     self.done.clear()
 
     # Write code to stdin of the process
     try:
```

### Comparing `open_interpreter-0.0.281/interpreter/interpreter.py` & `open_interpreter-0.0.282/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/llama_2.py` & `open_interpreter-0.0.282/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/message_block.py` & `open_interpreter-0.0.282/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/system_message.txt` & `open_interpreter-0.0.282/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/interpreter/utils.py` & `open_interpreter-0.0.282/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.281/pyproject.toml` & `open_interpreter-0.0.282/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.281"
+version = "0.0.282"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.281/PKG-INFO` & `open_interpreter-0.0.282/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.281
+Version: 0.0.282
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


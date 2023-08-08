# Comparing `tmp/open_interpreter-0.0.284.tar.gz` & `tmp/open_interpreter-0.0.285.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.284.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.285.tar", max compression
```

## Comparing `open_interpreter-0.0.284.tar` & `open_interpreter-0.0.285.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.284/LICENSE
--rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.284/README.md
--rw-r--r--   0        0        0      865 2023-08-08 20:49:23.574971 open_interpreter-0.0.284/interpreter/__init__.py
--rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.284/interpreter/cli.py
--rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.284/interpreter/code_block.py
--rw-r--r--   0        0        0     9095 2023-08-08 21:22:57.659640 open_interpreter-0.0.284/interpreter/code_interpreter.py
--rw-r--r--   0        0        0    13886 2023-08-08 21:21:48.596622 open_interpreter-0.0.284/interpreter/interpreter.py
--rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.284/interpreter/llama_2.py
--rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.284/interpreter/message_block.py
--rw-r--r--   0        0        0     2225 2023-08-08 19:57:21.789487 open_interpreter-0.0.284/interpreter/system_message.txt
--rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.284/interpreter/utils.py
--rw-r--r--   0        0        0      600 2023-08-08 21:23:04.944381 open_interpreter-0.0.284/pyproject.toml
--rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.284/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.285/LICENSE
+-rw-r--r--   0        0        0     6394 2023-08-06 09:01:16.892405 open_interpreter-0.0.285/README.md
+-rw-r--r--   0        0        0      865 2023-08-08 20:49:23.574971 open_interpreter-0.0.285/interpreter/__init__.py
+-rw-r--r--   0        0        0      965 2023-08-07 21:29:49.358089 open_interpreter-0.0.285/interpreter/cli.py
+-rw-r--r--   0        0        0     2641 2023-08-06 21:24:11.035549 open_interpreter-0.0.285/interpreter/code_block.py
+-rw-r--r--   0        0        0     9127 2023-08-08 21:24:48.635373 open_interpreter-0.0.285/interpreter/code_interpreter.py
+-rw-r--r--   0        0        0    13886 2023-08-08 21:21:48.596622 open_interpreter-0.0.285/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2508 2023-08-06 21:27:53.527041 open_interpreter-0.0.285/interpreter/llama_2.py
+-rw-r--r--   0        0        0     1529 2023-08-06 21:23:17.045848 open_interpreter-0.0.285/interpreter/message_block.py
+-rw-r--r--   0        0        0     2225 2023-08-08 19:57:21.789487 open_interpreter-0.0.285/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3535 2023-08-06 21:56:51.302530 open_interpreter-0.0.285/interpreter/utils.py
+-rw-r--r--   0        0        0      600 2023-08-08 21:23:54.182289 open_interpreter-0.0.285/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 open_interpreter-0.0.285/PKG-INFO
```

### Comparing `open_interpreter-0.0.284/LICENSE` & `open_interpreter-0.0.285/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/README.md` & `open_interpreter-0.0.285/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/__init__.py` & `open_interpreter-0.0.285/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/cli.py` & `open_interpreter-0.0.285/interpreter/cli.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/code_block.py` & `open_interpreter-0.0.285/interpreter/code_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/code_interpreter.py` & `open_interpreter-0.0.285/interpreter/code_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     # Use the print_cmd for the selected language
     self.print_cmd = language_map[self.language]["print_cmd"]
     code = self.code
 
     # Add print commands that tell us what the active line is
     # Disabled
-    # code = self.add_active_line_prints(code)
+    code = self.add_active_line_prints(code)
 
     # If it's Python, we also need to normalize
     # and fix indentation (so it works with `python -i`)
     if self.language == "python":
 
       # Normalize code by parsing then unparsing it
       try:
@@ -203,15 +203,15 @@
         return code
       for line in code_lines:
         if line.startswith(" "):
           return code
 
     # If it's Python, check for breaking cases
     if self.language == "python":
-      if "try" in code or "except" in code or "'''" in code or "'''" in code:
+      if "try" in code or "except" in code or "'''" in code or "'''" in code or "[\n" in code or "{\n" in code:
         return code
 
     # Initialize an empty list to hold the modified lines of code
     modified_code_lines = []
 
     # Iterate over each line in the original code
     for i, line in enumerate(code_lines):
```

### Comparing `open_interpreter-0.0.284/interpreter/interpreter.py` & `open_interpreter-0.0.285/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/llama_2.py` & `open_interpreter-0.0.285/interpreter/llama_2.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/message_block.py` & `open_interpreter-0.0.285/interpreter/message_block.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/system_message.txt` & `open_interpreter-0.0.285/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/interpreter/utils.py` & `open_interpreter-0.0.285/interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.284/pyproject.toml` & `open_interpreter-0.0.285/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"},
 ]
-version = "0.0.284"
+version = "0.0.285"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.284/PKG-INFO` & `open_interpreter-0.0.285/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.284
+Version: 0.0.285
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


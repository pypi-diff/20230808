# Comparing `tmp/fhirpathpy-0.2.1.tar.gz` & `tmp/fhirpathpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirpathpy-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fhirpathpy-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fhirpathpy-0.2.1.tar` & `fhirpathpy-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2453 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/README.md
--rw-r--r--   0        0        0     2967 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/__init__.py
--rw-r--r--   0        0        0     4626 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/__init__.py
--rw-r--r--   0        0        0     9524 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/evaluators/__init__.py
--rw-r--r--   0        0        0     5817 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/__init__.py
--rw-r--r--   0        0        0      799 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/collections.py
--rw-r--r--   0        0        0      282 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/combining.py
--rw-r--r--   0        0        0      587 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/constants.py
--rw-r--r--   0        0        0      932 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/datetime.py
--rw-r--r--   0        0        0     4738 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/equality.py
--rw-r--r--   0        0        0     2055 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/existence.py
--rw-r--r--   0        0        0     2549 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/filtering.py
--rw-r--r--   0        0        0     1223 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/logic.py
--rw-r--r--   0        0        0     3698 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/math.py
--rw-r--r--   0        0        0     2347 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/misc.py
--rw-r--r--   0        0        0     1450 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/navigation.py
--rw-r--r--   0        0        0     1526 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/strings.py
--rw-r--r--   0        0        0       94 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/invocations/subsetting.py
--rw-r--r--   0        0        0    11005 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/nodes.py
--rw-r--r--   0        0        0     1568 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/engine/util.py
--rw-r--r--   0        0        0     1280 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/ASTPathListener.py
--rw-r--r--   0        0        0     5507 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/FHIRPath.g4
--rw-r--r--   0        0        0      988 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/__init__.py
--rw-r--r--   0        0        0     5699 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.interp
--rw-r--r--   0        0        0     1029 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.tokens
--rw-r--r--   0        0        0    17301 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.interp
--rw-r--r--   0        0        0    20549 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.py
--rw-r--r--   0        0        0     1029 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.tokens
--rw-r--r--   0        0        0    12767 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathListener.py
--rw-r--r--   0        0        0    79435 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathParser.py
--rw-r--r--   0        0        0        0 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/fhirpathpy/parser/generated/__init__.py
--rw-r--r--   0        0        0     1786 2023-07-05 16:33:40.930712 fhirpathpy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 fhirpathpy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-07 22:52:18.799278 fhirpathpy-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     2453 2023-08-07 22:52:18.799278 fhirpathpy-0.2.2/README.md
+-rw-r--r--   0        0        0     2967 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/__init__.py
+-rw-r--r--   0        0        0     4735 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/__init__.py
+-rw-r--r--   0        0        0     9518 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/evaluators/__init__.py
+-rw-r--r--   0        0        0     5817 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/__init__.py
+-rw-r--r--   0        0        0      799 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/collections.py
+-rw-r--r--   0        0        0      282 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/combining.py
+-rw-r--r--   0        0        0      587 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/constants.py
+-rw-r--r--   0        0        0      932 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/datetime.py
+-rw-r--r--   0        0        0     4738 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/equality.py
+-rw-r--r--   0        0        0     2055 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/existence.py
+-rw-r--r--   0        0        0     2549 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/filtering.py
+-rw-r--r--   0        0        0     1223 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/logic.py
+-rw-r--r--   0        0        0     3698 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/math.py
+-rw-r--r--   0        0        0     2347 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/misc.py
+-rw-r--r--   0        0        0     1450 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/navigation.py
+-rw-r--r--   0        0        0     1526 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/strings.py
+-rw-r--r--   0        0        0       94 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/invocations/subsetting.py
+-rw-r--r--   0        0        0    11005 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/nodes.py
+-rw-r--r--   0        0        0     1568 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/engine/util.py
+-rw-r--r--   0        0        0     1280 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/ASTPathListener.py
+-rw-r--r--   0        0        0     5507 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/FHIRPath.g4
+-rw-r--r--   0        0        0      988 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/__init__.py
+-rw-r--r--   0        0        0     5699 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPath.interp
+-rw-r--r--   0        0        0     1029 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPath.tokens
+-rw-r--r--   0        0        0    17301 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.interp
+-rw-r--r--   0        0        0    20549 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.py
+-rw-r--r--   0        0        0     1029 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.tokens
+-rw-r--r--   0        0        0    12767 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathListener.py
+-rw-r--r--   0        0        0    79435 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathParser.py
+-rw-r--r--   0        0        0        0 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/fhirpathpy/parser/generated/__init__.py
+-rw-r--r--   0        0        0     1786 2023-08-07 22:52:18.803278 fhirpathpy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 fhirpathpy-0.2.2/PKG-INFO
```

### Comparing `fhirpathpy-0.2.1/LICENSE.md` & `fhirpathpy-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/README.md` & `fhirpathpy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/__init__.py` & `fhirpathpy-0.2.2/fhirpathpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from fhirpathpy.engine.invocations.constants import constants
 from fhirpathpy.parser import parse
 from fhirpathpy.engine import do_eval
 from fhirpathpy.engine.util import arraify, get_data, set_paths
 from fhirpathpy.engine.nodes import FP_Type
 
 __title__ = "fhirpathpy"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "beda.software"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 beda.software"
 
 # Version synonym
 VERSION = __version__
```

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/__init__.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -94,32 +94,34 @@
     "Number": check_number_param,
     "Boolean": check_boolean_param,
     "String": check_string_param,
 }
 
 
 def make_param(ctx, parentData, node_type, param):
-    ctx["currentData"] = parentData
 
     if node_type == "Expr":
 
         def func(data):
-            return do_eval(ctx, util.arraify(data), param)
+            ctx["$this"] = util.arraify(data)
+            return do_eval(ctx, ctx["$this"], param)
 
         return func
 
     if node_type == "AnyAtRoot":
+        ctx["$this"] = ctx["$this"] if "$this" in ctx else ctx['dataRoot']
         return do_eval(ctx, ctx["dataRoot"], param)
 
     if node_type == "Identifier":
         if param["type"] == "TermExpression":
             return param["text"]
 
         raise Exception("Expected identifier node, got " + json.dumps(param))
 
+    ctx["$this"] = parentData
     res = do_eval(ctx, parentData, param)
 
     if node_type == "Any":
         return res
 
     if isinstance(node_type, list):
         if len(res) == 0:
```

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/evaluators/__init__.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/evaluators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 def union_expression(ctx, parentData, node):
     return engine.infix_invoke(ctx, "|", parentData, node["children"])
 
 
 def this_invocation(ctx, parentData, node):
-    return util.arraify(ctx["currentData"])
+    return util.arraify(ctx["$this"])
 
 
 def op_expression(ctx, parentData, node):
     op = node["terminalNodeText"][0]
     return engine.infix_invoke(ctx, op, parentData, node["children"])
```

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/__init__.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/collections.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/collections.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/constants.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/constants.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/datetime.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/datetime.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/equality.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/equality.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/existence.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/existence.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/filtering.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/filtering.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/logic.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/logic.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/math.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/math.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/misc.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/misc.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/navigation.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/navigation.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/invocations/strings.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/invocations/strings.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/nodes.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/nodes.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/engine/util.py` & `fhirpathpy-0.2.2/fhirpathpy/engine/util.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/ASTPathListener.py` & `fhirpathpy-0.2.2/fhirpathpy/parser/ASTPathListener.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/FHIRPath.g4` & `fhirpathpy-0.2.2/fhirpathpy/parser/FHIRPath.g4`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/__init__.py` & `fhirpathpy-0.2.2/fhirpathpy/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.interp` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPath.interp`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPath.tokens` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPath.tokens`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.interp` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.interp`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.py` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathLexer.tokens` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathLexer.tokens`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathListener.py` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathListener.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/fhirpathpy/parser/generated/FHIRPathParser.py` & `fhirpathpy-0.2.2/fhirpathpy/parser/generated/FHIRPathParser.py`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/pyproject.toml` & `fhirpathpy-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fhirpathpy-0.2.1/PKG-INFO` & `fhirpathpy-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhirpathpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: FHIRPath implementation in Python
 Keywords: fhir,fhirpath
 Author-email: "beda.software" <fhirpath@beda.software>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```


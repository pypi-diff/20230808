# Comparing `tmp/jsonschema_markdown-0.1.0-py3-none-any.whl.zip` & `tmp/jsonschema_markdown-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5218 bytes, number of entries: 13
+Zip file size: 5611 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 jsonschema_markdown/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/__init__.py
--rw-r--r--  2.0 unx     5027 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
+-rw-r--r--  2.0 unx     6988 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
 -rw-r--r--  2.0 unx      587 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/parser.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/enums.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      646 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1171 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.0.dist-info/RECORD
-13 files, 8741 bytes uncompressed, 3194 bytes compressed:  63.5%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      646 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1171 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.1.dist-info/RECORD
+13 files, 10702 bytes uncompressed, 3587 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: jsonschema_markdown/utils/__init__.py
 Comment: 
 
 Filename: jsonschema_markdown/utils/enums.py
 Comment: 
 
-Filename: jsonschema_markdown-0.1.0.dist-info/LICENSE
+Filename: jsonschema_markdown-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: jsonschema_markdown-0.1.0.dist-info/METADATA
+Filename: jsonschema_markdown-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: jsonschema_markdown-0.1.0.dist-info/WHEEL
+Filename: jsonschema_markdown-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: jsonschema_markdown-0.1.0.dist-info/entry_points.txt
+Filename: jsonschema_markdown-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: jsonschema_markdown-0.1.0.dist-info/RECORD
+Filename: jsonschema_markdown-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonschema_markdown/converter/markdown.py

```diff
@@ -1,9 +1,11 @@
 import json
 
+from loguru import logger
+
 
 def generate(schema: dict) -> str:
     markdown = ""
 
     # Add the title and description of the schema
     markdown += (
         f"# {schema['title']}\n\n" if "title" in schema else "jsonschema-markdown\n\n"
@@ -13,17 +15,17 @@
         if "description" in schema
         else "JSON Schema missing a description, provide it using the `description` key in the root of the JSON document.\n\n"
     )
     markdown += _create_table_of_properties(schema)
 
     markdown += "\n\n---\n\n# Definitions\n\n"
 
-    for definition in schema.get("definitions", {}).values():
+    for definition in schema.get("definitions", schema.get("$defs", {})).values():
         markdown += f"\n\n## {definition.get('title', 'No Title')}\n\n"
-        markdown += f"{definition.get('description', '')}\n\n"
+        markdown += f"{definition.get('description', '').strip()}\n\n"
         markdown += _create_table_of_properties(definition)
 
     return markdown
 
 
 def _sort_properties(schema: dict) -> dict:
     """
@@ -48,14 +50,117 @@
             or item[1].get("deprecated", False),
         )
     )
 
     return properties
 
 
+def _remove_nulls(property_type: str, property_details: dict) -> tuple:
+    """
+    Get the possible values for a property.
+    """
+
+    if "oneOf" in property_details:
+        try:
+            property_details["oneOf"].remove({"type": "null"})
+        except Exception:
+            logger.warning("No null type in oneOf")
+
+        if len(property_details["oneOf"]) == 1:
+            return _remove_nulls("object", property_details["oneOf"][0])
+
+    if "anyOf" in property_details:
+        try:
+            property_details["anyOf"].remove({"type": "null"})
+        except Exception:
+            logger.warning("No null type in anyOf")
+
+        if len(property_details["anyOf"]) == 1:
+            return _remove_nulls("object", property_details["anyOf"][0])
+
+    if "allOf" in property_details:
+        try:
+            property_details["allOf"].remove({"type": "null"})
+        except Exception:
+            logger.warning("No null type in allOf")
+
+        if len(property_details["allOf"]) == 1:
+            return _remove_nulls("object", property_details["allOf"][0])
+
+    is_const = "const" in property_details
+    res_type = "const" if is_const else property_type
+
+    if "enum" in property_details:
+        res_details = ", ".join(
+            [f"`{str(value)}`" for value in property_details["enum"]]
+        )
+    elif "oneOf" in property_details:
+        res_details = ", ".join(
+            [
+                f"`{value.get('const') if 'const' in value else str(value)}`"
+                for value in property_details["oneOf"]
+            ]
+        )
+        if any("const" in value for value in property_details["oneOf"]):
+            res_type = "const"
+
+    elif "anyOf" in property_details:
+        res_details = " or ".join(
+            [
+                f"`{value.get('const') if 'const' in value else str(value)}`"
+                for value in property_details["anyOf"]
+            ]
+        )
+        if any("const" in value for value in property_details["anyOf"]):
+            res_type = "const"
+    elif "allOf" in property_details:
+        res_details = " and ".join(
+            [
+                f"`{value.get('const') if 'const' in value else str(value)}`"
+                for value in property_details["allOf"]
+            ]
+        )
+        if any("const" in value for value in property_details["allOf"]):
+            res_type = "const"
+    elif "items" in property_details:
+        title = property_details["items"].get("title")
+        _type = property_details["items"].get("type")
+        if title:
+            res_details = f"[{title}](#{title})"
+        elif _type:
+            res_details = f"`{_type}`"
+        else:
+            res_details = "yo124"
+    elif "pattern" in property_details:
+        pattern = property_details.get("pattern")
+        res_details = pattern
+    elif "additionalProperties" in property_details:
+        title = property_details["additionalProperties"].get("title")
+        _type = property_details["additionalProperties"].get("type")
+        if title:
+            res_details = f"[{title}](#{title})"
+        elif _type:
+            res_details = f"`{_type}`"
+        else:
+            res_details = "?"
+    elif is_const:
+        res_details = property_details.get("const")
+    else:
+        title = property_details.get("title")
+        res_type = res_type if res_type else property_details.get("type", "??")
+        if title and res_type != "string" and res_type != "boolean" and not is_const:
+            res_details = f"[{title}](#{title.replace(' ', '-')})"
+        elif res_type:
+            res_details = f"`{res_type}`"
+        else:
+            res_details = "???"
+
+    return res_type, res_details
+
+
 def _create_table_of_properties(schema: dict) -> str:
     """
     Create a table of the properties in the schema.
     Outputs a markdown table with the following columns:
     - Property name
     - Type
     - Required
@@ -74,65 +179,23 @@
     if not schema.get("additionalProperties", True):
         markdown += "> ⚠️ Additional properties are not allowed.\n\n"
 
     markdown += "| Property | Type | Required | Possible Values | Deprecated | Default | Description |\n"
     markdown += "| -------- | ---- | -------- | --------------- | ---------- | ------- | ----------- |\n"
 
     for property_name, property_details in schema["properties"].items():
-        property_type = property_details.get("type", "?")
+        property_type = property_details.get("type", property_details.get("const"))
 
-        if "enum" in property_details:
-            possible_values = ", ".join(
-                [f"`{str(value)}`" for value in property_details["enum"]]
-            )
-        elif "oneOf" in property_details:
-            possible_values = ", ".join(
-                [f"`{str(value)}`" for value in property_details["oneOf"]]
-            )
-            property_type = "array (`oneOf`)"
-        elif "anyOf" in property_details:
-            possible_values = " or ".join(
-                [f"`{str(value)}`" for value in property_details["anyOf"]]
-            )
-            property_type = "array (`anyOf`)"
-        elif "allOf" in property_details:
-            possible_values = " and ".join(
-                [
-                    f"[{value.get('title')}]({value.get('title')})"
-                    for value in property_details["allOf"]
-                ]
-            )
-            property_type = "array (`allOf`)"
-        elif "items" in property_details:
-            title = property_details["items"].get("title")
-            _type = property_details["items"].get("type")
-            if title:
-                possible_values = f"[{title}](#{title})"
-            elif _type:
-                possible_values = f"`{_type}`"
-            else:
-                possible_values = "??"
-        elif "pattern" in property_details:
-            pattern = property_details.get("pattern")
-            possible_values = pattern
-        elif "additionalProperties" in property_details:
-            title = property_details["additionalProperties"].get("title")
-            _type = property_details["additionalProperties"].get("type")
-            if title:
-                possible_values = f"[{title}](#{title})"
-            elif _type:
-                possible_values = f"`{_type}`"
-            else:
-                possible_values = "???"
-        else:
-            possible_values = f"`{property_type}`"
+        property_type, possible_values = _remove_nulls(property_type, property_details)
+
+        default = property_details.get("default")
 
         markdown += (
             f"| {property_name} | {property_type.capitalize()} | "
             f"{'✅' if property_name in schema.get('required', []) else ''} | "
             f"{possible_values}| "
             f"{'⛔️' if '[deprecated]' in str(property_details.get('description','')).lower() or property_details.get('deprecated') else ''} | "
-            f"{json.dumps(property_details.get('default')) if 'default' in property_details else ''} | "
+            f"{'`'+json.dumps(default)+'`' if default else ''} | "
             f"{property_details.get('description','')} |\n"
         )
 
     return markdown
```

## Comparing `jsonschema_markdown-0.1.0.dist-info/LICENSE` & `jsonschema_markdown-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jsonschema_markdown-0.1.0.dist-info/METADATA` & `jsonschema_markdown-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.1.0
+Version: 0.1.1
 Summary: Export a JSON Schema document to Markdown documentation.
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `jsonschema_markdown-0.1.0.dist-info/RECORD` & `jsonschema_markdown-0.1.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 jsonschema_markdown/__init__.py,sha256=6UdpCb2kIhAJZ3NiKvVW6E630TOBKjuml9zDpwUlZJw,81
 jsonschema_markdown/converter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jsonschema_markdown/converter/markdown.py,sha256=QY1CekVsmkp-EUMdTNN_PTtY0Aw3cA5Ak-9aXsS5Hyo,5027
+jsonschema_markdown/converter/markdown.py,sha256=bb0CEaE1HRqOdeCNrUIHmhvvwTbXShSwG0LP_rrlmqA,6988
 jsonschema_markdown/main.py,sha256=NzXBQJXuS8SAMUqMwUV5gNXkvdJ3hv4SLHzQJ44pCLY,587
 jsonschema_markdown/parser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/parser/parser.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/utils/enums.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jsonschema_markdown-0.1.0.dist-info/LICENSE,sha256=axN1TC4zNO_qVsrYheL5eB8fg6N4djrQEGgJY4NeMhU,1073
-jsonschema_markdown-0.1.0.dist-info/METADATA,sha256=qSmM7uvXVVb-8g6kPPAuhja-C_yaoNInprFHbXBsuLU,646
-jsonschema_markdown-0.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-jsonschema_markdown-0.1.0.dist-info/entry_points.txt,sha256=M6MzkSl1InYyJeflgFfh1Ewa-KluWxOWvDMWsSA7hrY,68
-jsonschema_markdown-0.1.0.dist-info/RECORD,,
+jsonschema_markdown-0.1.1.dist-info/LICENSE,sha256=axN1TC4zNO_qVsrYheL5eB8fg6N4djrQEGgJY4NeMhU,1073
+jsonschema_markdown-0.1.1.dist-info/METADATA,sha256=D-hpcOmW3mwtoNQspl3aJx5h3XOGpYgAwW7erMW2X-Y,646
+jsonschema_markdown-0.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+jsonschema_markdown-0.1.1.dist-info/entry_points.txt,sha256=M6MzkSl1InYyJeflgFfh1Ewa-KluWxOWvDMWsSA7hrY,68
+jsonschema_markdown-0.1.1.dist-info/RECORD,,
```


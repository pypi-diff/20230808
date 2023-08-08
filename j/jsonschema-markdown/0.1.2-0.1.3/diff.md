# Comparing `tmp/jsonschema_markdown-0.1.2-py3-none-any.whl.zip` & `tmp/jsonschema_markdown-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5622 bytes, number of entries: 13
+Zip file size: 6114 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 jsonschema_markdown/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/__init__.py
--rw-r--r--  2.0 unx     7041 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
--rw-r--r--  2.0 unx      587 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
+-rw-r--r--  2.0 unx    10399 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
+-rw-r--r--  2.0 unx      493 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/parser.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/enums.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      646 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1171 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.2.dist-info/RECORD
-13 files, 10755 bytes uncompressed, 3598 bytes compressed:  66.5%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      651 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1172 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.3.dist-info/RECORD
+13 files, 14025 bytes uncompressed, 4090 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: jsonschema_markdown/utils/__init__.py
 Comment: 
 
 Filename: jsonschema_markdown/utils/enums.py
 Comment: 
 
-Filename: jsonschema_markdown-0.1.2.dist-info/LICENSE
+Filename: jsonschema_markdown-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: jsonschema_markdown-0.1.2.dist-info/METADATA
+Filename: jsonschema_markdown-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: jsonschema_markdown-0.1.2.dist-info/WHEEL
+Filename: jsonschema_markdown-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: jsonschema_markdown-0.1.2.dist-info/entry_points.txt
+Filename: jsonschema_markdown-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: jsonschema_markdown-0.1.2.dist-info/RECORD
+Filename: jsonschema_markdown-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonschema_markdown/converter/markdown.py

```diff
@@ -1,32 +1,36 @@
 import json
+import urllib.parse
 
+import jsonref
 from loguru import logger
 
 
 def generate(schema: dict) -> str:
+    _schema: dict = jsonref.replace_refs(schema)  # type: ignore
     markdown = ""
 
     # Add the title and description of the schema
+    markdown += f"# {_schema.get('title', 'jsonschema-markdown')}\n\n"
+    description = _schema.get("description", "").strip(" \n")
     markdown += (
-        f"# {schema['title']}\n\n" if "title" in schema else "jsonschema-markdown\n\n"
-    )
-    markdown += (
-        f"{schema['description']}\n\n"
-        if "description" in schema
+        f"{description}\n\n"
+        if description
         else "JSON Schema missing a description, provide it using the `description` key in the root of the JSON document.\n\n"
     )
-    markdown += _create_table_of_properties(schema)
+    markdown += _create_definition_table(_schema)
 
     markdown += "\n\n---\n\n# Definitions\n\n"
 
-    for definition in schema.get("definitions", schema.get("$defs", {})).values():
+    for definition in _schema.get("definitions", _schema.get("$defs", {})).values():
+        description = definition.get("description", "").strip(" \n")
         markdown += f"\n\n## {definition.get('title', 'No Title')}\n\n"
-        markdown += f"{definition.get('description', '').strip()}\n\n"
-        markdown += _create_table_of_properties(definition)
+        markdown += f"{description}\n\n"
+        markdown += f"**Type:** `{definition.get('type', '?').strip()}`\n\n"
+        markdown += _create_definition_table(definition)
 
     return markdown
 
 
 def _sort_properties(schema: dict) -> dict:
     """
     Sort the properties in the schema by required, making the deprecated properties last.
@@ -50,45 +54,73 @@
             or item[1].get("deprecated", False),
         )
     )
 
     return properties
 
 
-def _remove_nulls(property_type: str, property_details: dict) -> tuple:
+def _create_enum_markdown(schema: dict) -> str:
+    """
+    Create a markdown table of the enum values.
+    """
+
+    markdown = "**Possible Values:** "
+    markdown += " or ".join([f"`{value}`" for value in schema["enum"]]) + "\n\n"
+
+    return markdown
+
+
+def _create_const_markdown(schema: dict) -> str:
+    """
+    Create a markdown table of the enum values.
+    """
+
+    return f"**Possible Values:** {schema.get('const', '?')}\n\n"
+
+
+def _get_property_details(property_type: str, property_details: dict) -> tuple:
     """
     Get the possible values for a property.
     """
 
     if "oneOf" in property_details:
         try:
             property_details["oneOf"].remove({"type": "null"})
         except Exception:
             logger.warning("No null type in oneOf")
 
         if len(property_details["oneOf"]) == 1:
-            return _remove_nulls("object", property_details["oneOf"][0])
+            return _get_property_details(
+                property_details["oneOf"][0].get("type", "?"),
+                property_details["oneOf"][0],
+            )
 
     if "anyOf" in property_details:
         try:
             property_details["anyOf"].remove({"type": "null"})
         except Exception:
             logger.warning("No null type in anyOf")
 
         if len(property_details["anyOf"]) == 1:
-            return _remove_nulls("object", property_details["anyOf"][0])
+            return _get_property_details(
+                property_details["anyOf"][0].get("type", "?"),
+                property_details["anyOf"][0],
+            )
 
     if "allOf" in property_details:
         try:
             property_details["allOf"].remove({"type": "null"})
         except Exception:
             logger.warning("No null type in allOf")
 
         if len(property_details["allOf"]) == 1:
-            return _remove_nulls("object", property_details["allOf"][0])
+            return _get_property_details(
+                property_details["allOf"][0].get("type", "?"),
+                property_details["allOf"][0],
+            )
 
     is_const = "const" in property_details
     res_type = "const" if is_const else property_type
 
     if "enum" in property_details:
         res_details = ", ".join(
             [f"`{str(value)}`" for value in property_details["enum"]]
@@ -120,84 +152,142 @@
             ]
         )
         if any("const" in value for value in property_details["allOf"]):
             res_type = "const"
     elif "items" in property_details:
         title = property_details["items"].get("title")
         _type = property_details["items"].get("type")
-        if title:
+        if "anyOf" in property_details["items"]:
+            res_details = ", ".join(
+                [
+                    _get_property_details(value.get("type", "?"), value)[1]
+                    for value in property_details["items"]["anyOf"]
+                ]
+            )
+        elif "oneOf" in property_details["items"]:
+            res_details = ", ".join(
+                [
+                    _get_property_details(value.get("type", "?"), value)[1]
+                    for value in property_details["items"]["oneOf"]
+                ]
+            )
+        elif "allOf" in property_details["items"]:
+            res_details = ", ".join(
+                [
+                    _get_property_details(value.get("type", "?"), value)[1]
+                    for value in property_details["items"]["allOf"]
+                ]
+            )
+        elif title:
             res_details = f"[{title}](#{title})"
         elif _type:
-            res_details = f"`{_type}`"
+            res_details = _type
         else:
-            res_details = "yo124"
+            res_details = "?"
     elif "pattern" in property_details:
-        pattern = property_details.get("pattern")
-        res_details = pattern
+        pattern = property_details.get("pattern", "?")
+        res_details = f"[`{pattern}`](https://regex101.com/?regex={urllib.parse.quote_plus(pattern)})"
     elif "additionalProperties" in property_details:
         title = property_details["additionalProperties"].get("title")
         _type = property_details["additionalProperties"].get("type")
         if title:
             res_details = f"[{title}](#{title})"
         elif _type:
-            res_details = f"`{_type}`"
+            res_details = f"{_type}"
         else:
             res_details = "?"
     elif is_const:
-        res_details = property_details.get("const")
+        res_details = f"`{property_details.get('const')}`"
+    elif property_type == "integer":
+        # write the range of the integer in the format a <= x <= b
+        minimum = property_details.get("minimum")
+        maximum = property_details.get("maximum")
+        exclusive_minimum = property_details.get("exclusiveMinimum")
+        exclusive_maximum = property_details.get("exclusiveMaximum")
+        if minimum is not None and maximum is not None:
+            if exclusive_minimum is not None and exclusive_maximum is not None:
+                res_details = f"`{minimum} < x < {maximum}`"
+            elif exclusive_minimum is not None:
+                res_details = f"`{minimum} < x <= {maximum}`"
+            elif exclusive_maximum is not None:
+                res_details = f"`{minimum} <= x < {maximum}`"
+            else:
+                res_details = f"`{minimum} <= x <= {maximum}`"
+        elif minimum is not None:
+            if exclusive_minimum is not None:
+                res_details = f"`{minimum} < x`"
+            else:
+                res_details = f"`{minimum} <= x`"
+        elif maximum is not None:
+            if exclusive_maximum is not None:
+                res_details = f"`x < {maximum}`"
+            else:
+                res_details = f"`x <= {maximum}`"
+        else:
+            # fallback to integer when no range is specified
+            res_details = property_type
+
     else:
         title = property_details.get("title")
-        res_type = res_type if res_type else property_details.get("type", "??")
+        res_type = res_type if res_type else property_details.get("type", "?")
         if title and res_type != "string" and res_type != "boolean" and not is_const:
             res_details = f"[{title}](#{title.replace(' ', '-')})"
         elif res_type:
-            res_details = f"`{res_type}`"
+            res_details = f"{res_type}"
         else:
-            res_details = "???"
+            res_details = "?"
 
     return res_type, res_details
 
 
-def _create_table_of_properties(schema: dict) -> str:
+def _create_definition_table(schema: dict) -> str:
     """
     Create a table of the properties in the schema.
     Outputs a markdown table with the following columns:
     - Property name
     - Type
     - Required
     - Possible Values / Definition Subschema
     - Deprecated
     - Default value
     - Description
 
     Search for deprecated string in the description or a deprecated key set to true in the property
     """
-    if "properties" not in schema:
-        return ""
+
+    if schema.get("enum"):
+        return _create_enum_markdown(schema)
+
+    if schema.get("const"):
+        return _create_const_markdown(schema)
+
     schema["properties"] = _sort_properties(schema)
 
     markdown = ""
 
     # Add a warning before the table to indicate if additional properties are allowed
     if not schema.get("additionalProperties", True):
         markdown += "> ⚠️ Additional properties are not allowed.\n\n"
 
     markdown += "| Property | Type | Required | Possible Values | Deprecated | Default | Description |\n"
     markdown += "| -------- | ---- | -------- | --------------- | ---------- | ------- | ----------- |\n"
 
     for property_name, property_details in schema["properties"].items():
         property_type = property_details.get("type", property_details.get("const"))
 
-        property_type, possible_values = _remove_nulls(property_type, property_details)
+        property_type, possible_values = _get_property_details(
+            property_type, property_details
+        )
 
         default = property_details.get("default")
+        description = property_details.get("description", "").strip(" \n")
 
         markdown += (
-            f"| {property_name} | {property_type.capitalize()} | "
+            f"| {property_name} | `{property_type}` | "
             f"{'✅' if property_name in schema.get('required', []) else ''} | "
             f"{possible_values}| "
             f"{'⛔️' if '[deprecated]' in str(property_details.get('description','')).lower() or property_details.get('deprecated') else ''} | "
             f"{'`'+json.dumps(default)+'`' if default else ''} | "
-            f"{property_details.get('description','')} |\n"
+            f"{description} |\n"
         )
 
     return markdown
```

## jsonschema_markdown/main.py

```diff
@@ -1,25 +1,22 @@
 import json
 
 import click
-import jsonref
 
 import jsonschema_markdown
 
 
 @click.command()
 @click.argument("filename", type=click.Path(exists=True))
 @click.version_option(package_name="jsonschema_markdown")
 def cli(filename):
     """
     Load a file and output the markdown.
     """
     with open(filename, "r") as f:
         file_contents = json.load(f)
 
-    file_contents: dict = jsonref.replace_refs(file_contents)  # type: ignore
-
     # Convert the file contents to markdown
     markdown = jsonschema_markdown.generate(file_contents)
 
     # Output the markdown
     click.echo(markdown)
```

## Comparing `jsonschema_markdown-0.1.2.dist-info/LICENSE` & `jsonschema_markdown-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jsonschema_markdown-0.1.2.dist-info/METADATA` & `jsonschema_markdown-0.1.3.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.1.2
+Version: 0.1.3
 Summary: Export a JSON Schema document to Markdown documentation.
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,7 +13,9 @@
 Requires-Dist: click (>=8.1.5,<9.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # jsonschema-markdown
 
+WIP
+
```

## Comparing `jsonschema_markdown-0.1.2.dist-info/RECORD` & `jsonschema_markdown-0.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 jsonschema_markdown/__init__.py,sha256=6UdpCb2kIhAJZ3NiKvVW6E630TOBKjuml9zDpwUlZJw,81
 jsonschema_markdown/converter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jsonschema_markdown/converter/markdown.py,sha256=W6d5jTTO-YTwOv96Xr2wHe33hFOlWfAv40WagG7HlAc,7041
-jsonschema_markdown/main.py,sha256=NzXBQJXuS8SAMUqMwUV5gNXkvdJ3hv4SLHzQJ44pCLY,587
+jsonschema_markdown/converter/markdown.py,sha256=eTKyuSPZkRMPQ8-a_-BuJdlwSXavdn2yPszqkW8lyAI,10399
+jsonschema_markdown/main.py,sha256=HXvdqCvWApK1Cc1zjH8nv588x7MLiRnMs15GAMM7nUg,493
 jsonschema_markdown/parser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/parser/parser.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jsonschema_markdown/utils/enums.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jsonschema_markdown-0.1.2.dist-info/LICENSE,sha256=axN1TC4zNO_qVsrYheL5eB8fg6N4djrQEGgJY4NeMhU,1073
-jsonschema_markdown-0.1.2.dist-info/METADATA,sha256=3vYCiMyyIGmOUzwMyHBaKq1Jfw7zqS2cdoRaNXBULEE,646
-jsonschema_markdown-0.1.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-jsonschema_markdown-0.1.2.dist-info/entry_points.txt,sha256=M6MzkSl1InYyJeflgFfh1Ewa-KluWxOWvDMWsSA7hrY,68
-jsonschema_markdown-0.1.2.dist-info/RECORD,,
+jsonschema_markdown-0.1.3.dist-info/LICENSE,sha256=axN1TC4zNO_qVsrYheL5eB8fg6N4djrQEGgJY4NeMhU,1073
+jsonschema_markdown-0.1.3.dist-info/METADATA,sha256=sbFFk5cOLrsnN50LhespR2Ip85IcmVB51ZERVQxwVMg,651
+jsonschema_markdown-0.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+jsonschema_markdown-0.1.3.dist-info/entry_points.txt,sha256=M6MzkSl1InYyJeflgFfh1Ewa-KluWxOWvDMWsSA7hrY,68
+jsonschema_markdown-0.1.3.dist-info/RECORD,,
```


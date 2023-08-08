# Comparing `tmp/jsonschema_markdown-0.1.4-py3-none-any.whl.zip` & `tmp/jsonschema_markdown-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,11 @@
-Zip file size: 6338 bytes, number of entries: 13
+Zip file size: 6498 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 jsonschema_markdown/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/__init__.py
--rw-r--r--  2.0 unx    10399 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
+-rw-r--r--  2.0 unx    10407 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
 -rw-r--r--  2.0 unx      493 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/parser/parser.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils/enums.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1277 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1173 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.4.dist-info/RECORD
-13 files, 14652 bytes uncompressed, 4314 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.1.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      812 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.1.5.dist-info/RECORD
+9 files, 16085 bytes uncompressed, 5068 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -6,35 +6,23 @@
 
 Filename: jsonschema_markdown/converter/markdown.py
 Comment: 
 
 Filename: jsonschema_markdown/main.py
 Comment: 
 
-Filename: jsonschema_markdown/parser/__init__.py
+Filename: jsonschema_markdown-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: jsonschema_markdown/parser/parser.py
+Filename: jsonschema_markdown-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: jsonschema_markdown/utils/__init__.py
+Filename: jsonschema_markdown-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: jsonschema_markdown/utils/enums.py
+Filename: jsonschema_markdown-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: jsonschema_markdown-0.1.4.dist-info/LICENSE
-Comment: 
-
-Filename: jsonschema_markdown-0.1.4.dist-info/METADATA
-Comment: 
-
-Filename: jsonschema_markdown-0.1.4.dist-info/WHEEL
-Comment: 
-
-Filename: jsonschema_markdown-0.1.4.dist-info/entry_points.txt
-Comment: 
-
-Filename: jsonschema_markdown-0.1.4.dist-info/RECORD
+Filename: jsonschema_markdown-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonschema_markdown/converter/markdown.py

```diff
@@ -226,15 +226,15 @@
             # fallback to integer when no range is specified
             res_details = property_type
 
     else:
         title = property_details.get("title")
         res_type = res_type if res_type else property_details.get("type", "?")
         if title and res_type != "string" and res_type != "boolean" and not is_const:
-            res_details = f"[{title}](#{title.replace(' ', '-')})"
+            res_details = f"[{title}](#{title.replace(' ', '-').lower()})"
         elif res_type:
             res_details = f"{res_type}"
         else:
             res_details = "?"
 
     return res_type, res_details
```

## Comparing `jsonschema_markdown-0.1.4.dist-info/LICENSE` & `jsonschema_markdown-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*


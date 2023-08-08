# Comparing `tmp/normalize_json-0.0.4.tar.gz` & `tmp/normalize_json-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normalize_json-0.0.4.tar", last modified: Mon Aug  7 19:50:11 2023, max compression
+gzip compressed data, was "normalize_json-0.0.6.tar", last modified: Tue Aug  8 18:54:00 2023, max compression
```

## Comparing `normalize_json-0.0.4.tar` & `normalize_json-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/
--rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.4/LICENSE
--rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-07 19:50:11.711550 normalize_json-0.0.4/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)     4160 2023-08-07 04:06:44.000000 normalize_json-0.0.4/README.md
--rw-r--r--   0 mega      (1000) mega      (1000)      506 2023-08-07 19:48:44.000000 normalize_json-0.0.4/pyproject.toml
--rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-07 19:50:11.711550 normalize_json-0.0.4/setup.cfg
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/normalize_json/
--rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.4/src/normalize_json/__init__.py
--rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.4/src/normalize_json/cli.py
--rw-r--r--   0 mega      (1000) mega      (1000)     6845 2023-08-07 19:48:26.000000 normalize_json-0.0.4/src/normalize_json/normalize.py
-drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-07 19:50:11.711550 normalize_json-0.0.4/src/normalize_json.egg-info/
--rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/PKG-INFO
--rw-r--r--   0 mega      (1000) mega      (1000)      289 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/SOURCES.txt
--rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/dependency_links.txt
--rw-r--r--   0 mega      (1000) mega      (1000)       15 2023-08-07 19:50:11.000000 normalize_json-0.0.4/src/normalize_json.egg-info/top_level.txt
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-08 18:54:00.491101 normalize_json-0.0.6/
+-rw-r--r--   0 mega      (1000) mega      (1000)     1083 2023-08-04 22:32:02.000000 normalize_json-0.0.6/LICENSE
+-rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-08 18:54:00.491101 normalize_json-0.0.6/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)     4160 2023-08-07 04:06:44.000000 normalize_json-0.0.6/README.md
+-rw-r--r--   0 mega      (1000) mega      (1000)      506 2023-08-08 18:53:46.000000 normalize_json-0.0.6/pyproject.toml
+-rw-r--r--   0 mega      (1000) mega      (1000)       38 2023-08-08 18:54:00.491101 normalize_json-0.0.6/setup.cfg
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-08 18:54:00.487767 normalize_json-0.0.6/src/
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-08 18:54:00.487767 normalize_json-0.0.6/src/normalize_json/
+-rw-r--r--   0 mega      (1000) mega      (1000)       25 2023-08-04 23:11:44.000000 normalize_json-0.0.6/src/normalize_json/__init__.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     1410 2023-08-05 00:11:28.000000 normalize_json-0.0.6/src/normalize_json/cli.py
+-rw-r--r--   0 mega      (1000) mega      (1000)     7706 2023-08-07 23:48:29.000000 normalize_json-0.0.6/src/normalize_json/normalize.py
+drwxr-xr-x   0 mega      (1000) mega      (1000)        0 2023-08-08 18:54:00.491101 normalize_json-0.0.6/src/normalize_json.egg-info/
+-rw-r--r--   0 mega      (1000) mega      (1000)     4593 2023-08-08 18:54:00.000000 normalize_json-0.0.6/src/normalize_json.egg-info/PKG-INFO
+-rw-r--r--   0 mega      (1000) mega      (1000)      289 2023-08-08 18:54:00.000000 normalize_json-0.0.6/src/normalize_json.egg-info/SOURCES.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)        1 2023-08-08 18:54:00.000000 normalize_json-0.0.6/src/normalize_json.egg-info/dependency_links.txt
+-rw-r--r--   0 mega      (1000) mega      (1000)       15 2023-08-08 18:54:00.000000 normalize_json-0.0.6/src/normalize_json.egg-info/top_level.txt
```

### Comparing `normalize_json-0.0.4/LICENSE` & `normalize_json-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.4/PKG-INFO` & `normalize_json-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normalize_json
-Version: 0.0.4
+Version: 0.0.6
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `normalize_json-0.0.4/README.md` & `normalize_json-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.4/src/normalize_json/cli.py` & `normalize_json-0.0.6/src/normalize_json/cli.py`

 * *Files identical despite different names*

### Comparing `normalize_json-0.0.4/src/normalize_json/normalize.py` & `normalize_json-0.0.6/src/normalize_json/normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,30 +44,31 @@
     'trim_start': typing.NotRequired[int],
     'trim_end': typing.NotRequired[int],
     'pick_until': typing.NotRequired[str],
     '__fields': typing.NotRequired[dict[str, 'Node']]
 })
 
 Mapping = typing.TypedDict('Mapping', {
+    'array': typing.NotRequired[bool],
     'modifiers': typing.NotRequired[list[Modifier]],
     '__fields': typing.NotRequired[dict[str, 'Node']]
 })
 
 StringMapping = typing.TypedDict('StringMapping', {
     '__fields': dict[str, str | list[str]]
 })
 
 RawObject = dict[str, typing.Any]
 
-def unserialize(raw: RawObject | str | bytes, mime: AcceptedMime = 'application/json'):
+def unserialize(raw: typing.Any, mime: AcceptedMime = 'application/json'):
     match mime:
         case 'application/json':
-            if isinstance(raw, dict): return raw
-            if isinstance(raw, str): return raw
-            else: return json.loads(raw)
+            if isinstance(raw, str): return json.loads(raw)
+            if isinstance(raw, bytes): return json.loads(raw)
+            else: return raw
 
     raise TypeError('invalid mime')
 
 def flatten(target: RawObject, separator: str = '.', preserve_arrays: bool = False):
     ret: RawObject = {}
 
     def internal_flatten(obj: typing.Any, parent: str = '') -> typing.Any:
@@ -86,28 +87,33 @@
         else:
             ret[parent] = obj
 
     internal_flatten(target)
     return ret
 
 
-def check_types(node: Node, value: typing.Any, expected: typing.Any):
+def check_types(node: Node, value: typing.Any, expected: typing.Any, modifiers: list[Modifier]):
+    if node.get('array') and value == []:
+        return None
+
     actual = value[0].__class__.__name__ \
         if node.get('array') \
         else value.__class__.__name__
 
     vexpected = TYPE_MAPPING.get(str(expected))
     if actual == vexpected \
-            or (actual == 'int' and vexpected in ['number', 'float']):
+            or (actual == 'int' and vexpected in ['number', 'float']) \
+            or (actual == 'NoneType' and 'default_null' in modifiers):
         return None
 
     return actual, str(expected)
 
 def handle_modifiers(node: Node, modifiers: list[Modifier], old_value: typing.Any):
     value = old_value
+
     if not value:
         if 'default' in node:
             value = node['default']
         elif 'default_null' in modifiers:
             return None
         else:
             raise ValueError('value for %s wasnt provided' % node.get('map'))
@@ -127,18 +133,18 @@
             case 'integer': value = int(value)
             case 'string': value = str(value)
             case 'datetime': value = dateparser.parse(value)
             case _: ...
 
     return value
 
-def get_initial_value(target: typing.Any, original_name: str, flat_obj: RawObject):
-    initial_value = flat_obj.get(original_name) \
-        if original_name[0] == '.' \
-        else target.get(original_name)
+def get_initial_value(target: typing.Any, mapped_name: str, flat_obj: RawObject):
+    initial_value = flat_obj.get(mapped_name) \
+        if mapped_name[0] == '.' or mapped_name[:2] == '[]' \
+        else target.get(mapped_name)
 
     return initial_value
 
 
 def translate(target: T | tuple[T, int], mapping: Mapping, acc: RawObject = {}, inherited_modifiers: list[Modifier] | None = None, inherited_flat_obj: tuple[RawObject, RawObject] | None = None) -> T:
     ret: RawObject = {}
     flat_obj, flat_obj_arr = inherited_flat_obj or (
@@ -162,39 +168,58 @@
             mapped_type = node['type']
             initial_value: typing.Any = None
 
             modifiers = node.get('modifiers', root_modifiers)
             if 'reverse' in modifiers:
                 mapped_name, original_name = original_name, mapped_name
 
+            if not mapped_name:
+                continue
+
             for n in mapped_name if isinstance(mapped_name, list) else mapped_name.split('|'):
-                n = n.strip()
-                if typing.cast(RawObject, target).get(n):
-                    mapped_name = n
-                elif flat_obj.get(n):
-                    mapped_name = n
-                    initial_value = flat_obj[n]
-                elif '[]' in n:
-                    mapped_name = n.replace('[]', '[%d]' % target_index)
+                mapped_name = n.strip()
+
+                if '[]' in mapped_name:
+                    mapped_name = mapped_name.replace('[]', '[%d]' % target_index)
+
+                if typing.cast(typing.Any, target).get(mapped_name):
+                    initial_value = target[mapped_name]
+                    break
+                elif flat_obj.get(mapped_name):
+                    mapped_name = mapped_name
+                    initial_value = flat_obj[mapped_name]
+                    break
                 elif mapped_name in flat_obj_arr:
                     initial_value = flat_obj_arr.get(mapped_name)
+                    break
 
             mapped_name = typing.cast(str, mapped_name)
             original_name = typing.cast(str, original_name)
 
             if '__fields' in node:
-                child: typing.Any = initial_value or target[mapped_name]
-                ret[original_name] = translate(child, node, acc, modifiers, (flat_obj, flat_obj_arr))
+                if not node.get('map'):
+                    value = translate(typing.cast(typing.Any, target), node, acc, modifiers)
+                else:
+                    child: typing.Any = initial_value or target[original_name]
+                    value = translate(child, node, acc, modifiers, (flat_obj, flat_obj_arr))
+
+                if node.get('array') and not isinstance(value, list):
+                    value = [value]
+
+                ret[original_name] = value
                 continue
 
             if not initial_value:
                 initial_value = get_initial_value(target, mapped_name, flat_obj)
 
             value = handle_modifiers(node, modifiers, initial_value)
-            if err := check_types(node, value, mapped_type):
+            if node.get('array') and not isinstance(value, list):
+                value = [value]
+
+            if err := check_types(node, value, mapped_type, modifiers):
                 raise ValueError('check_types @ %s (got "%s", expected "%s")' % (original_name, *err))
 
             ret[original_name] = value
 
     if isinstance(target, list):
         if not mapping.get('array'):
             raise ValueError('illegal array')
```

### Comparing `normalize_json-0.0.4/src/normalize_json.egg-info/PKG-INFO` & `normalize_json-0.0.6/src/normalize_json.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normalize-json
-Version: 0.0.4
+Version: 0.0.6
 Summary: todo
 Author-email: João Gabriel Santos <joaosan177@gmail.com>
 Project-URL: Homepage, https://github.com/capsulbrasil/normalize-json
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```


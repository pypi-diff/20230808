# Comparing `tmp/mango_odm-0.3.1.tar.gz` & `tmp/mango_odm-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_odm-0.3.1.tar", last modified: Tue Aug  1 13:20:22 2023, max compression
+gzip compressed data, was "mango_odm-0.3.2.tar", last modified: Tue Aug  8 13:24:05 2023, max compression
```

## Comparing `mango_odm-0.3.1.tar` & `mango_odm-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1064 2023-08-01 13:20:12.075699 mango_odm-0.3.1/LICENSE
--rw-r--r--   0        0        0     4815 2023-08-01 13:20:12.075699 mango_odm-0.3.1/README.md
--rw-r--r--   0        0        0      445 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/__init__.py
--rw-r--r--   0        0        0     4331 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/drive.py
--rw-r--r--   0        0        0     1110 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/encoder.py
--rw-r--r--   0        0        0     5639 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/expression.py
--rw-r--r--   0        0        0     3284 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/fields.py
--rw-r--r--   0        0        0     1665 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/index.py
--rw-r--r--   0        0        0     1040 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/meta.py
--rw-r--r--   0        0        0     9261 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/models.py
--rw-r--r--   0        0        0        0 2023-08-01 13:20:12.075699 mango_odm-0.3.1/mango/py.typed
--rw-r--r--   0        0        0     6570 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/result.py
--rw-r--r--   0        0        0     2221 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/source.py
--rw-r--r--   0        0        0    16192 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/stage.py
--rw-r--r--   0        0        0     4391 2023-08-01 13:20:12.079699 mango_odm-0.3.1/mango/utils.py
--rw-r--r--   0        0        0     2533 2023-08-01 13:20:22.235786 mango_odm-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 mango_odm-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-08 13:23:57.531989 mango_odm-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4815 2023-08-08 13:23:57.531989 mango_odm-0.3.2/README.md
+-rw-r--r--   0        0        0      445 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/__init__.py
+-rw-r--r--   0        0        0     4331 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/drive.py
+-rw-r--r--   0        0        0     1110 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/encoder.py
+-rw-r--r--   0        0        0     5639 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/expression.py
+-rw-r--r--   0        0        0     3284 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/fields.py
+-rw-r--r--   0        0        0     1665 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/index.py
+-rw-r--r--   0        0        0     1040 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/meta.py
+-rw-r--r--   0        0        0     9294 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/models.py
+-rw-r--r--   0        0        0        0 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/py.typed
+-rw-r--r--   0        0        0     6570 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/result.py
+-rw-r--r--   0        0        0     2221 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/source.py
+-rw-r--r--   0        0        0    16192 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/stage.py
+-rw-r--r--   0        0        0     4405 2023-08-08 13:23:57.531989 mango_odm-0.3.2/mango/utils.py
+-rw-r--r--   0        0        0     2533 2023-08-08 13:24:05.240160 mango_odm-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6047 1970-01-01 00:00:00.000000 mango_odm-0.3.2/PKG-INFO
```

### Comparing `mango_odm-0.3.1/LICENSE` & `mango_odm-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/README.md` & `mango_odm-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/drive.py` & `mango_odm-0.3.2/mango/drive.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/encoder.py` & `mango_odm-0.3.2/mango/encoder.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/expression.py` & `mango_odm-0.3.2/mango/expression.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/fields.py` & `mango_odm-0.3.2/mango/fields.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/index.py` & `mango_odm-0.3.2/mango/index.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/meta.py` & `mango_odm-0.3.2/mango/meta.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/models.py` & `mango_odm-0.3.2/mango/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         if key.startswith(operators):
             flatted |= flat_filter(reduce(lambda x, y: x | y, value))
         elif "." in key:
             parent, child = key.split(".", maxsplit=1)
             flatted[parent] = flat_filter({child: value})
         else:
             for operator in operators:
-                if ov := value.get(operator):
-                    flatted[key] = ov
+                if isinstance(value, dict) and operator in value:
+                    flatted[key] = value[operator]
     return flatted
 
 
 def merge_map(data: MutableMapping[Any, Any], into: Mapping[Any, Any]) -> None:
     for k, v in into.items():
         k = str(k)
         if isinstance(data.get(k), dict) and isinstance(v, dict | EmbeddedDocument):
```

### Comparing `mango_odm-0.3.1/mango/result.py` & `mango_odm-0.3.2/mango/result.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/source.py` & `mango_odm-0.3.2/mango/source.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/stage.py` & `mango_odm-0.3.2/mango/stage.py`

 * *Files identical despite different names*

### Comparing `mango_odm-0.3.1/mango/utils.py` & `mango_odm-0.3.2/mango/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             if index := finfo.index:
                 if index is True:
                     yield Index(name)
                 elif isinstance(index, IndexType):
                     yield Index((name, index))
                 else:
                     yield index
-            elif expire := finfo.expire:
+            elif (expire := finfo.expire) is not None:
                 yield Index(name, expireAfterSeconds=expire)
 
     for index in model.__meta__.indexes:
         if isinstance(index, str):
             yield Index(index)
         elif isinstance(index, Sequence):
             yield Index(*index)
```

### Comparing `mango_odm-0.3.1/pyproject.toml` & `mango_odm-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mango-odm"
-version = "0.3.1"
+version = "0.3.2"
 description = "🥭 Async MongoDB ODM with type hints in Python"
 authors = [
     { name = "Akirami", email = "akiramiaya@outlook.com" },
 ]
 requires-python = ">=3.10,<4.0"
 readme = "README.md"
 keywords = [
```

### Comparing `mango_odm-0.3.1/PKG-INFO` & `mango_odm-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-odm
-Version: 0.3.1
+Version: 0.3.2
 Summary: 🥭 Async MongoDB ODM with type hints in Python
 Keywords: mongo mongodb async asyncio odm types pydantic motor
 Author-Email: Akirami <akiramiaya@outlook.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```


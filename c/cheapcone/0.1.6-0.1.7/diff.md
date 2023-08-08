# Comparing `tmp/cheapcone-0.1.6.tar.gz` & `tmp/cheapcone-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.6.tar", max compression
+gzip compressed data, was "cheapcone-0.1.7.tar", max compression
```

## Comparing `cheapcone-0.1.6.tar` & `cheapcone-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.6/README.md
--rw-r--r--   0        0        0       41 2023-08-08 08:02:52.084595 cheapcone-0.1.6/cheapcone/__init__.py
--rw-r--r--   0        0        0     5596 2023-08-08 08:01:45.352735 cheapcone-0.1.6/cheapcone/client.py
--rw-r--r--   0        0        0     2330 2023-08-08 08:01:57.908708 cheapcone-0.1.6/cheapcone/json.py
--rw-r--r--   0        0        0     1138 2023-08-08 08:02:56.792585 cheapcone-0.1.6/cheapcone/proxy.py
--rw-r--r--   0        0        0     1123 2023-08-08 08:02:54.632590 cheapcone-0.1.6/cheapcone/schemas.py
--rw-r--r--   0        0        0     2902 2023-08-08 08:02:55.744588 cheapcone-0.1.6/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-08 08:04:25.312413 cheapcone-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.7/README.md
+-rw-r--r--   0        0        0       41 2023-08-08 08:02:52.084595 cheapcone-0.1.7/cheapcone/__init__.py
+-rw-r--r--   0        0        0     5596 2023-08-08 08:01:45.352735 cheapcone-0.1.7/cheapcone/client.py
+-rw-r--r--   0        0        0     2330 2023-08-08 08:01:57.908708 cheapcone-0.1.7/cheapcone/json.py
+-rw-r--r--   0        0        0     1138 2023-08-08 08:02:56.792585 cheapcone-0.1.7/cheapcone/proxy.py
+-rw-r--r--   0        0        0     1123 2023-08-08 08:02:54.632590 cheapcone-0.1.7/cheapcone/schemas.py
+-rw-r--r--   0        0        0     2686 2023-08-08 09:22:47.138172 cheapcone-0.1.7/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-08 09:22:55.405921 cheapcone-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.7/PKG-INFO
```

### Comparing `cheapcone-0.1.6/cheapcone/client.py` & `cheapcone-0.1.7/cheapcone/client.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.6/cheapcone/json.py` & `cheapcone-0.1.7/cheapcone/json.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.6/cheapcone/proxy.py` & `cheapcone-0.1.7/cheapcone/proxy.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.6/cheapcone/schemas.py` & `cheapcone-0.1.7/cheapcone/schemas.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.6/cheapcone/typedefs.py` & `cheapcone-0.1.7/cheapcone/typedefs.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,15 @@
     Dict[AndOr, List[Dict[str, Union[Value, "Query", List[Value], List["Query"]]]]],
 ]
 
 
 class CheapModel(BaseModel):
     """Cheap model that allow cheap serialization and deserialization."""
 
-    @classmethod
-    def __init_subclass__(cls, **kwargs):
-        super().__init_subclass__(**kwargs)
-        cls.__doc__ = cls.schema_json()
-        cls.__repr__ = cls.schema_json
-        cls.__str__ = cls.schema_json
+   
 
     def json(self, *args, **kwargs) -> str:
         """Serialize the model to JSON."""
         return dumps(self.dict())
 
     @classmethod
     def parse(cls, s: str) -> CheapModel:
```


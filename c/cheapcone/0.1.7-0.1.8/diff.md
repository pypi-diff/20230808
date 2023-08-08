# Comparing `tmp/cheapcone-0.1.7.tar.gz` & `tmp/cheapcone-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.7.tar", max compression
+gzip compressed data, was "cheapcone-0.1.8.tar", max compression
```

## Comparing `cheapcone-0.1.7.tar` & `cheapcone-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.7/README.md
--rw-r--r--   0        0        0       41 2023-08-08 08:02:52.084595 cheapcone-0.1.7/cheapcone/__init__.py
--rw-r--r--   0        0        0     5596 2023-08-08 08:01:45.352735 cheapcone-0.1.7/cheapcone/client.py
--rw-r--r--   0        0        0     2330 2023-08-08 08:01:57.908708 cheapcone-0.1.7/cheapcone/json.py
--rw-r--r--   0        0        0     1138 2023-08-08 08:02:56.792585 cheapcone-0.1.7/cheapcone/proxy.py
--rw-r--r--   0        0        0     1123 2023-08-08 08:02:54.632590 cheapcone-0.1.7/cheapcone/schemas.py
--rw-r--r--   0        0        0     2686 2023-08-08 09:22:47.138172 cheapcone-0.1.7/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-08 09:22:55.405921 cheapcone-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.8/README.md
+-rw-r--r--   0        0        0       41 2023-08-08 08:02:52.084595 cheapcone-0.1.8/cheapcone/__init__.py
+-rw-r--r--   0        0        0     5596 2023-08-08 08:01:45.352735 cheapcone-0.1.8/cheapcone/client.py
+-rw-r--r--   0        0        0     2330 2023-08-08 08:01:57.908708 cheapcone-0.1.8/cheapcone/json.py
+-rw-r--r--   0        0        0     1138 2023-08-08 08:02:56.792585 cheapcone-0.1.8/cheapcone/proxy.py
+-rw-r--r--   0        0        0     1122 2023-08-08 09:41:10.952487 cheapcone-0.1.8/cheapcone/schemas.py
+-rw-r--r--   0        0        0     2679 2023-08-08 09:39:47.321238 cheapcone-0.1.8/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-08 09:43:14.887445 cheapcone-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.8/PKG-INFO
```

### Comparing `cheapcone-0.1.7/cheapcone/client.py` & `cheapcone-0.1.8/cheapcone/client.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.7/cheapcone/json.py` & `cheapcone-0.1.8/cheapcone/json.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.7/cheapcone/proxy.py` & `cheapcone-0.1.8/cheapcone/proxy.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.7/cheapcone/schemas.py` & `cheapcone-0.1.8/cheapcone/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     metadata: MetaData = Field(...)
 
 
 class QueryRequest(CheapModel):
     """Request to query for similar vectors."""
 
     topK: int = Field(default=10)
-    filter: Query = Field(...)
+    filter: dict = Field(...)
     includeMetadata: bool = Field(default=True)
     vector: Vector = Field(...)
 
 
 class QueryMatch(CheapModel):
     """A single match from a query."""
```

### Comparing `cheapcone-0.1.7/cheapcone/typedefs.py` & `cheapcone-0.1.8/cheapcone/typedefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 
    
 
     def json(self, *args, **kwargs) -> str:
         """Serialize the model to JSON."""
         return dumps(self.dict())
 
-    @classmethod
-    def parse(cls, s: str) -> CheapModel:
-        """Deserialize the model from JSON."""
-        return cls(**loads(s))
 
+    def dict(self, *args, **kwargs) -> Dict:
+        """Serialize the model to a dictionary."""
+        return loads(self.json())
 
 class QueryBuilder:
     """Query builder for Pinecone Query API with MongoDB-like syntax."""
 
     def __init__(self, field: str = None, query: Query = None):  # type: ignore
         self.field = field
         self.query = query if query else {}
```


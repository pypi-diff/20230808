# Comparing `tmp/cheapcone-0.1.4.tar.gz` & `tmp/cheapcone-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.4.tar", max compression
+gzip compressed data, was "cheapcone-0.1.5.tar", max compression
```

## Comparing `cheapcone-0.1.4.tar` & `cheapcone-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.4/cheapcone/__init__.py
--rw-r--r--   0        0        0     4208 2023-08-07 09:34:44.510872 cheapcone-0.1.4/cheapcone/client.py
--rw-r--r--   0        0        0     1595 2023-08-07 09:31:42.362613 cheapcone-0.1.4/cheapcone/json.py
--rw-r--r--   0        0        0      993 2023-08-07 09:31:42.354613 cheapcone-0.1.4/cheapcone/proxy.py
--rw-r--r--   0        0        0      747 2023-08-07 09:31:42.362613 cheapcone-0.1.4/cheapcone/schemas.py
--rw-r--r--   0        0        0     2385 2023-08-07 09:34:46.402875 cheapcone-0.1.4/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-07 09:34:58.962894 cheapcone-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.5/cheapcone/__init__.py
+-rw-r--r--   0        0        0     4506 2023-08-07 10:53:57.601295 cheapcone-0.1.5/cheapcone/client.py
+-rw-r--r--   0        0        0     1595 2023-08-07 09:31:42.362613 cheapcone-0.1.5/cheapcone/json.py
+-rw-r--r--   0        0        0      993 2023-08-07 09:31:42.354613 cheapcone-0.1.5/cheapcone/proxy.py
+-rw-r--r--   0        0        0      845 2023-08-07 10:50:21.443580 cheapcone-0.1.5/cheapcone/schemas.py
+-rw-r--r--   0        0        0     2385 2023-08-07 09:34:46.402875 cheapcone-0.1.5/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-07 10:54:10.161171 cheapcone-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.5/PKG-INFO
```

### Comparing `cheapcone-0.1.4/cheapcone/client.py` & `cheapcone-0.1.5/cheapcone/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 from aiohttp import ClientSession
 from aiohttp.client import ClientResponse, ClientTimeout, TCPConnector
 from dotenv import load_dotenv
 from multidict import CIMultiDict
 from pydantic import BaseModel, Field
 
 from .proxy import LazyProxy
-from .schemas import (MetaData, Query, QueryMatch, QueryRequest, QueryResponse,
-                      UpsertRequest, UpsertResponse, Vector)
+from .schemas import (Embedding, MetaData, Query, QueryMatch, QueryRequest,
+                      QueryResponse, UpsertRequest, UpsertResponse, Vector)
 from .typedefs import Filter, QueryBuilder, Value
 
 load_dotenv()
 
 
+
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class APIClient(LazyProxy[ClientSession]):
     """
     HTTP Client:
     Base class to create HTTP clients that wrap `aiohttp.ClientSession`.
     Provides Lazy Loading through proxy objects and session reuse using the singleton pattern.
     Constructor Signature:
@@ -85,28 +86,35 @@
 
     base_url: str = field(default=environ["PINECONE_API_URL"], init=True, repr=True)
     api_key: str = field(default=environ["PINECONE_API_KEY"], init=True, repr=False)
 
     def __load__(self) -> ClientSession:
         return ClientSession(base_url=self.base_url, headers={"api-key": self.api_key})
 
-    async def upsert(self, values: Vector, metadata: MetaData) -> UpsertResponse:
+    async def upsert(self, embeddings:List[Embedding]) -> UpsertResponse:
         async with self.__load__() as session:
+            values = []
+            metadata = []
+            for embedding in embeddings:
+                values.append(embedding.values)
+                metadata.append(embedding.metadata)
+            
             async with session.post(
-                "/upsert", json=UpsertRequest(values=values, metadata=metadata).dict()
+                "/vectors/upsert", json={"vectors": [UpsertRequest(values=values, metadata=metadata).dict() for values, metadata in zip(values, metadata)]}
             ) as response:
                 return UpsertResponse(**await response.json())
 
     async def query(
         self, expr: Query, vector: Vector, includeMetadata: bool = True, topK: int = 10
     ) -> QueryResponse:
         async with self.__load__() as session:
-            async with session.post(
-                "/vectors/query",
-                json=QueryRequest(
+            payload = QueryRequest(
                     topK=topK,
                     filter=expr,
                     vector=vector,
                     includeMetadata=includeMetadata,
-                ).dict(),
+                ).dict()
+            async with session.post(
+                "/query",
+                json=payload,
             ) as response:
-                return QueryResponse(**await response.json())
+                return QueryResponse(**await response.json())
```

### Comparing `cheapcone-0.1.4/cheapcone/json.py` & `cheapcone-0.1.5/cheapcone/json.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.4/cheapcone/proxy.py` & `cheapcone-0.1.5/cheapcone/proxy.py`

 * *Files identical despite different names*

### Comparing `cheapcone-0.1.4/cheapcone/schemas.py` & `cheapcone-0.1.5/cheapcone/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 
 class UpsertRequest(CheapModel):
     id: str = Field(default_factory=lambda: str(uuid4()))
     values: Vector = Field(...)
     metadata: MetaData = Field(...)
 
+class Embedding(CheapModel):
+    values: Vector = Field(...)
+    metadata: MetaData = Field(...)
+
 
 class QueryRequest(CheapModel):
     topK: int = Field(default=10)
     filter: Query = Field(...)
     includeMetadata: bool = Field(default=True)
     vector: Vector = Field(...)
```

### Comparing `cheapcone-0.1.4/cheapcone/typedefs.py` & `cheapcone-0.1.5/cheapcone/typedefs.py`

 * *Files identical despite different names*


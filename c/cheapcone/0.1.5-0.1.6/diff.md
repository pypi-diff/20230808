# Comparing `tmp/cheapcone-0.1.5.tar.gz` & `tmp/cheapcone-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheapcone-0.1.5.tar", max compression
+gzip compressed data, was "cheapcone-0.1.6.tar", max compression
```

## Comparing `cheapcone-0.1.5.tar` & `cheapcone-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-08-07 06:22:11.313840 cheapcone-0.1.5/cheapcone/__init__.py
--rw-r--r--   0        0        0     4506 2023-08-07 10:53:57.601295 cheapcone-0.1.5/cheapcone/client.py
--rw-r--r--   0        0        0     1595 2023-08-07 09:31:42.362613 cheapcone-0.1.5/cheapcone/json.py
--rw-r--r--   0        0        0      993 2023-08-07 09:31:42.354613 cheapcone-0.1.5/cheapcone/proxy.py
--rw-r--r--   0        0        0      845 2023-08-07 10:50:21.443580 cheapcone-0.1.5/cheapcone/schemas.py
--rw-r--r--   0        0        0     2385 2023-08-07 09:34:46.402875 cheapcone-0.1.5/cheapcone/typedefs.py
--rw-r--r--   0        0        0      327 2023-08-07 10:54:10.161171 cheapcone-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-07 04:48:50.791009 cheapcone-0.1.6/README.md
+-rw-r--r--   0        0        0       41 2023-08-08 08:02:52.084595 cheapcone-0.1.6/cheapcone/__init__.py
+-rw-r--r--   0        0        0     5596 2023-08-08 08:01:45.352735 cheapcone-0.1.6/cheapcone/client.py
+-rw-r--r--   0        0        0     2330 2023-08-08 08:01:57.908708 cheapcone-0.1.6/cheapcone/json.py
+-rw-r--r--   0        0        0     1138 2023-08-08 08:02:56.792585 cheapcone-0.1.6/cheapcone/proxy.py
+-rw-r--r--   0        0        0     1123 2023-08-08 08:02:54.632590 cheapcone-0.1.6/cheapcone/schemas.py
+-rw-r--r--   0        0        0     2902 2023-08-08 08:02:55.744588 cheapcone-0.1.6/cheapcone/typedefs.py
+-rw-r--r--   0        0        0      327 2023-08-08 08:04:25.312413 cheapcone-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 cheapcone-0.1.6/PKG-INFO
```

### Comparing `cheapcone-0.1.5/cheapcone/client.py` & `cheapcone-0.1.6/cheapcone/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
+"""Pinecone API Client for the cheap developers."""
 from __future__ import annotations
 
 import asyncio
 from asyncio import Lock
 from dataclasses import dataclass, field
 from os import environ
 from typing import Dict, List, Optional, Type
 
 from aiohttp import ClientSession
 from aiohttp.client import ClientResponse, ClientTimeout, TCPConnector
 from dotenv import load_dotenv
 from multidict import CIMultiDict
-from pydantic import BaseModel, Field
 
 from .proxy import LazyProxy
 from .schemas import (Embedding, MetaData, Query, QueryMatch, QueryRequest,
                       QueryResponse, UpsertRequest, UpsertResponse, Vector)
 from .typedefs import Filter, QueryBuilder, Value
 
 load_dotenv()
 
 
-
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class APIClient(LazyProxy[ClientSession]):
     """
     HTTP Client:
     Base class to create HTTP clients that wrap `aiohttp.ClientSession`.
     Provides Lazy Loading through proxy objects and session reuse using the singleton pattern.
     Constructor Signature:
@@ -36,30 +35,33 @@
     headers: Dict[str, str] = field(default_factory=dict)
     _subclasses: Optional[List[Type[APIClient]]] = None
     _session_creation_lock = asyncio.Lock()
     _session: Optional[ClientSession] = None
 
     @classmethod
     def __init_subclass__(cls, **kwargs):
+        """Register the subclass."""
         super().__init_subclass__(**kwargs)
         if cls._subclasses is None:
             cls._subclasses = []
         cls._subclasses.append(cls)
 
     @classmethod
     async def cleanup(cls):
+        """Cleanup all the client sessions."""
         if hasattr(cls, "_subclasses") and cls._subclasses is not None:
             tasks = []
             for subclass in cls._subclasses:
                 if subclass._session is not None:
                     tasks.append(subclass._session.close())
             await asyncio.gather(*tasks)
             cls._subclasses = None
 
     async def __load__(self) -> ClientSession:
+        """Lazy load the client session."""
         async with self._session_creation_lock:
             if self._session is None:
                 self._session = ClientSession(
                     base_url=self.base_url,
                     headers=CIMultiDict(self.headers),
                     response_class=ClientResponse,
                     connector=TCPConnector(
@@ -77,44 +79,74 @@
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.base_url}>"
 
 
 @dataclass(init=True, repr=True, unsafe_hash=False, frozen=False)
 class PineconeClient(APIClient):
     """
-    Cheapcone went greedy so I had to make this one.
+    Cheapcone went greedy and removed the namespace feature from the free tier so let's query the API directly with MongoDB Filter Expressions.
+    Also it's a good example of streamlining the development of API clients.
     """
 
     base_url: str = field(default=environ["PINECONE_API_URL"], init=True, repr=True)
     api_key: str = field(default=environ["PINECONE_API_KEY"], init=True, repr=False)
 
     def __load__(self) -> ClientSession:
+        """Lazy load the client session."""
         return ClientSession(base_url=self.base_url, headers={"api-key": self.api_key})
 
-    async def upsert(self, embeddings:List[Embedding]) -> UpsertResponse:
+    async def upsert(self, embeddings: List[Embedding]) -> UpsertResponse:
+        """
+        upsert
+        Upsert embeddings into the vector index.
+
+        Args:
+            embeddings (List[Embedding]): Embeddings to upsert.
+
+        Returns:
+            UpsertResponse: Upsert response.
+        """
         async with self.__load__() as session:
             values = []
             metadata = []
             for embedding in embeddings:
                 values.append(embedding.values)
                 metadata.append(embedding.metadata)
-            
+
             async with session.post(
-                "/vectors/upsert", json={"vectors": [UpsertRequest(values=values, metadata=metadata).dict() for values, metadata in zip(values, metadata)]}
+                "/vectors/upsert",
+                json={
+                    "vectors": [
+                        UpsertRequest(values=values, metadata=metadata).dict()
+                        for values, metadata in zip(values, metadata)
+                    ]
+                },
             ) as response:
                 return UpsertResponse(**await response.json())
 
     async def query(
         self, expr: Query, vector: Vector, includeMetadata: bool = True, topK: int = 10
     ) -> QueryResponse:
+        """query
+        Query the vector index.
+
+        Args:
+            expr (Query): Query expression.
+            vector (Vector): Query vector.
+            includeMetadata (bool, optional): Whether to include metadata in the response. Defaults to True.
+            topK (int, optional): Number of results to return. Defaults to 10.
+
+        Returns:
+            QueryResponse: Query response.
+        """
         async with self.__load__() as session:
             payload = QueryRequest(
-                    topK=topK,
-                    filter=expr,
-                    vector=vector,
-                    includeMetadata=includeMetadata,
-                ).dict()
+                topK=topK,
+                filter=expr,
+                vector=vector,
+                includeMetadata=includeMetadata,
+            ).dict()
             async with session.post(
                 "/query",
                 json=payload,
             ) as response:
-                return QueryResponse(**await response.json())
+                return QueryResponse(**await response.json())
```

### Comparing `cheapcone-0.1.5/cheapcone/json.py` & `cheapcone-0.1.6/cheapcone/json.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,68 @@
+"""JSON serialization and deserialization for Pinecone."""
 from datetime import datetime
 from json import JSONDecoder, JSONEncoder
 from typing import Any, NamedTuple
 from uuid import UUID
 
-from pydantic import BaseModel
+from pydantic import BaseModel  # pylint: disable=no-name-in-module
+from typing_extensions import override
 
 
 class PineconeEncoder(JSONEncoder):
+    """Serialize UUID, datetime, NamedTuple, and Pydantic models."""
+
     def default(self, obj: Any) -> Any:
+        """Serialize UUID, datetime, NamedTuple, and Pydantic models."""
         if isinstance(obj, UUID):
             return str(obj)
         elif isinstance(obj, datetime):
             return obj.astimezone().isoformat()
         elif isinstance(obj, NamedTuple):
             return obj._asdict()
         elif isinstance(obj, BaseModel):
             return obj.dict()
         else:
             return super().default(obj)
 
 
 class PineconeDecoder(JSONDecoder):
+    """Deserialize UUID, datetime, NamedTuple, and Pydantic models."""
+
     def __init__(self, *args, **kwargs):
+        """Deserialize UUID, datetime, NamedTuple, and Pydantic models."""
         kwargs["object_hook"] = self.object_hook
         super().__init__(*args, **kwargs)
 
+    @override
     def object_hook(self, obj: Any) -> Any:
+        """Deserialize UUID, datetime, NamedTuple, and Pydantic models."""
         if "uuid" in obj:
             return UUID(obj["uuid"])
         elif "datetime" in obj:
             return datetime.fromisoformat(obj["datetime"])
         elif "type" in obj and "fields" in obj:
             return self.named_tuple_hook(obj)
         elif "type" in obj and "data" in obj:
             return self.pydantic_hook(obj)
         else:
             return obj
 
     def named_tuple_hook(self, obj: Any) -> Any:
+        """Deserialize NamedTuple."""
         cls = NamedTuple(obj["type"], obj["fields"])
         return cls(*obj["values"])
 
     def pydantic_hook(self, obj: Any) -> Any:
+        """Deserialize Pydantic models."""
         cls = getattr(__import__(obj["type"]), obj["type"])
         return cls(**obj["data"])
 
 
 def dumps(obj: Any) -> str:
+    """Serialize UUID, datetime, NamedTuple, and Pydantic models."""
     return PineconeEncoder().encode(obj)
 
 
 def loads(s: str) -> Any:
+    """Deserialize UUID, datetime, NamedTuple, and Pydantic models."""
     return PineconeDecoder().decode(s)
```

### Comparing `cheapcone-0.1.5/cheapcone/proxy.py` & `cheapcone-0.1.6/cheapcone/proxy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+"""Lazy proxy class that loads the proxied object on first access."""
 from abc import ABC, abstractmethod
 from typing import Generic, Iterable, TypeVar, Union, cast
 
 T = TypeVar("T")
 
 
 class LazyProxy(Generic[T], ABC):
+    """Lazy proxy class that loads the proxied object on first access."""
+
     def __init__(self) -> None:
         self.__proxied: Union[T, None] = None
 
     def __getattr__(self, attr: str) -> object:
         return getattr(self.__get_proxied__(), attr)
 
     def __repr__(self) -> str:
```

### Comparing `cheapcone-0.1.5/cheapcone/typedefs.py` & `cheapcone-0.1.6/cheapcone/typedefs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,50 @@
+"""Type definitions for CheapCone."""
 from __future__ import annotations
 
-from typing import (Any, Callable, Dict, Generic, List, Literal, Optional,
-                    Tuple, Type, TypeVar, Union, cast)
-from uuid import UUID, uuid4
+from typing import Dict, List, Literal, Union
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel  # pylint: disable=no-name-in-module
 
 from .json import dumps, loads
 
 Vector = List[float]
-Value = Union[str, int, float, bool, List[str]]
+Value = str | int | float | bool | List[str]
 MetaData = Dict[str, Value]
 Filter = Literal["$eq", "$ne", "$lt", "$lte", "$gt", "$gte", "$in", "$nin"]
 AndOr = Literal["$and", "$or"]
 Query = Union[
     Dict[str, Union[Value, "Query", List[Value], List["Query"]]],
     Dict[AndOr, List[Dict[str, Union[Value, "Query", List[Value], List["Query"]]]]],
 ]
 
 
 class CheapModel(BaseModel):
+    """Cheap model that allow cheap serialization and deserialization."""
+
+    @classmethod
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        cls.__doc__ = cls.schema_json()
+        cls.__repr__ = cls.schema_json
+        cls.__str__ = cls.schema_json
+
     def json(self, *args, **kwargs) -> str:
+        """Serialize the model to JSON."""
         return dumps(self.dict())
 
     @classmethod
     def parse(cls, s: str) -> CheapModel:
+        """Deserialize the model from JSON."""
         return cls(**loads(s))
 
 
 class QueryBuilder:
+    """Query builder for Pinecone Query API with MongoDB-like syntax."""
+
     def __init__(self, field: str = None, query: Query = None):  # type: ignore
         self.field = field
         self.query = query if query else {}
 
     def __repr__(self) -> str:
         return f"{self.query}"
 
@@ -60,11 +72,13 @@
     def __gt__(self, value: Value) -> QueryBuilder:
         return QueryBuilder(query={self.field: {"$gt": value}})
 
     def __ge__(self, value: Value) -> QueryBuilder:
         return QueryBuilder(query={self.field: {"$gte": value}})
 
     def in_(self, values: List[Value]) -> QueryBuilder:
+        """MongoDB-like syntax for $in operator."""
         return QueryBuilder(query={self.field: {"$in": values}})
 
     def nin_(self, values: List[Value]) -> QueryBuilder:
+        """MongoDB-like syntax for $nin operator."""
         return QueryBuilder(query={self.field: {"$nin": values}})
```


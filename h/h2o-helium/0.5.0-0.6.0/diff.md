# Comparing `tmp/h2o_helium-0.5.0-py3-none-any.whl.zip` & `tmp/h2o_helium-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4762 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    13011 b- defN 23-Jul-07 10:05 h2o_helium/__init__.py
--rw-rw-r--  2.0 unx     2014 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      390 b- defN 23-Jul-07 10:05 h2o_helium-0.5.0.dist-info/RECORD
-5 files, 15518 bytes uncompressed, 4036 bytes compressed:  74.0%
+Zip file size: 5180 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    15156 b- defN 23-Aug-08 01:27 h2o_helium/__init__.py
+-rw-rw-r--  2.0 unx     2012 b- defN 23-Aug-08 01:28 h2o_helium-0.6.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-08 01:28 h2o_helium-0.6.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Aug-08 01:28 h2o_helium-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      390 b- defN 23-Aug-08 01:28 h2o_helium-0.6.0.dist-info/RECORD
+5 files, 17661 bytes uncompressed, 4454 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: h2o_helium/__init__.py
 Comment: 
 
-Filename: h2o_helium-0.5.0.dist-info/METADATA
+Filename: h2o_helium-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: h2o_helium-0.5.0.dist-info/WHEEL
+Filename: h2o_helium-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_helium-0.5.0.dist-info/top_level.txt
+Filename: h2o_helium-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_helium-0.5.0.dist-info/RECORD
+Filename: h2o_helium-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_helium/__init__.py

```diff
@@ -1,32 +1,37 @@
 import json
 import time
 import uuid
+from dataclasses import dataclass, asdict
 from datetime import datetime
 from enum import Enum
 from typing import Iterable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 from pydantic import BaseModel
 from websockets.sync.client import connect as ws_connect, ClientConnection
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 
 class Status(str, Enum):
     Unknown = 'unknown'
     Scheduled = 'scheduled'
     Queued = 'queued'
     Running = 'running'
     Completed = 'completed'
     Failed = 'failed'
     Canceled = 'canceled'
 
 
+class Answer(BaseModel):
+    content: str
+
+
 class ChatMessage(BaseModel):
     id: str
     content: str
     reply_to: Optional[str]
     created_at: datetime
 
 
@@ -56,15 +61,15 @@
 
 
 class Chunk(BaseModel):
     text: str
 
 
 class Chunks(BaseModel):
-    chunks: List[Chunk]
+    result: List[Chunk]
 
 
 class Collection(BaseModel):
     id: str
     name: str
     description: str
     document_count: int
@@ -152,14 +157,61 @@
 class Result(BaseModel):
     status: Status
 
     class Config:
         use_enum_values = True
 
 
+class SearchResult(BaseModel):
+    id: str
+    topic: str
+    name: str
+    text: str
+    size: int
+    score: float
+
+
+class SearchResults(BaseModel):
+    result: List[SearchResult]
+
+
+@dataclass
+class ChatRequest:
+    t: str  # cq
+    mode: str  # l=lexical, s=semantic, h=hybrid
+    session_id: str
+    correlation_id: str
+    body: str
+
+
+@dataclass
+class ChatAcknowledgement:
+    t: str  # cx
+    session_id: str
+    correlation_id: str
+    message_id: str
+
+
+@dataclass
+class ChatResponse:
+    t: str  # ca
+    session_id: str
+    message_id: str
+    reply_to_id: str
+    body: str
+
+
+@dataclass
+class ChatError:
+    t: str  # ce
+    session_id: str
+    reply_to_id: str
+    body: str
+
+
 class SessionError(Exception):
     pass
 
 
 class Session:
     def __init__(self, address: str, api_key: str, chat_session_id: str):
         url = urlparse(address)
@@ -173,55 +225,56 @@
     def connect(self):
         self._connection = ws_connect(self._address, additional_headers={
             'Authorization': f'Bearer {self._api_key}'
         })
 
     def query(self, message: str, timeout: Optional[float] = None) -> ChatMessage:
         correlation_id = str(uuid.uuid4())
-        req = dict(
-            s=self._chat_session_id,
-            x=correlation_id,
-            b=message,
-        )
+        req = asdict(ChatRequest(
+            t='cq',
+            mode='s',
+            session_id=self._chat_session_id,
+            correlation_id=correlation_id,
+            body=message,
+        ))
         self._connection.send(marshal(req))
 
         deadline = time.time() + timeout
         request_id: Optional[str] = None
         response = ''
         while True:
             res = self._connection.recv(deadline - time.time())
 
             data = unmarshal(res)
             t = data['t']
-            chat_session_id = data['s']
-            reply_to_id = data['x']
-            message_id = data.get('a', None)
-            body = data['b']
-
-            if chat_session_id != self._chat_session_id:
-                continue
-
-            if t == 'a':  # ack
-                if reply_to_id == correlation_id:
-                    request_id = body
-            elif t == 'p':
-                if reply_to_id == request_id:
-                    response += body
-            elif t == 'f':
-                if reply_to_id == request_id:
-                    response += body
+
+            if t == 'cx':  # ack
+                res = ChatAcknowledgement(**data)
+                if res.session_id != self._chat_session_id:
+                    continue
+                if res.correlation_id == correlation_id:
+                    request_id = res.message_id
+            elif t == 'ca':  # response
+                res = ChatResponse(**data)
+                if res.session_id != self._chat_session_id:
+                    continue
+                if res.reply_to_id == request_id:
+                    response += res.body
                     return ChatMessage(
-                        id=message_id,
+                        id=res.message_id,
                         content=response,
-                        reply_to=reply_to_id,
+                        reply_to=res.reply_to_id,
                         created_at=datetime.now(),
                     )
-            elif t == 'e':
-                if reply_to_id == request_id:
-                    raise SessionError(f'Remote error: {body}')
+            elif t == 'ce':
+                res = ChatError(**data)
+                if res.session_id != self._chat_session_id:
+                    continue
+                if res.reply_to_id == request_id:
+                    raise SessionError(f'Remote error: {res.body}')
             else:
                 raise SessionError(f'Invalid chat response type {t}.')
 
     def disconnect(self):
         self._connection.close()
 
     def __enter__(self):
@@ -265,26 +318,36 @@
 
     def _db(self, method: str, *args):
         return self._post('/rpc/db', marshal([method, *args]))
 
     def _job(self, method: str, **kwargs):
         return self._post('/rpc/job', marshal([method, kwargs]))
 
-    def _vex(self, method: str, **kwargs):
-        return self._post('/rpc/vex', marshal(dict(method=method, params=kwargs)))
+    def _lang(self, method: str, **kwargs):
+        res = self._post('/rpc/lang', marshal(dict(method=method, params=kwargs)))
+        err = res.get('error')
+        if err:
+            raise Exception(err)
+        return res['result']
+
+    def _vex(self, method: str, collection_id: str, **kwargs):
+        return self._post('/rpc/vex', marshal(dict(method=method, collection_id=collection_id, params=kwargs)))
 
     def _wait(self, d):
         job_id = _to_id(d)
         while True:
             time.sleep(1)
             job = self.get_job(job_id)
             if job.completed or job.canceled:
                 break
         return job
 
+    def answer_question(self, question: str, context: str):
+        return Answer(**self._lang('answer_question_using_context', question=question, context=context))
+
     def cancel_job(self, job_id: str) -> Result:
         return Result(**self._job('.Cancel', job_id=job_id))
 
     def count_chat_sessions(self) -> int:
         return ChatSessionCount(**self._db('count_chat_sessions')).chat_session_count
 
     def count_chat_sessions_for_collection(self, collection_id: str) -> int:
@@ -317,18 +380,20 @@
     def delete_documents(self, document_ids: Iterable[str]):
         return self._wait(self._job('crawl.DeleteDocumentsJob', document_ids=document_ids))
 
     def delete_documents_from_collection(self, collection_id: str, document_ids: Iterable[str]):
         return self._wait(self._job('crawl.DeleteDocumentsFromCollectionJob', collection_id=collection_id,
                                     document_ids=document_ids))
 
+    def encode_for_retrieval(self, chunks: List[str]) -> List[List[float]]:
+        return self._lang('encode_for_retrieval', chunks=chunks)
+
     def get_chunks(self, collection_id: str, chunk_ids: Iterable[int]) -> List[Chunk]:
-        res = self._vex('get_chunks', collection_id=collection_id, chunk_ids=list(chunk_ids))
-        chunks = Chunks(**res).chunks
-        return chunks
+        res = self._vex('get_chunks', collection_id, chunk_ids=list(chunk_ids))
+        return Chunks(**res).result
 
     def get_collection(self, collection_id: str) -> Collection:
         res = self._db('get_collection', collection_id)
         if len(res) == 0:
             raise KeyError(f'Collection {collection_id} not found')
         return Collection(**res[0])
 
@@ -390,14 +455,26 @@
 
     def list_recent_collections(self, offset: int, limit: int) -> List[CollectionInfo]:
         return [CollectionInfo(**d) for d in self._db('list_recent_collections', offset, limit)]
 
     def list_recent_documents(self, offset: int, limit: int) -> List[DocumentInfo]:
         return [DocumentInfo(**d) for d in self._db('list_recent_documents', offset, limit)]
 
+    def match_chunks(
+            self, collection_id: str, vectors: List[List[float]], topics: List[str], offset: int, limit: int
+    ) -> List[SearchResult]:
+        res = self._vex('match_chunks', collection_id, vectors=vectors, topics=topics, offset=offset, limit=limit)
+        return SearchResults(**res).result
+
+    def search_chunks(
+            self, collection_id: str, query: str, topics: List[str], offset: int, limit: int
+    ) -> List[SearchResult]:
+        res = self._vex('search_chunks', collection_id, query=query, topics=topics, offset=offset, limit=limit)
+        return SearchResults(**res).result
+
     def upload(self, file_name: str, file: any) -> str:
         res = requests.post(
             f'{self._address}/rpc/fs',
             headers={
                 'Authorization': self._auth_header,
             },
             files=dict(file=(file_name, file)),
```

## Comparing `h2o_helium-0.5.0.dist-info/METADATA` & `h2o_helium-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: h2o-helium
-Version: 0.5.0
+Version: 0.6.0
 Summary: Client library for H2O Helium
 Author-email: Prithvi Prabhu <prithvi.prabhu@gmail.com>
 Project-URL: Source, https://github.com/h2oai/helium
 Project-URL: Issues, https://github.com/h2oai/helium/issues
 Project-URL: Documentation, https://github.com/h2oai/helium/wiki
 Keywords: information-retrieval,LLM,large-language-models,question-answering,search,semantic-search,analytical-search,lexical-search,document-search,natural-language-querying
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: pydantic[dotenv] (~=1.10)
+Requires-Dist: pydantic[dotenv] ~=1.10
 Requires-Dist: requests
 Requires-Dist: websockets
 
 # H2O Helium Python Client
 
 ## Install
```


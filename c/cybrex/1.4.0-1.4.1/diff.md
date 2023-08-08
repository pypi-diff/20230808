# Comparing `tmp/cybrex-1.4.0.tar.gz` & `tmp/cybrex-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.4.0.tar", last modified: Tue Aug  8 10:59:15 2023, max compression
+gzip compressed data, was "cybrex-1.4.1.tar", last modified: Tue Aug  8 14:18:39 2023, max compression
```

## Comparing `cybrex-1.4.0.tar` & `cybrex-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.299872 cybrex-1.4.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 10:59:15.299072 cybrex-1.4.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.0/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.281437 cybrex-1.4.0/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.0/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.289132 cybrex-1.4.0/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.0/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.0/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5477 2023-08-08 10:14:20.000000 cybrex-1.4.0/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    12027 2023-08-08 10:57:13.000000 cybrex-1.4.0/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.291187 cybrex-1.4.0/cybrex/data_source/
--rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.0/cybrex/data_source/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     1261 2023-08-08 10:58:41.000000 cybrex-1.4.0/cybrex/data_source/geck_data_source.py
--rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.0/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.0/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.292421 cybrex-1.4.0/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9846 2023-08-07 16:35:58.000000 cybrex-1.4.0/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.297022 cybrex-1.4.0/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.0/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2626 2023-08-08 08:47:20.000000 cybrex-1.4.0/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.287017 cybrex-1.4.0/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 10:58:45.000000 cybrex-1.4.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 08:25:43.000000 cybrex-1.4.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 10:59:15.300186 cybrex-1.4.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.835056 cybrex-1.4.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:18:39.834105 cybrex-1.4.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.1/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.811567 cybrex-1.4.1/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.1/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.820932 cybrex-1.4.1/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.1/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.1/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5475 2023-08-08 12:09:00.000000 cybrex-1.4.1/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12223 2023-08-08 13:44:49.000000 cybrex-1.4.1/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.824186 cybrex-1.4.1/cybrex/data_source/
+-rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.1/cybrex/data_source/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1293 2023-08-08 13:14:00.000000 cybrex-1.4.1/cybrex/data_source/geck_data_source.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.1/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.1/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.827238 cybrex-1.4.1/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9847 2023-08-08 11:30:06.000000 cybrex-1.4.1/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.831733 cybrex-1.4.1/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.1/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.1/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2782 2023-08-08 13:45:08.000000 cybrex-1.4.1/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 14:18:39.818466 cybrex-1.4.1/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 14:18:39.000000 cybrex-1.4.1/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 14:17:59.000000 cybrex-1.4.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 14:17:56.000000 cybrex-1.4.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 14:18:39.835447 cybrex-1.4.1/setup.cfg
```

### Comparing `cybrex-1.4.0/PKG-INFO` & `cybrex-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.0
+Version: 1.4.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.0/README.md` & `cybrex-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.0/cybrex/chains/map_reduce.py` & `cybrex-1.4.1/cybrex/chains/map_reduce.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.0/cybrex/cli.py` & `cybrex-1.4.1/cybrex/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     async def add_all_documents(self):
         async with self.cybrex as cybrex:
             async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
                 document = json.loads(document)
                 await self.cybrex.upsert_documents([document])
 
-    async def export_chunks(self, query: str, output_path: str, n_documents: int = 100):
+    async def export_chunks(self, query: str, output_path: str, n_documents: int = 10):
         """
         Store STC text chunks in ZIP archive
 
         :param query: query to STC
         :param output_path: where to store result
         :param n_documents: the number of chunks to extract
         """
@@ -44,15 +44,15 @@
         """
         Import binary file with embeddings
 
         :param input_path:
         """
         await self.cybrex.import_chunks(input_path=input_path)
 
-    async def chat_doc(self, document_query: str, query: str, n_chunks: int = 4):
+    async def chat_doc(self, document_query: str, query: str, n_chunks: int = 5):
         """
         Ask a question about content of document identified by DOI.
 
         :param document_query: query that returns unique document
         :param query: Text query to the document
         :param n_chunks: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
@@ -62,15 +62,15 @@
             print(f"{colored('Q', 'green')}: {query}")
             response = await cybrex.chat_document(document_query, query, n_chunks)
             print(f"{colored('A', 'green')}: {response}")
 
     async def chat_sci(
         self,
         query: str,
-        n_chunks: int = 4,
+        n_chunks: int = 5,
         n_documents: int = 10,
     ):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: text query to the document
         :param n_chunks: the number of chunks to extract from Chroma
@@ -100,15 +100,15 @@
         :param document_query: query that returns unique document
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Document', 'green')}: {document_query}")
             response = await cybrex.summarize_document(document_query)
             print(f"{colored('Summarization', 'green')}: {response}")
 
-    async def semantic_search(self, query: str, n_chunks: int = 10, n_documents: int = 30):
+    async def semantic_search(self, query: str, n_chunks: int = 5, n_documents: int = 10):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: query to STC
         :param n_chunks: number of pieces to return
         :param n_documents: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
```

### Comparing `cybrex-1.4.0/cybrex/cybrex_ai.py` & `cybrex-1.4.1/cybrex/cybrex_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import numpy as np
 import pypdf
 import yaml
 from aiokit import AioThing
 from izihawa_configurator import Configurator
 from izihawa_utils.exceptions import BaseError
 from izihawa_utils.file import mkdir_p
-from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
 from .chains.map_reduce import (
     QAChain,
     SummarizeChain,
 )
 from .data_source.base import SourceDocument
@@ -78,44 +77,46 @@
         self.model = CybrexModel(config['model'])
         self.document_chunker = DocumentChunker(text_splitter=self.model.text_splitter)
 
         self.geck = geck
         if not self.geck:
             self.geck = StcGeck(
                 ipfs_http_base_url=config['ipfs']['http']['base_url'],
-                grpc_api_endpoint=config['summa']['endpoint']
+                grpc_api_endpoint=config['summa']['endpoint'],
+                timeout=600,
             )
             self.starts.append(self.geck)
 
         self.data_source = GeckDataSource(self.geck)
         self.vector_storage = ChromaVectorStorage(
             path=os.path.join(self.home_path, 'chroma'),
             collection_name=self.model.get_embeddings_id(),
+            embedding_function=self.model.embed_documents,
         )
 
     async def resolve_document_content(self, document: SourceDocument) -> Optional[str]:
         document = document.document
         if 'content' in document:
             return document['content']
         elif 'links' in document:
             primary_link = document['links'][0]
             file_content = await self.geck.download(document['links'][0]['cid'])
-            match primary_link['type']:
+            match primary_link['extension']:
                 case 'pdf':
                     pdf_reader = pypdf.PdfReader(io.BytesIO(file_content))
                     return '\n'.join(page.extract_text() for page in pdf_reader.pages)
                 case _:
                     raise RuntimeError("Unsupported extension")
 
     async def generate_chunks_from_document(self, document: SourceDocument) -> List[dict]:
-        document['content'] = await self.resolve_document_content(document)
+        document.document['content'] = await self.resolve_document_content(document)
         return self.document_chunker.to_chunks(document)
 
     async def _get_missing_chunks(self, documents: List[SourceDocument], skip_downloading_pdf: bool = True) -> List[dict]:
-        chunks = []
+        all_chunks = []
         for document in documents:
             chunks = await asyncio.get_running_loop().run_in_executor(
                 None,
                 lambda: self.vector_storage.get_by_field_value('id', document.document_id)
             )
             if chunks:
                 logging.getLogger('statbox').info({
@@ -133,16 +134,16 @@
                 continue
             logging.getLogger('statbox').info({
                 'action': 'retrieve_content',
                 'mode': 'cybrex',
                 'id': document.document_id,
             })
             document_chunks = await self.generate_chunks_from_document(document)
-            chunks.extend(document_chunks)
-        return chunks
+            all_chunks.extend(document_chunks)
+        return all_chunks
 
     async def upsert_documents(self, documents: List[SourceDocument], skip_downloading_pdf: bool = True):
         if not documents:
             return
         chunks = await self._get_missing_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if chunks:
             logging.getLogger('statbox').info({
@@ -268,43 +269,45 @@
         })
         topic = ' '.join(map(lambda x: x[0], filter(lambda x: x[1] > 0.5, keywords)))
         documents = await self.data_source.query_documents(query=topic, limit=n_documents)
         return documents
 
     async def get_summa_documents_from_documents(self, documents):
         ids = set([document['metadata']['id'] for document in documents])
-        _summa_documents = await asyncio.gather(*[
-            self.geck.get_summa_client().search_documents([{
-                'index_alias': 'nexus_science',
-                'query': {'term': {'field': id_.split(':', 1)[0], 'value': id_.split(':', 1)[1]}},
-                'collectors': [{'top_docs': {'limit': 100}}],
-            }])
-            for id_ in ids
-        ])
+        search_requests = []
+        for id_ in ids:
+            index_alias, field, value = id_.split(':', 2)
+            search_request = {
+                'index_alias': index_alias,
+                'query': {'term': {'field': field, 'value': value}},
+                'collectors': [{'top_docs': {'limit': 1}}],
+            }
+            search_requests.append(self.geck.get_summa_client().search_documents([search_request]))
+        _summa_documents = await asyncio.gather(*search_requests)
         summa_documents = []
         for summa_document in _summa_documents:
             summa_documents.append(summa_document[0])
         return summa_documents
 
     async def semantic_search(self, query: str, n_chunks: int = 10, n_documents: int = 30):
         documents = await self.keywords_search(query, n_documents)
         await self.upsert_documents(documents)
         return await self._query(query, n_chunks)
 
     async def chat_document(self, document_query: str, query: str, n_chunks: int):
-        document_id = await self.upsert_document_by_query(document_query, skip_downloading_pdf=False)
+        document_id = await self.upsert_document_by_query(str(document_query), skip_downloading_pdf=False)
         chunks = await self._query(query=query, n_chunks=n_chunks, where={'id': document_id})
 
         chain = QAChain(query=query, llm=self.model.llm)
         answer = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: chain.process(chunks),
         )
 
-        return answer
+        return answer.strip()
 
     async def summarize_document(self, document_query):
         document_id = await self.upsert_document_by_query(document_query)
         chunks = self.vector_storage.get_by_field_value('id', document_id)
         chain = SummarizeChain(llm=self.model.llm)
         result = await asyncio.get_running_loop().run_in_executor(
             None,
```

### Comparing `cybrex-1.4.0/cybrex/data_source/geck_data_source.py` & `cybrex-1.4.1/cybrex/data_source/geck_data_source.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 from .base import BaseDataSource, SourceDocument
 
 
 class GeckDataSource(BaseDataSource):
     def __init__(self, geck: StcGeck):
         self.geck = geck
 
-    async def query_documents(self, query: str, limit: int = 5, sources: Optional[List[str]] = None) -> List[SourceDocument]:
+    async def query_documents(
+        self,
+        query: str,
+        limit: int = 5,
+        sources: Optional[List[str]] = None
+    ) -> List[SourceDocument]:
         queries = self.geck.get_query_processor().process(query, limit=limit, index_aliases=sources)
         response = await self.geck.get_summa_client().search(queries)
         source_documents = []
         for scored_document in response.collector_outputs[0].documents.scored_documents:
             document = orjson.loads(scored_document.document)
             match scored_document.index_alias:
                 case 'nexus_science':
                     document_id = f'nexus_science:doi:{document["doi"]}'
                 case 'nexus_free':
-                    document_id = f'nexus_free:metadata.isbns:{document["id"]["isbns"][0]}'
+                    document_id = f'nexus_free:id.isbns:{document["id"]["isbns"][0]}'
                 case _:
                     raise RuntimeError("Unsupported table")
             source_documents.append(SourceDocument(
                 document=document,
                 document_id=document_id,
             ))
         return source_documents
```

### Comparing `cybrex-1.4.0/cybrex/document_chunker.py` & `cybrex-1.4.1/cybrex/document_chunker.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.0/cybrex/models.py` & `cybrex-1.4.1/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.0/cybrex/prompts/base.py` & `cybrex-1.4.1/cybrex/prompts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
 ASSISTANT:'''.format(summary=self.generate_summary(chunks))
 
     def generate_summary(self, chunks: List[dict]):
         chunk_summaries = []
         chunk_summaries_grouped = OrderedDict()
         for chunk in chunks:
-            id_ = chunk.get("metadata", {}).get("id")
+            id_ = chunk["metadata"]["id"]
             if id_ not in chunk_summaries_grouped:
                 chunk_summaries_grouped[id_] = []
             chunk_summaries_grouped[id_].append(chunk['text'])
         for id_, texts in chunk_summaries_grouped.items():
             texts = ' <..> '.join(texts)
             if id_:
-                field, value = id_.split(':', 1)
+                index_alias, field, value = id_.split(':', 2)
                 chunk_summaries.append(f'{field.upper()}: {value}\nCONTENT: {texts}')
             else:
                 chunk_summaries.append(f'CONTENT: {texts}')
         return '\n'.join(chunk_summaries)
 
 
 class Llama27bPrompter(BasePrompter):
```

### Comparing `cybrex-1.4.0/cybrex/vector_storage/chroma.py` & `cybrex-1.4.1/cybrex/vector_storage/chroma.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 import chromadb
 
 from .base import BaseVectorStorage
 
 
 class ChromaVectorStorage(BaseVectorStorage):
-    def __init__(self, path, collection_name):
+    def __init__(self, path, collection_name, embedding_function=None):
         self.db = chromadb.PersistentClient(path=path)
         self.collection_name = collection_name
-
-        self.collection = self.db.get_or_create_collection(name=self.collection_name)
+        self.collection = self.db.get_or_create_collection(
+            name=self.collection_name,
+            embedding_function=embedding_function,
+        )
 
     def _unpack(self, chroma_response, i: int = 0) -> List[dict]:
         chunks = []
         documents = chroma_response.get('documents', [])
         if documents and isinstance(documents[0], list):
             documents = documents[i]
 
@@ -39,15 +41,16 @@
         return chunks
 
     def _pack(self, chunks):
         embeddings = []
         metadatas = []
         texts = []
         for chunk in chunks:
-            embeddings.append(chunk['embedding'])
+            if 'embedding' in chunk:
+                embeddings.append(chunk['embedding'])
             if 'metadata' in chunk:
                 metadatas.append(chunk['metadata'])
             if 'text' in chunk:
                 texts.append(chunk['text'])
         return embeddings, metadatas, texts
 
     def get_by_field_value(self, field, value) -> List[dict]:
@@ -65,12 +68,12 @@
         for i in range(len(responses["documents"])):
             unpacked_responses.append(self._unpack(responses, i=i))
         return unpacked_responses
 
     def upsert(self, chunks: List[dict]):
         embeddings, metadatas, texts = self._pack(chunks)
         return self.collection.upsert(
-            embeddings=embeddings,
+            embeddings=embeddings or None,
             documents=texts or None,
             metadatas=metadatas or None,
-            ids=[str(uuid.uuid1()) for _ in range(len(embeddings))]
+            ids=[str(uuid.uuid1()) for _ in range(len(embeddings or texts))]
         )
```

### Comparing `cybrex-1.4.0/cybrex.egg-info/PKG-INFO` & `cybrex-1.4.1/cybrex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.4.0
+Version: 1.4.1
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.4.0/cybrex.egg-info/SOURCES.txt` & `cybrex-1.4.1/cybrex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybrex-1.4.0/pyproject.toml` & `cybrex-1.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.4.0"
+version = "1.4.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```


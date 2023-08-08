# Comparing `tmp/cybrex-1.3.3.tar.gz` & `tmp/cybrex-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.3.3.tar", last modified: Mon Aug  7 15:11:50 2023, max compression
+gzip compressed data, was "cybrex-1.4.0.tar", last modified: Tue Aug  8 10:59:15 2023, max compression
```

## Comparing `cybrex-1.3.3.tar` & `cybrex-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.086683 cybrex-1.3.3/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.3.3/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 15:11:50.086145 cybrex-1.3.3/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.3.3/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.074495 cybrex-1.3.3/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.3.3/cybrex/__init__.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.081124 cybrex-1.3.3/cybrex/chains/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.3/cybrex/chains/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.3.3/cybrex/chains/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.3.3/cybrex/chains/map_reduce.py
--rw-r--r--   0 pasha      (501) staff       (20)     5564 2023-08-07 13:54:06.000000 cybrex-1.3.3/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11775 2023-08-07 15:10:06.000000 cybrex-1.3.3/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)     1676 2023-08-05 19:44:06.000000 cybrex-1.3.3/cybrex/document_chunker.py
--rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.3.3/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.082242 cybrex-1.3.3/cybrex/prompts/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.3/cybrex/prompts/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     9984 2023-08-07 14:45:37.000000 cybrex-1.3.3/cybrex/prompts/base.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.084857 cybrex-1.3.3/cybrex/vector_storage/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.3.3/cybrex/vector_storage/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.3.3/cybrex/vector_storage/base.py
--rw-r--r--   0 pasha      (501) staff       (20)     2626 2023-08-07 15:07:49.000000 cybrex-1.3.3/cybrex/vector_storage/chroma.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-07 15:11:50.079251 cybrex-1.3.3/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      554 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-07 15:11:50.000000 cybrex-1.3.3/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-07 15:11:26.000000 cybrex-1.3.3/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      270 2023-08-02 11:17:07.000000 cybrex-1.3.3/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-07 15:11:50.086881 cybrex-1.3.3/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.299872 cybrex-1.4.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.4.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 10:59:15.299072 cybrex-1.4.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     4539 2023-08-08 10:28:15.000000 cybrex-1.4.0/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.281437 cybrex-1.4.0/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:27.000000 cybrex-1.4.0/cybrex/__init__.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.289132 cybrex-1.4.0/cybrex/chains/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/chains/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:17:49.000000 cybrex-1.4.0/cybrex/chains/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2389 2023-08-07 14:15:31.000000 cybrex-1.4.0/cybrex/chains/map_reduce.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5477 2023-08-08 10:14:20.000000 cybrex-1.4.0/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    12027 2023-08-08 10:57:13.000000 cybrex-1.4.0/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.291187 cybrex-1.4.0/cybrex/data_source/
+-rw-r--r--   0 pasha      (501) staff       (20)      329 2023-08-08 08:33:51.000000 cybrex-1.4.0/cybrex/data_source/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1261 2023-08-08 10:58:41.000000 cybrex-1.4.0/cybrex/data_source/geck_data_source.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1750 2023-08-08 10:22:36.000000 cybrex-1.4.0/cybrex/document_chunker.py
+-rw-r--r--   0 pasha      (501) staff       (20)     4843 2023-08-07 14:38:25.000000 cybrex-1.4.0/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.292421 cybrex-1.4.0/cybrex/prompts/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/prompts/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     9846 2023-08-07 16:35:58.000000 cybrex-1.4.0/cybrex/prompts/base.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.297022 cybrex-1.4.0/cybrex/vector_storage/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-08-07 10:20:28.000000 cybrex-1.4.0/cybrex/vector_storage/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      213 2023-08-07 15:07:49.000000 cybrex-1.4.0/cybrex/vector_storage/base.py
+-rw-r--r--   0 pasha      (501) staff       (20)     2626 2023-08-08 08:47:20.000000 cybrex-1.4.0/cybrex/vector_storage/chroma.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 10:59:15.287017 cybrex-1.4.0/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     4815 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      620 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-08 10:59:15.000000 cybrex-1.4.0/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-08 10:58:45.000000 cybrex-1.4.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      277 2023-08-08 08:25:43.000000 cybrex-1.4.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 10:59:15.300186 cybrex-1.4.0/setup.cfg
```

### Comparing `cybrex-1.3.3/cybrex/chains/map_reduce.py` & `cybrex-1.4.0/cybrex/chains/map_reduce.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.3/cybrex/cli.py` & `cybrex-1.4.0/cybrex/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import fire
 from termcolor import colored
 
 from .cybrex_ai import CybrexAI
 
 
 def create_snippet(document):
-    return document['metadata']['doi'] + ': ' + document['text']
+    return document['metadata']['id'] + ': ' + document['text']
 
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
     async def add_all_documents(self):
         async with self.cybrex as cybrex:
             async for document in cybrex.geck.get_summa_client().documents('nexus_science'):
                 document = json.loads(document)
-                await self.cybrex.add_full_documents([document])
+                await self.cybrex.upsert_documents([document])
 
     async def export_chunks(self, query: str, output_path: str, n_documents: int = 100):
         """
         Store STC text chunks in ZIP archive
 
         :param query: query to STC
         :param output_path: where to store result
@@ -44,68 +44,68 @@
         """
         Import binary file with embeddings
 
         :param input_path:
         """
         await self.cybrex.import_chunks(input_path=input_path)
 
-    async def chat_doc(self, field: str, value: str, question: str, n_chunks: int = 4):
+    async def chat_doc(self, document_query: str, query: str, n_chunks: int = 4):
         """
         Ask a question about content of document identified by DOI.
 
-        :param field: name of the field in document used for selection
-        :param value: value of the field in document used for selection
-        :param question: Text question to the document
+        :param document_query: query that returns unique document
+        :param query: Text query to the document
         :param n_chunks: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
-            print(f"{colored('Document', 'green')}: {field}:{value}")
-            print(f"{colored('Q', 'green')}: {question}")
-            response = await cybrex.chat_document(field, value, question, n_chunks)
+            print(f"{colored('Document', 'green')}: {document_query}")
+            print(f"{colored('Q', 'green')}: {query}")
+            response = await cybrex.chat_document(document_query, query, n_chunks)
             print(f"{colored('A', 'green')}: {response}")
 
     async def chat_sci(
         self,
         query: str,
         n_chunks: int = 4,
         n_documents: int = 10,
     ):
         """
         Ask a question about content of document identified by DOI.
 
-        :param query: Text question to the document
+        :param query: text query to the document
         :param n_chunks: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         :param n_documents: the number of chunks to extract from Chroma
             more means more tokens to use and more precision in answer
         """
         async with self.cybrex as cybrex:
             print(f"{colored('Q', 'green')}: {query}")
             answer, documents, summa_documents = await cybrex.chat_science(
                 query=query,
                 n_chunks=n_chunks,
                 n_documents=n_documents,
             )
             answer = re.sub(r'\(DOI: ([^)]+)\)', r'(https://doi.org/\g<1>)', answer)
-            summa_documents = [f'{summa_document["doi"]}: {summa_document["title"]}' for summa_document in summa_documents]
+            summa_documents = [
+                f'{summa_document.get("doi") or summa_document.get("metadata", {}).get("isbns")}: {summa_document["title"]}'
+                for summa_document in summa_documents]
             sources = '\n'.join(summa_documents)
             print(f"{colored('A', 'green')}: {answer}")
             print(f"{colored('References', 'green')}:\n{textwrap.indent(sources, ' - ')}")
 
-    async def sum_doc(self, field: str, value: str):
+    async def sum_doc(self, document_query: str):
         """
         Summarization of the document
 
-        :param field: name of the field in document used for selection
-        :param value: value of the field in document used for selection
+        :param document_query: query that returns unique document
         """
         async with self.cybrex as cybrex:
-            print(f"{colored('Document', 'green')}: {field}:{value}")
-            response = await cybrex.summarize_document(field, value)
+            print(f"{colored('Document', 'green')}: {document_query}")
+            response = await cybrex.summarize_document(document_query)
             print(f"{colored('Summarization', 'green')}: {response}")
 
     async def semantic_search(self, query: str, n_chunks: int = 10, n_documents: int = 30):
         """
         Ask a question about content of document identified by DOI.
 
         :param query: query to STC
```

### Comparing `cybrex-1.3.3/cybrex/cybrex_ai.py` & `cybrex-1.4.0/cybrex/cybrex_ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from stc_geck.advices import get_documents_on_topic
 from stc_geck.client import StcGeck
 
 from .chains.map_reduce import (
     QAChain,
     SummarizeChain,
 )
+from .data_source.base import SourceDocument
+from .data_source.geck_data_source import GeckDataSource
 from .document_chunker import DocumentChunker
 from .models import CybrexModel
 from .vector_storage.chroma import ChromaVectorStorage
 
 
 class DocumentNotFoundError(BaseError):
     pass
@@ -80,68 +82,69 @@
         if not self.geck:
             self.geck = StcGeck(
                 ipfs_http_base_url=config['ipfs']['http']['base_url'],
                 grpc_api_endpoint=config['summa']['endpoint']
             )
             self.starts.append(self.geck)
 
+        self.data_source = GeckDataSource(self.geck)
         self.vector_storage = ChromaVectorStorage(
             path=os.path.join(self.home_path, 'chroma'),
             collection_name=self.model.get_embeddings_id(),
         )
 
-    async def resolve_document_content(self, document: dict) -> Optional[str]:
+    async def resolve_document_content(self, document: SourceDocument) -> Optional[str]:
+        document = document.document
         if 'content' in document:
             return document['content']
         elif 'links' in document:
             primary_link = document['links'][0]
             file_content = await self.geck.download(document['links'][0]['cid'])
             match primary_link['type']:
                 case 'pdf':
                     pdf_reader = pypdf.PdfReader(io.BytesIO(file_content))
                     return '\n'.join(page.extract_text() for page in pdf_reader.pages)
                 case _:
                     raise RuntimeError("Unsupported extension")
 
-    async def generate_chunks_from_document(self, document: dict) -> List[dict]:
+    async def generate_chunks_from_document(self, document: SourceDocument) -> List[dict]:
         document['content'] = await self.resolve_document_content(document)
         return self.document_chunker.to_chunks(document)
 
-    async def _get_missing_chunks(self, documents: List[dict], skip_downloading_pdf: bool = True) -> List[dict]:
+    async def _get_missing_chunks(self, documents: List[SourceDocument], skip_downloading_pdf: bool = True) -> List[dict]:
         chunks = []
         for document in documents:
-            doi = document['doi']
             chunks = await asyncio.get_running_loop().run_in_executor(
                 None,
-                lambda: self.vector_storage.get_by_field_value('doi', doi)
+                lambda: self.vector_storage.get_by_field_value('id', document.document_id)
             )
             if chunks:
                 logging.getLogger('statbox').info({
                     'action': 'already_stored',
                     'mode': 'cybrex',
-                    'doi': doi,
+                    'id': document.document_id,
                 })
                 continue
             if skip_downloading_pdf and 'content' not in document:
                 logging.getLogger('statbox').info({
                     'action': 'no_content',
                     'mode': 'cybrex',
-                    'doi': doi,
+                    'id': document.document_id,
                 })
                 continue
             logging.getLogger('statbox').info({
                 'action': 'retrieve_content',
                 'mode': 'cybrex',
-                'doi': doi,
+                'id': document.document_id,
             })
             document_chunks = await self.generate_chunks_from_document(document)
             chunks.extend(document_chunks)
         return chunks
 
-    async def add_full_documents(self, documents: List[dict], skip_downloading_pdf: bool = True):
+    async def upsert_documents(self, documents: List[SourceDocument], skip_downloading_pdf: bool = True):
         if not documents:
             return
         chunks = await self._get_missing_chunks(documents, skip_downloading_pdf=skip_downloading_pdf)
         if chunks:
             logging.getLogger('statbox').info({
                 'action': 'add_full_documents',
                 'mode': 'cybrex',
@@ -153,27 +156,20 @@
             )
             logging.getLogger('statbox').info({
                 'action': 'added_full_documents',
                 'mode': 'cybrex',
                 'n': len(chunks),
             })
 
-    async def add_full_document_by_field_value(self, field, value) -> List[dict]:
-        documents = await self.geck.get_summa_client().search_documents([{
-            'index_alias': 'nexus_science',
-            'collectors': [{'top_docs': {'limit': 1}}],
-            'query': {'term': {'field': field, 'value': value}}
-        }])
+    async def upsert_document_by_query(self, query: str, skip_downloading_pdf: bool = True):
+        documents = await self.data_source.query_documents(query, limit=1)
         if not documents:
-            raise DocumentNotFoundError(**{field: value})
-        await self.add_full_documents(documents)
-        return await asyncio.get_running_loop().run_in_executor(
-            None,
-            lambda: self.vector_storage.get_by_field_value(field, value),
-        )
+            raise DocumentNotFoundError(id_=query)
+        await self.upsert_documents(documents, skip_downloading_pdf=skip_downloading_pdf)
+        return documents[0].document_id
 
     async def export_chunks(self, query: str, output_path: str, n_documents: int, skip_downloading_pdf: bool = True):
         documents = await self.keywords_search(query, n_documents=n_documents)
         chunks = await self._get_missing_chunks(
             documents,
             skip_downloading_pdf=skip_downloading_pdf,
         )
@@ -184,60 +180,49 @@
             ])
 
     async def import_chunks(self, input_path: str):
         chunks = []
         with GzipFile(input_path, mode='rb') as zipper:
             for line in zipper.readlines():
                 chunk = json.loads(line)
-                doi = chunk['metadata']['doi']
+                if 'doi' in chunk['metadata']:
+                    chunk['metadata']['id'] = f"nexus_science:doi:{chunk['metadata'].pop('doi')}"
+                document_id = chunk['metadata']['id']
                 chunks_from_storage = await asyncio.get_running_loop().run_in_executor(
                     None,
-                    lambda: self.vector_storage.get_by_field_value('doi', doi)
+                    lambda: self.vector_storage.get_by_field_value('id', document_id)
                 )
                 if chunks_from_storage:
                     logging.getLogger('statbox').info({
                         'action': 'already_stored',
                         'mode': 'cybrex',
-                        'doi': doi,
+                        'id': document_id,
                     })
                     continue
                 chunk['embedding'] = base64.b64decode(chunk['embedding'])
                 chunk['embedding'] = [n.item() for n in np.frombuffer(chunk['embedding'], dtype=np.float64)]
                 chunks.append(chunk)
 
         if chunks:
             await asyncio.get_running_loop().run_in_executor(
                 None,
                 lambda: self.vector_storage.upsert(chunks),
             )
 
-    async def chat_document(self, field, value, query, n_chunks: int):
-        await self.add_full_document_by_field_value(field, value)
-
-        chunks = await self._query(query, n_chunks, where={field: value})
-        chain = QAChain(query=query, llm=self.model.llm)
-        answer = await asyncio.get_running_loop().run_in_executor(
-            None,
-            lambda: chain.process(chunks),
-        )
-
-        return answer
-
     async def chat_science(self, query: str, n_chunks: int, n_documents: int, semantic_threshold: float = 0.5):
         full_documents = await self.keywords_search(query, n_documents)
 
-        await self.add_full_documents(full_documents)
+        await self.upsert_documents(full_documents)
 
         chunks = await self._query(query, n_chunks, semantic_threshold=semantic_threshold)
         chain = QAChain(query=query, llm=self.model.llm)
         answer = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: chain.process(chunks),
         )
-
         return answer, chunks, await self.get_summa_documents_from_documents(chunks)
 
     async def _query(self, query: str, n_chunks: int = 3, where: Optional[dict] = None, semantic_threshold: float = 0.5):
         logging.getLogger('statbox').info({
             'action': 'query',
             'mode': 'cybrex',
             'query': query,
@@ -278,42 +263,51 @@
         )
         logging.getLogger('statbox').info({
             'action': 'extracted_keywords',
             'mode': 'cybrex',
             'keywords': keywords,
         })
         topic = ' '.join(map(lambda x: x[0], filter(lambda x: x[1] > 0.5, keywords)))
-        documents = await get_documents_on_topic(
-            summa_client=self.geck.get_summa_client(),
-            topic=topic,
-            documents=n_documents,
-        )
+        documents = await self.data_source.query_documents(query=topic, limit=n_documents)
         return documents
 
     async def get_summa_documents_from_documents(self, documents):
-        dois = set([document['metadata']['doi'] for document in documents])
+        ids = set([document['metadata']['id'] for document in documents])
         _summa_documents = await asyncio.gather(*[
             self.geck.get_summa_client().search_documents([{
                 'index_alias': 'nexus_science',
-                'query': {'term': {'field': 'doi', 'value': doi}},
+                'query': {'term': {'field': id_.split(':', 1)[0], 'value': id_.split(':', 1)[1]}},
                 'collectors': [{'top_docs': {'limit': 100}}],
             }])
-            for doi in dois
+            for id_ in ids
         ])
         summa_documents = []
         for summa_document in _summa_documents:
             summa_documents.append(summa_document[0])
         return summa_documents
 
     async def semantic_search(self, query: str, n_chunks: int = 10, n_documents: int = 30):
         documents = await self.keywords_search(query, n_documents)
-        await self.add_full_documents(documents)
+        await self.upsert_documents(documents)
         return await self._query(query, n_chunks)
 
-    async def summarize_document(self, field, value):
-        chunks = await self.add_full_document_by_field_value(field, value)
+    async def chat_document(self, document_query: str, query: str, n_chunks: int):
+        document_id = await self.upsert_document_by_query(document_query, skip_downloading_pdf=False)
+        chunks = await self._query(query=query, n_chunks=n_chunks, where={'id': document_id})
+
+        chain = QAChain(query=query, llm=self.model.llm)
+        answer = await asyncio.get_running_loop().run_in_executor(
+            None,
+            lambda: chain.process(chunks),
+        )
+
+        return answer
+
+    async def summarize_document(self, document_query):
+        document_id = await self.upsert_document_by_query(document_query)
+        chunks = self.vector_storage.get_by_field_value('id', document_id)
         chain = SummarizeChain(llm=self.model.llm)
         result = await asyncio.get_running_loop().run_in_executor(
             None,
             lambda: chain.process(chunks),
         )
         return result.strip()
```

### Comparing `cybrex-1.3.3/cybrex/document_chunker.py` & `cybrex-1.4.0/cybrex/document_chunker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
 from typing import List
 
 from bs4 import BeautifulSoup
 
+from .data_source.base import SourceDocument
+
 
 class DocumentChunker:
     def __init__(self, text_splitter, minimal_chunk_size: int = 128):
         self.text_splitter = text_splitter
         self.minimal_chunk_size = minimal_chunk_size
 
-    def to_chunks(self, document: dict) -> List[dict]:
+    def to_chunks(self, document: SourceDocument) -> List[dict]:
         logging.getLogger('statbox').info({
             'action': 'chunking',
-            'id': f'doi:{document["doi"]}',
+            'id': document.document_id,
             'mode': 'cybrex',
         })
-        abstract = document.get('abstract', '')
-        content = document.get('content')
+        abstract = document.document.get('abstract', '')
+        content = document.document.get('content')
         if not content:
             return []
 
         abstract_soup = BeautifulSoup(abstract, features='lxml')
         content_soup = BeautifulSoup(content, features='lxml')
 
         extracted_texts = []
@@ -37,13 +39,13 @@
 
         for chunk_id, chunk in enumerate(self.text_splitter.split_text('\n\n'.join(extracted_texts))):
             if len(chunk) < self.minimal_chunk_size:
                 continue
             chunks.append({
                 'text': chunk,
                 'metadata': {
-                    'doi': document['doi'],
+                    'id': document.document_id,
                     'length': len(chunk),
                     'chunk_id': chunk_id,
                 }
             })
         return chunks
```

### Comparing `cybrex-1.3.3/cybrex/models.py` & `cybrex-1.4.0/cybrex/models.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.3/cybrex/prompts/base.py` & `cybrex-1.4.0/cybrex/prompts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
             'openai': OpenAIPrompter()
         }[type_]
 
     def qa_prompt(self, question, chunks: List[dict]):
         if len(chunks) >= 1:
             return '''
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references using DOIs from extracted parts near corresponding statements in your answer.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 
 USER:
 Extracted parts:
 {summary}
 
 Question:
@@ -45,34 +44,34 @@
 
 ASSISTANT:'''.format(summary=self.generate_summary(chunks))
 
     def generate_summary(self, chunks: List[dict]):
         chunk_summaries = []
         chunk_summaries_grouped = OrderedDict()
         for chunk in chunks:
-            doi = chunk.get("metadata", {}).get("doi")
-            if doi not in chunk_summaries_grouped:
-                chunk_summaries_grouped[doi] = []
-            chunk_summaries_grouped[doi].append(chunk['text'])
-        for doi, texts in chunk_summaries_grouped.items():
+            id_ = chunk.get("metadata", {}).get("id")
+            if id_ not in chunk_summaries_grouped:
+                chunk_summaries_grouped[id_] = []
+            chunk_summaries_grouped[id_].append(chunk['text'])
+        for id_, texts in chunk_summaries_grouped.items():
             texts = ' <..> '.join(texts)
-            if doi:
-                chunk_summaries.append(f'DOI: {doi}\nCONTENT: {texts}')
+            if id_:
+                field, value = id_.split(':', 1)
+                chunk_summaries.append(f'{field.upper()}: {value}\nCONTENT: {texts}')
             else:
                 chunk_summaries.append(f'CONTENT: {texts}')
         return '\n'.join(chunk_summaries)
 
 
 class Llama27bPrompter(BasePrompter):
     def qa_prompt(self, question: str, chunks: List[dict]):
         if len(chunks) >= 1:
             return '''
 <s><<SYS>>
 You are Cybrex AI created by People of Nexus. Given the following extracted parts of a long document and a question, create a final answer.
-ALWAYS add references using DOIs from extracted parts near corresponding statements in your answer.
 If you don't know the answer, just say that you don't know. Don't try to make up an answer.
 <</SYS>>
 [INST]
 Extracted parts:
 {summary}
 
 Question:
```

### Comparing `cybrex-1.3.3/cybrex/vector_storage/chroma.py` & `cybrex-1.4.0/cybrex/vector_storage/chroma.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.3.3/cybrex.egg-info/SOURCES.txt` & `cybrex-1.4.0/cybrex.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 cybrex.egg-info/dependency_links.txt
 cybrex.egg-info/entry_points.txt
 cybrex.egg-info/requires.txt
 cybrex.egg-info/top_level.txt
 cybrex/chains/__init__.py
 cybrex/chains/base.py
 cybrex/chains/map_reduce.py
+cybrex/data_source/base.py
+cybrex/data_source/geck_data_source.py
 cybrex/prompts/__init__.py
 cybrex/prompts/base.py
 cybrex/vector_storage/__init__.py
 cybrex/vector_storage/base.py
 cybrex/vector_storage/chroma.py
```

### Comparing `cybrex-1.3.3/pyproject.toml` & `cybrex-1.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.3.3"
+version = "1.4.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```


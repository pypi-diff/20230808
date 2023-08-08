# Comparing `tmp/vlite-0.1.7.tar.gz` & `tmp/vlite-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.1.7.tar", last modified: Fri Jul  7 06:27:15 2023, max compression
+gzip compressed data, was "vlite-0.1.8.tar", last modified: Tue Aug  8 21:44:27 2023, max compression
```

## Comparing `vlite-0.1.7.tar` & `vlite-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.765326 vlite-0.1.7/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-07 06:27:15.765175 vlite-0.1.7/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     1547 2023-07-04 23:54:37.000000 vlite-0.1.7/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2023-07-07 06:27:15.765383 vlite-0.1.7/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      410 2023-07-07 06:23:53.000000 vlite-0.1.7/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.764253 vlite-0.1.7/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.7/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     2626 2023-07-04 15:11:01.000000 vlite-0.1.7/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     3278 2023-07-06 23:49:16.000000 vlite-0.1.7/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     3041 2023-07-04 15:13:56.000000 vlite-0.1.7/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-07-07 06:27:15.764963 vlite-0.1.7/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      176 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      224 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)       43 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2023-07-07 06:27:15.000000 vlite-0.1.7/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.954951 vlite-0.1.8/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-08-08 21:44:27.954815 vlite-0.1.8/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     1605 2023-07-07 07:20:20.000000 vlite-0.1.8/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2023-08-08 21:44:27.954997 vlite-0.1.8/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      410 2023-08-08 21:43:28.000000 vlite-0.1.8/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.953975 vlite-0.1.8/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       23 2023-07-04 08:27:33.000000 vlite-0.1.8/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     2760 2023-07-09 11:01:10.000000 vlite-0.1.8/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3278 2023-07-06 23:49:16.000000 vlite-0.1.8/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3066 2023-07-07 07:20:20.000000 vlite-0.1.8/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2023-08-08 21:44:27.954627 vlite-0.1.8/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      176 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      224 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)       43 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2023-08-08 21:44:27.000000 vlite-0.1.8/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.1.7/README.md` & `vlite-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 ![442f7062-ab69-4621-96ca-4ee66df06ffc](https://github.com/sdan/vlite/assets/22898443/fc36481c-f1f6-4973-8461-6aef3a04486d)
 
 ## usage
 
 ```python
 from vlite import VLite
 
-db = VLite()
+db = VLite() # default mps
+
+# db = VLite(device="cpu") # to run on cpu
 
 db.memorize(["hello world"]*5)
 
 db.remember("adele")
 
 ```
```

### Comparing `vlite-0.1.7/vlite/main.py` & `vlite-0.1.8/vlite/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 from uuid import uuid4
-from .model import EmbeddingModel
-from .utils import chop_and_chunk, cos_sim
+from vlite.model import EmbeddingModel
+from vlite.utils import chop_and_chunk, cos_sim
 
 class VLite:
     '''
     vlite is a simple vector database that stores vectors in a numpy array.
     '''
-    def __init__(self, collection='vlite.npz'):
+    def __init__(self, collection='vlite.npz',device='mps',model_name=None):
         self.collection = collection
-        self.model = EmbeddingModel()
+        self.device = device
+        self.model = EmbeddingModel() if model_name is None else EmbeddingModel(model_name)
         try:
             with np.load(self.collection, allow_pickle=True) as data:
                 self.texts = data['texts'].tolist()
                 self.metadata = data['metadata'].tolist()
                 self.vectors = data['vectors']
         except FileNotFoundError:
             self.texts = []
@@ -31,30 +32,30 @@
         # print("[get_similar_vectors] Top k idx:", top_k_idx)
         # print("[get_similar_vectors] Top k sims:", sims[top_k_idx])
         return top_k_idx, sims[top_k_idx]
 
     def memorize(self, text, id=None, metadata=None):
         id = id or str(uuid4())
         chunks = chop_and_chunk(text)
-        encoded_data = self.model.embed(texts=chunks, device="mps")
+        encoded_data = self.model.embed(texts=chunks, device=self.device)
         self.vectors = np.vstack((self.vectors, encoded_data))
         for chunk in chunks:
             self.texts.append(chunk)
             idx = len(self.texts) - 1
             self.metadata[idx] = metadata or {}
             self.metadata[idx]['index'] = id or idx
         self.save()
         return id, self.vectors
 
     def remember(self, text=None, id=None, top_k=5):
         if id:
             return self.metadata[id]
         if text:
 
-            sims = cos_sim(self.model.embed(texts=text, device="cpu") , self.vectors)
+            sims = cos_sim(self.model.embed(texts=text, device=self.device) , self.vectors)
             print("[remember] Sims:", sims.shape)
             sims = sims[0]
 
             # Use np.argpartition to partially sort only the top 5 values
             top_5_idx = np.argpartition(sims, -top_k)[-top_k:]  
 
             # Use np.argsort to sort just those top 5 indices
```

### Comparing `vlite-0.1.7/vlite/model.py` & `vlite-0.1.8/vlite/model.py`

 * *Files identical despite different names*

### Comparing `vlite-0.1.7/vlite/utils.py` & `vlite-0.1.8/vlite/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pysbd
 import PyPDF2
 import itertools
+from typing import List
 from transformers import AutoTokenizer, AutoModel
 import regex as re
 
 # def chop_and_chunk(text, max_seq_length=256):
 #     if isinstance(text, str):
 #         if len(text) < max_seq_length*4:
 #             return [text]
@@ -75,20 +76,20 @@
     extracted_text = []
     with open(pdf_path, "rb") as file:
         reader = PyPDF2.PdfReader(file)
         for page in iter(reader.pages):
             extracted_text.append(page.extract_text())  
     return extracted_text
 
-def visualize_tokens(token_values: list[str]) -> None:
+def visualize_tokens(token_values: List[str]) -> None:
         backgrounds = itertools.cycle(
             ["\u001b[48;5;{}m".format(i) for i in [167, 179, 185, 77, 80, 68, 134]]
         )
         interleaved = itertools.chain.from_iterable(zip(backgrounds, token_values))
         print(("".join(interleaved) + "\u001b[0m"))
 
 def token_count(texts):
         tz = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L6-v2', use_fast=True)
         tokens = 0
         for text in texts:
             tokens+=len(tz.tokenize(text, padding=True, truncation=True))
-        return tokens
+        return tokens
```


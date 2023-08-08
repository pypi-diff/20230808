# Comparing `tmp/sparsembed-0.0.2.tar.gz` & `tmp/sparsembed-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparsembed-0.0.2.tar", last modified: Sun Aug  6 21:04:03 2023, max compression
+gzip compressed data, was "sparsembed-0.0.3.tar", last modified: Tue Aug  8 00:18:43 2023, max compression
```

## Comparing `sparsembed-0.0.2.tar` & `sparsembed-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.277861 sparsembed-0.0.2/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-08-04 22:25:59.000000 sparsembed-0.0.2/LICENSE
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5462 2023-08-06 21:04:03.277938 sparsembed-0.0.2/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4842 2023-08-06 20:58:58.000000 sparsembed-0.0.2/README.md
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-08-06 21:04:03.278143 sparsembed-0.0.2/setup.cfg
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1118 2023-08-06 20:57:40.000000 sparsembed-0.0.2/setup.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.273590 sparsembed-0.0.2/sparsembed/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-08-04 23:19:14.000000 sparsembed-0.0.2/sparsembed/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-08-06 20:52:35.000000 sparsembed-0.0.2/sparsembed/__version__.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.275091 sparsembed-0.0.2/sparsembed/losses/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       83 2023-07-30 21:12:15.000000 sparsembed-0.0.2/sparsembed/losses/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2757 2023-08-04 22:59:07.000000 sparsembed-0.0.2/sparsembed/losses/cosine.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     1828 2023-08-05 00:12:23.000000 sparsembed-0.0.2/sparsembed/losses/flops.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.275740 sparsembed-0.0.2/sparsembed/model/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       61 2023-08-04 22:31:40.000000 sparsembed-0.0.2/sparsembed/model/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     7443 2023-08-06 20:46:28.000000 sparsembed-0.0.2/sparsembed/model/sparsembed.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.276330 sparsembed-0.0.2/sparsembed/retrieve/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       58 2023-08-06 20:43:44.000000 sparsembed-0.0.2/sparsembed/retrieve/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)    11031 2023-08-06 20:57:27.000000 sparsembed-0.0.2/sparsembed/retrieve/retriever.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.277604 sparsembed-0.0.2/sparsembed/utils/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      123 2023-08-04 23:23:36.000000 sparsembed-0.0.2/sparsembed/utils/__init__.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      145 2023-08-05 00:11:56.000000 sparsembed-0.0.2/sparsembed/utils/evaluate.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     2105 2023-08-06 20:51:55.000000 sparsembed-0.0.2/sparsembed/utils/iter.py
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     4317 2023-08-06 18:48:59.000000 sparsembed-0.0.2/sparsembed/utils/scores.py
-drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-06 21:04:03.274350 sparsembed-0.0.2/sparsembed.egg-info/
--rw-r--r--   0 raphael.sourty   (502) staff       (20)     5462 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/PKG-INFO
--rw-r--r--   0 raphael.sourty   (502) staff       (20)      574 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/SOURCES.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/dependency_links.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       44 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/requires.txt
--rw-r--r--   0 raphael.sourty   (502) staff       (20)       11 2023-08-06 21:04:03.000000 sparsembed-0.0.2/sparsembed.egg-info/top_level.txt
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.275513 sparsembed-0.0.3/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-08-04 22:25:59.000000 sparsembed-0.0.3/LICENSE
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5598 2023-08-08 00:18:43.275582 sparsembed-0.0.3/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4978 2023-08-08 00:16:12.000000 sparsembed-0.0.3/README.md
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-08-08 00:18:43.275800 sparsembed-0.0.3/setup.cfg
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1118 2023-08-06 20:57:40.000000 sparsembed-0.0.3/setup.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.271068 sparsembed-0.0.3/sparsembed/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-08-04 23:19:14.000000 sparsembed-0.0.3/sparsembed/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-08-07 23:38:32.000000 sparsembed-0.0.3/sparsembed/__version__.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.272824 sparsembed-0.0.3/sparsembed/losses/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       83 2023-07-30 21:12:15.000000 sparsembed-0.0.3/sparsembed/losses/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     2783 2023-08-07 23:37:55.000000 sparsembed-0.0.3/sparsembed/losses/cosine.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1828 2023-08-05 00:12:23.000000 sparsembed-0.0.3/sparsembed/losses/flops.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.273541 sparsembed-0.0.3/sparsembed/model/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       61 2023-08-04 22:31:40.000000 sparsembed-0.0.3/sparsembed/model/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     7443 2023-08-06 20:46:28.000000 sparsembed-0.0.3/sparsembed/model/sparsembed.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.274114 sparsembed-0.0.3/sparsembed/retrieve/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       58 2023-08-06 20:43:44.000000 sparsembed-0.0.3/sparsembed/retrieve/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)    11282 2023-08-08 00:17:16.000000 sparsembed-0.0.3/sparsembed/retrieve/retriever.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.275385 sparsembed-0.0.3/sparsembed/utils/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      123 2023-08-04 23:23:36.000000 sparsembed-0.0.3/sparsembed/utils/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      145 2023-08-05 00:11:56.000000 sparsembed-0.0.3/sparsembed/utils/evaluate.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1872 2023-08-06 21:13:53.000000 sparsembed-0.0.3/sparsembed/utils/iter.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4552 2023-08-08 00:11:09.000000 sparsembed-0.0.3/sparsembed/utils/scores.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-08-08 00:18:43.271894 sparsembed-0.0.3/sparsembed.egg-info/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5598 2023-08-08 00:18:43.000000 sparsembed-0.0.3/sparsembed.egg-info/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      574 2023-08-08 00:18:43.000000 sparsembed-0.0.3/sparsembed.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-08-08 00:18:43.000000 sparsembed-0.0.3/sparsembed.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       44 2023-08-08 00:18:43.000000 sparsembed-0.0.3/sparsembed.egg-info/requires.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       11 2023-08-08 00:18:43.000000 sparsembed-0.0.3/sparsembed.egg-info/top_level.txt
```

### Comparing `sparsembed-0.0.2/LICENSE` & `sparsembed-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.2/PKG-INFO` & `sparsembed-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsembed
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sparse Embeddings for Neural Search.
 Home-page: https://github.com/raphaelsty/sparseembed
 Download-URL: https://github.com/user/sparseembed/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,semantic search,SparseEmbed,Google Research
@@ -60,15 +60,15 @@
     device=device,
 )
 
 model = model.to(device)
 
 optimizer = torch.optim.AdamW(
     filter(lambda p: p.requires_grad, model.parameters()),
-    lr=2e-6,
+    lr=2e-5,
 )
 
 flops_loss = losses.Flops()
 
 cosine_loss = losses.Cosine()
 
 dataset = [
@@ -82,23 +82,24 @@
 for queries, documents, labels in utils.iter(
     dataset,
     device=device,
     epochs=1,
     batch_size=batch_size,
     shuffle=True,
 ):
-    queries_embeddings = model(queries, k=96)
+    queries_embeddings = model(queries, k=32)
 
-    documents_embeddings = model(documents, k=256)
+    documents_embeddings = model(documents, k=32)
 
     scores = utils.scores(
         queries_activations=queries_embeddings["activations"],
         queries_embeddings=queries_embeddings["embeddings"],
         documents_activations=documents_embeddings["activations"],
         documents_embeddings=documents_embeddings["embeddings"],
+        device=device,
     )
 
     loss = cosine_loss.dense(
         scores=scores,
         labels=labels,
     )
 
@@ -150,24 +151,25 @@
     key="id", 
     on="document", 
     model=model # Trained SparseEmbed model.
 )
 
 retriever = retriever.add(
     documents=documents,
-    k_token=64,
+    k_token=32, # Number of tokens to activate.
     batch_size=3,
 )
 
 retriever(
     q = [
         "Apple", 
         "Banana",
     ], 
-    k_sparse=64, 
+    k_sparse=20, # Number of documents to retrieve.
+    k_token=32, # Number of tokens to activate.
     batch_size=3
 )
 ```
 
 ```python
 [[{'id': 0, 'similarity': 195.057861328125},
   {'id': 1, 'similarity': 183.51429748535156},
```

### Comparing `sparsembed-0.0.2/README.md` & `sparsembed-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     device=device,
 )
 
 model = model.to(device)
 
 optimizer = torch.optim.AdamW(
     filter(lambda p: p.requires_grad, model.parameters()),
-    lr=2e-6,
+    lr=2e-5,
 )
 
 flops_loss = losses.Flops()
 
 cosine_loss = losses.Cosine()
 
 dataset = [
@@ -65,23 +65,24 @@
 for queries, documents, labels in utils.iter(
     dataset,
     device=device,
     epochs=1,
     batch_size=batch_size,
     shuffle=True,
 ):
-    queries_embeddings = model(queries, k=96)
+    queries_embeddings = model(queries, k=32)
 
-    documents_embeddings = model(documents, k=256)
+    documents_embeddings = model(documents, k=32)
 
     scores = utils.scores(
         queries_activations=queries_embeddings["activations"],
         queries_embeddings=queries_embeddings["embeddings"],
         documents_activations=documents_embeddings["activations"],
         documents_embeddings=documents_embeddings["embeddings"],
+        device=device,
     )
 
     loss = cosine_loss.dense(
         scores=scores,
         labels=labels,
     )
 
@@ -133,24 +134,25 @@
     key="id", 
     on="document", 
     model=model # Trained SparseEmbed model.
 )
 
 retriever = retriever.add(
     documents=documents,
-    k_token=64,
+    k_token=32, # Number of tokens to activate.
     batch_size=3,
 )
 
 retriever(
     q = [
         "Apple", 
         "Banana",
     ], 
-    k_sparse=64, 
+    k_sparse=20, # Number of documents to retrieve.
+    k_token=32, # Number of tokens to activate.
     batch_size=3
 )
 ```
 
 ```python
 [[{'id': 0, 'similarity': 195.057861328125},
   {'id': 1, 'similarity': 183.51429748535156},
```

### Comparing `sparsembed-0.0.2/setup.py` & `sparsembed-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.2/sparsembed/losses/cosine.py` & `sparsembed-0.0.3/sparsembed/losses/cosine.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     ... )
 
     >>> scores = utils.scores(
     ...     queries_activations=queries_embeddings["activations"],
     ...     queries_embeddings=queries_embeddings["embeddings"],
     ...     documents_activations=documents_embeddings["activations"],
     ...     documents_embeddings=documents_embeddings["embeddings"],
+    ...     device="cpu",
     ... )
 
     >>> cosine_loss = losses.Cosine()
 
     >>> loss += cosine_loss.sparse(
     ...     queries_sparse_activations=queries_embeddings["sparse_activations"],
     ...     documents_sparse_activations=documents_embeddings["sparse_activations"],
```

### Comparing `sparsembed-0.0.2/sparsembed/losses/flops.py` & `sparsembed-0.0.3/sparsembed/losses/flops.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.2/sparsembed/model/sparsembed.py` & `sparsembed-0.0.3/sparsembed/model/sparsembed.py`

 * *Files identical despite different names*

### Comparing `sparsembed-0.0.2/sparsembed/retrieve/retriever.py` & `sparsembed-0.0.3/sparsembed/retrieve/retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import torch
 import tqdm
+import warnings
 
 from ..model import SparsEmbed
 
 __all__ = ["Retriever"]
 
 
 class Retriever:
@@ -42,49 +43,49 @@
 
     >>> documents = [
     ...     {"id": 0, "document": "Food is good."},
     ...     {"id": 1, "document": "Sports is great."},
     ... ]
     >>> retriever = retriever.add(
     ...     documents=documents,
-    ...     k_token=256,
+    ...     k_token=32,
     ...     batch_size=24
     ... )
 
     >>> documents = [
     ...     {"id": 2, "document": "Cinema is great."},
     ...     {"id": 3, "document": "Music is amazing."},
     ... ]
     >>> retriever = retriever.add(
     ...     documents=documents,
-    ...     k_token=256,
+    ...     k_token=32,
     ...     batch_size=24
     ... )
 
-    >>> print(retriever(["Food", "Sports", "Cinema", "Music", "Hello World"], k_token=96))
-    [[{'id': 0, 'similarity': 1.4686675071716309},
-      {'id': 1, 'similarity': 1.345913052558899},
-      {'id': 3, 'similarity': 1.304019808769226},
-      {'id': 2, 'similarity': 1.1579231023788452}],
-     [{'id': 1, 'similarity': 7.0373148918151855},
-      {'id': 3, 'similarity': 3.528376817703247},
-      {'id': 2, 'similarity': 2.4535036087036133},
-      {'id': 0, 'similarity': 1.7893059253692627}],
-     [{'id': 2, 'similarity': 2.3167333602905273},
-      {'id': 3, 'similarity': 2.2312183380126953},
-      {'id': 1, 'similarity': 2.0195937156677246},
-      {'id': 0, 'similarity': 1.2890148162841797}],
-     [{'id': 3, 'similarity': 2.4722704887390137},
-      {'id': 2, 'similarity': 1.8648046255111694},
-      {'id': 1, 'similarity': 1.732576608657837},
-      {'id': 0, 'similarity': 1.3416467905044556}],
-     [{'id': 3, 'similarity': 3.7778899669647217},
-      {'id': 2, 'similarity': 3.198120355606079},
-      {'id': 1, 'similarity': 3.1253902912139893},
-      {'id': 0, 'similarity': 2.458303451538086}]]
+    >>> print(retriever(["Food", "Sports", "Cinema", "Music", "Hello World"], k_token=32))
+    [[{'id': 3, 'similarity': 0.5633876323699951},
+      {'id': 2, 'similarity': 0.4271728992462158},
+      {'id': 1, 'similarity': 0.4205787181854248},
+      {'id': 0, 'similarity': 0.3673652410507202}],
+     [{'id': 1, 'similarity': 1.547836184501648},
+      {'id': 3, 'similarity': 0.7415981888771057},
+      {'id': 2, 'similarity': 0.6557919979095459},
+      {'id': 0, 'similarity': 0.5385637879371643}],
+     [{'id': 3, 'similarity': 0.5051844716072083},
+      {'id': 2, 'similarity': 0.48867619037628174},
+      {'id': 1, 'similarity': 0.3863832950592041},
+      {'id': 0, 'similarity': 0.2812037169933319}],
+     [{'id': 3, 'similarity': 0.9398075938224792},
+      {'id': 1, 'similarity': 0.595514178276062},
+      {'id': 2, 'similarity': 0.5711489319801331},
+      {'id': 0, 'similarity': 0.46095147728919983}],
+     [{'id': 2, 'similarity': 1.3963655233383179},
+      {'id': 3, 'similarity': 1.2879667282104492},
+      {'id': 1, 'similarity': 1.229896068572998},
+      {'id': 0, 'similarity': 1.2129783630371094}]]
 
     """
 
     def __init__(
         self,
         key: str,
         on: list[str],
@@ -99,14 +100,17 @@
         # Mapping between sparse matrix index and document key.
         self.sparse_matrix = None
         self.documents_keys = {}
 
         # Documents embeddings and activations store.
         self.documents_embeddings, self.documents_activations = [], []
         os.environ["TOKENIZERS_PARALLELISM"] = tokenizer_parallelism
+        warnings.filterwarnings(
+            "ignore", ".*Sparse CSR tensor support is in beta state.*"
+        )
 
     def add(
         self,
         documents: list,
         k_token: int = 256,
         batch_size: int = 32,
     ) -> "Retriever":
@@ -310,16 +314,16 @@
     @staticmethod
     def _intersection(t1: torch.Tensor, t2: torch.Tensor) -> list[int]:
         t1, t2 = t1.flatten(), t2.flatten()
         combined = torch.cat((t1, t2), dim=0)
         uniques, counts = combined.unique(return_counts=True, sorted=False)
         return uniques[counts > 1].tolist()
 
-    @staticmethod
     def _get_scores(
+        self,
         queries_embeddings: list[torch.Tensor],
         documents_embeddings: list[list[torch.Tensor]],
         intersections: list[torch.Tensor],
     ) -> list:
         """Computes similarity scores between queries and documents with activated tokens embeddings."""
         return torch.stack(
             [
@@ -331,14 +335,16 @@
                                 dim=0,
                             )
                             * torch.stack(
                                 [query_embeddings[token] for token in intersection],
                                 dim=0,
                             )
                         )
+                        if len(intersection) > 0
+                        else torch.tensor(0.0, device=self.model.device)
                         for intersection, document_embddings in zip(
                             query_intersections, query_documents_embddings
                         )
                     ],
                     dim=0,
                 )
                 for query_intersections, query_embeddings, query_documents_embddings in zip(
```

### Comparing `sparsembed-0.0.2/sparsembed/utils/iter.py` & `sparsembed-0.0.3/sparsembed/utils/iter.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,23 +34,14 @@
     ...    ("Banana", "Apple is a popular fruit.", 0),
     ...    ("Banana", "Banana is a yellow fruit.", 1),
     ... ]
 
     >>> for queries, documents, labels in utils.iter(
     ...         X,
     ...         device="cpu",
-    ...         epochs=10,
-    ...         batch_size=3,
-    ...         shuffle=False
-    ...     ):
-    ...     print(queries)
-
-    >>> for queries, documents, labels in utils.iter(
-    ...         X,
-    ...         device="cpu",
     ...         epochs=1,
     ...         batch_size=3,
     ...         shuffle=False
     ...     ):
     ...     break
 
     >>> print(queries)
```

### Comparing `sparsembed-0.0.2/sparsembed/utils/scores.py` & `sparsembed-0.0.3/sparsembed/utils/scores.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,40 +35,44 @@
     ]
 
 
 def _get_scores(
     queries_embeddings_index: torch.Tensor,
     documents_embeddings_index: torch.Tensor,
     intersections: torch.Tensor,
+    device: str,
     func,
 ) -> list:
     """Computes similarity scores between queries and documents based on activated tokens embeddings"""
     return torch.stack(
         [
             func(
                 torch.stack(
                     [document_embeddings_index[token] for token in intersection], dim=0
                 )
                 * torch.stack(
                     [query_embeddings_index[token] for token in intersection], dim=0
                 )
             )
+            if len(intersection) > 0
+            else torch.tensor(0.0, device=device)
             for query_embeddings_index, document_embeddings_index, intersection in zip(
                 queries_embeddings_index, documents_embeddings_index, intersections
             )
         ],
         dim=0,
     )
 
 
 def scores(
     queries_activations: torch.Tensor,
     queries_embeddings: torch.Tensor,
     documents_activations: torch.Tensor,
     documents_embeddings: torch.Tensor,
+    device: str,
     func=torch.mean,
 ) -> list:
     """Computes score between queries and documents intersected activated tokens.
 
     Parameters
     ----------
     queries_activations
@@ -107,14 +111,16 @@
     ... )
 
     >>> scores = utils.scores(
     ...     queries_activations=queries_embeddings["activations"],
     ...     queries_embeddings=queries_embeddings["embeddings"],
     ...     documents_activations=documents_embeddings["activations"],
     ...     documents_embeddings=documents_embeddings["embeddings"],
+    ...     func=torch.sum, # torch.sum is dedicated to training
+    ...     device="cpu",
     ... )
 
     """
     queries_embeddings_index = _build_index(
         activations=queries_activations, embeddings=queries_embeddings
     )
 
@@ -128,8 +134,9 @@
     )
 
     return _get_scores(
         queries_embeddings_index=queries_embeddings_index,
         documents_embeddings_index=documents_embeddings_index,
         intersections=intersections,
         func=func,
+        device=device,
     )
```

### Comparing `sparsembed-0.0.2/sparsembed.egg-info/PKG-INFO` & `sparsembed-0.0.3/sparsembed.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparsembed
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sparse Embeddings for Neural Search.
 Home-page: https://github.com/raphaelsty/sparseembed
 Download-URL: https://github.com/user/sparseembed/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,semantic search,SparseEmbed,Google Research
@@ -60,15 +60,15 @@
     device=device,
 )
 
 model = model.to(device)
 
 optimizer = torch.optim.AdamW(
     filter(lambda p: p.requires_grad, model.parameters()),
-    lr=2e-6,
+    lr=2e-5,
 )
 
 flops_loss = losses.Flops()
 
 cosine_loss = losses.Cosine()
 
 dataset = [
@@ -82,23 +82,24 @@
 for queries, documents, labels in utils.iter(
     dataset,
     device=device,
     epochs=1,
     batch_size=batch_size,
     shuffle=True,
 ):
-    queries_embeddings = model(queries, k=96)
+    queries_embeddings = model(queries, k=32)
 
-    documents_embeddings = model(documents, k=256)
+    documents_embeddings = model(documents, k=32)
 
     scores = utils.scores(
         queries_activations=queries_embeddings["activations"],
         queries_embeddings=queries_embeddings["embeddings"],
         documents_activations=documents_embeddings["activations"],
         documents_embeddings=documents_embeddings["embeddings"],
+        device=device,
     )
 
     loss = cosine_loss.dense(
         scores=scores,
         labels=labels,
     )
 
@@ -150,24 +151,25 @@
     key="id", 
     on="document", 
     model=model # Trained SparseEmbed model.
 )
 
 retriever = retriever.add(
     documents=documents,
-    k_token=64,
+    k_token=32, # Number of tokens to activate.
     batch_size=3,
 )
 
 retriever(
     q = [
         "Apple", 
         "Banana",
     ], 
-    k_sparse=64, 
+    k_sparse=20, # Number of documents to retrieve.
+    k_token=32, # Number of tokens to activate.
     batch_size=3
 )
 ```
 
 ```python
 [[{'id': 0, 'similarity': 195.057861328125},
   {'id': 1, 'similarity': 183.51429748535156},
```

### Comparing `sparsembed-0.0.2/sparsembed.egg-info/SOURCES.txt` & `sparsembed-0.0.3/sparsembed.egg-info/SOURCES.txt`

 * *Files identical despite different names*


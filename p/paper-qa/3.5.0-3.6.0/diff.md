# Comparing `tmp/paper-qa-3.5.0.tar.gz` & `tmp/paper-qa-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.5.0.tar", last modified: Thu Jul 27 13:02:25 2023, max compression
+gzip compressed data, was "paper-qa-3.6.0.tar", last modified: Tue Aug  8 16:59:34 2023, max compression
```

## Comparing `paper-qa-3.5.0.tar` & `paper-qa-3.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.765984 paper-qa-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 13:01:37.000000 paper-qa-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-27 13:02:25.765984 paper-qa-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-27 13:01:37.000000 paper-qa-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:02:25.765984 paper-qa-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 13:01:37.000000 paper-qa-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28728 2023-07-27 13:01:37.000000 paper-qa-3.5.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:59:34.799382 paper-qa-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 16:58:55.000000 paper-qa-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-08-08 16:59:34.799382 paper-qa-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-08-08 16:58:55.000000 paper-qa-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:59:34.795382 paper-qa-3.6.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-08-08 16:59:34.000000 paper-qa-3.6.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-08 16:59:34.000000 paper-qa-3.6.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:59:34.000000 paper-qa-3.6.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 16:59:34.000000 paper-qa-3.6.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 16:59:34.000000 paper-qa-3.6.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:59:34.795382 paper-qa-3.6.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:59:34.799382 paper-qa-3.6.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 16:58:55.000000 paper-qa-3.6.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:59:34.799382 paper-qa-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 16:58:55.000000 paper-qa-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:59:34.799382 paper-qa-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29817 2023-08-08 16:58:55.000000 paper-qa-3.6.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.5.0/LICENSE` & `paper-qa-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/PKG-INFO` & `paper-qa-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.5.0
+Version: 3.6.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
-License: MIT
+License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Paper QA- [Paper QA](#paper-qa)
 - [Paper QA- Paper QA](#paper-qa--paper-qa)
   - [Output Example](#output-example)
```

### Comparing `paper-qa-3.5.0/README.md` & `paper-qa-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.6.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.5.0
+Version: 3.6.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
-License: MIT
+License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Paper QA- [Paper QA](#paper-qa)
 - [Paper QA- Paper QA](#paper-qa--paper-qa)
   - [Output Example](#output-example)
```

### Comparing `paper-qa-3.5.0/paperqa/chains.py` & `paper-qa-3.6.0/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/paperqa/contrib/zotero.py` & `paper-qa-3.6.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/paperqa/docs.py` & `paper-qa-3.6.0/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,19 +359,21 @@
         """Clear the memory of the model."""
         if self.memory_model is not None:
             self.memory_model.clear()
 
     def get_evidence(
         self,
         answer: Answer,
-        k: int = 3,
+        k: int = 10,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
         detailed_citations: bool = False,
+        disable_vector_search: bool = False,
+        disable_summarization: bool = False,
     ) -> Answer:
         # special case for jupyter notebooks
         if "get_ipython" in globals() or "google.colab" in sys.modules:
             import nest_asyncio
 
             nest_asyncio.apply()
         try:
@@ -383,36 +385,41 @@
             self.aget_evidence(
                 answer,
                 k=k,
                 max_sources=max_sources,
                 marginal_relevance=marginal_relevance,
                 get_callbacks=get_callbacks,
                 detailed_citations=detailed_citations,
+                disable_vector_search=disable_vector_search,
+                disable_summarization=disable_summarization,
             )
         )
 
     async def aget_evidence(
         self,
         answer: Answer,
-        k: int = 3,
-        max_sources: int = 5,
+        k: int = 10,  # Number of vectors to retrieve
+        max_sources: int = 5,  # Number of scored contexts to use
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
         detailed_citations: bool = False,
+        disable_vector_search: bool = False,
+        disable_summarization: bool = False,
     ) -> Answer:
+        if disable_vector_search:
+            k = k * 10000
         if len(self.docs) == 0 and self.doc_index is None:
             return answer
         self._build_texts_index(keys=answer.dockey_filter)
         if self.texts_index is None:
             return answer
         self.texts_index = cast(VectorStore, self.texts_index)
         _k = k
         if answer.dockey_filter is not None:
             _k = k * 10  # heuristic
-        # want to work through indices but less k
         if marginal_relevance:
             matches = self.texts_index.max_marginal_relevance_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         else:
             matches = self.texts_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
@@ -465,45 +472,60 @@
                     text=match.page_content,
                     callbacks=callbacks,
                 )
             except Exception as e:
                 if guess_is_4xx(str(e)):
                     return None
                 raise e
-            if "not applicable" in context.lower():
+            if "not applicable" in context.lower() or "not relevant" in context.lower():
                 return None
             c = Context(
                 context=context,
                 text=Text(
                     text=match.page_content,
                     name=match.metadata["name"],
                     doc=Doc(**match.metadata["doc"]),
                 ),
                 score=get_score(context),
             )
             return c
 
-        results = await gather_with_concurrency(
-            self.max_concurrent, *[process(m) for m in matches]
+        if disable_summarization:
+            contexts = [
+                Context(
+                    context=match.page_content,
+                    score=10,
+                    text=Text(
+                        text=match.page_content,
+                        name=match.metadata["name"],
+                        doc=Doc(**match.metadata["doc"]),
+                    ),
+                )
+                for match in matches
+            ]
+
+        else:
+            results = await gather_with_concurrency(
+                self.max_concurrent, *[process(m) for m in matches]
+            )
+            # filter out failures
+            contexts = [c for c in results if c is not None]
+
+        answer.contexts = sorted(
+            contexts + answer.contexts, key=lambda x: x.score, reverse=True
         )
-        # filter out failures
-        contexts = [c for c in results if c is not None]
-        if len(contexts) == 0:
-            return answer
-        contexts = sorted(contexts, key=lambda x: x.score, reverse=True)
-        contexts = contexts[:max_sources]
-        # add to answer contexts
-        answer.contexts += contexts
+        answer.contexts = answer.contexts[:max_sources]
         context_str = "\n\n".join(
             [
                 f"{c.text.name}: {c.context}"
                 + (f" Based on {c.text.doc.citation}" if detailed_citations else "")
                 for c in answer.contexts
             ]
         )
+
         valid_names = [c.text.name for c in answer.contexts]
         context_str += "\n\nValid keys: " + ", ".join(valid_names)
         answer.context = context_str
         return answer
 
     def query(
         self,
```

### Comparing `paper-qa-3.5.0/paperqa/prompts.py` & `paper-qa-3.6.0/paperqa/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     template="Select papers that may help answer the question below. "
     "Papers are listed as $KEY: $PAPER_INFO. "
     "Return a list of keys, separated by commas. "
     'Return "None", if no papers are applicable. '
     "Choose papers that are relevant, from reputable sources, and timely "
     "(if the question requires timely information). \n\n"
     "Question: {question}\n\n"
-    "{papers}\n\n"
+    "Papers: {papers}\n\n"
     "Selected keys:",
 )
 
 # We are unable to serialize with partial variables
 # so TODO: update year next year
 citation_prompt = PromptTemplate(
     input_variables=["text"],
```

### Comparing `paper-qa-3.5.0/paperqa/readers.py` & `paper-qa-3.6.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/paperqa/types.py` & `paper-qa-3.6.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/paperqa/utils.py` & `paper-qa-3.6.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.5.0/setup.py` & `paper-qa-3.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="paper-qa",
     version=__version__,
     description="LLM Chain for answering questions from docs ",
     author="Andrew White",
     author_email="white.d.andrew@gmail.com",
     url="https://github.com/whitead/paper-qa",
-    license="MIT",
+    license="Apache License 2.0",
     packages=["paperqa", "paperqa.contrib"],
     install_requires=[
         "pypdf",
         "langchain>=0.0.198",
         "openai >= 0.27.8",
         "faiss-cpu",
         "PyCryptodome",
@@ -26,11 +26,11 @@
         "tiktoken>=0.4.0",
     ],
     test_suite="tests",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `paper-qa-3.5.0/tests/test_paperqa.py` & `paper-qa-3.6.0/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,39 @@
 
 
 class TestHandler(AsyncCallbackHandler):
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         print(token)
 
 
+def test_ablations():
+    tests_dir = os.path.dirname(os.path.abspath(__file__))
+    doc_path = os.path.join(tests_dir, "paper.pdf")
+    with open(doc_path, "rb") as f:
+        docs = Docs()
+        docs.add_file(f, "Wellawatte et al, XAI Review, 2023")
+        answer = docs.get_evidence(
+            Answer(
+                question="Which page is the statement 'Deep learning (DL) is advancing the boundaries of computational"
+                + "chemistry because it can accurately model non-linear structure-function relationships.' on?"
+            ),
+            disable_summarization=True,
+        )
+        assert (
+            answer.contexts[0].text.text == answer.contexts[0].context
+        ), "summarization not ablated"
+        answer = docs.get_evidence(
+            Answer(
+                question="Which page is the statement 'Deep learning (DL) is advancing the boundaries of computational"
+                + "chemistry because it can accurately model non-linear structure-function relationships.' on?"
+            ),
+            disable_vector_search=True,
+        )
+
+
 def test_location_awareness():
     tests_dir = os.path.dirname(os.path.abspath(__file__))
     doc_path = os.path.join(tests_dir, "paper.pdf")
     with open(doc_path, "rb") as f:
         docs = Docs()
         docs.add_file(f, "Wellawatte et al, XAI Review, 2023")
         answer = docs.get_evidence(
```


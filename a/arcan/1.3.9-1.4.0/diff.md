# Comparing `tmp/arcan-1.3.9.tar.gz` & `tmp/arcan-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.9.tar", max compression
+gzip compressed data, was "arcan-1.4.0.tar", max compression
```

## Comparing `arcan-1.3.9.tar` & `arcan-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
--rw-r--r--   0        0        0     1711 2023-08-07 05:27:49.814621 arcan-1.3.9/LICENSE
--rw-r--r--   0        0        0     2888 2023-08-07 05:27:49.814621 arcan-1.3.9/README.md
--rw-r--r--   0        0        0     2610 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/agent/__init__.py
--rw-r--r--   0        0        0     4154 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/agent/qanda.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/ml/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/session/__init__.py
--rw-r--r--   0        0        0       31 2023-08-07 05:27:49.818621 arcan-1.3.9/arcan/storage/__init__.py
--rw-r--r--   0        0        0       62 2023-08-07 05:27:49.818621 arcan-1.3.9/main.py
--rw-r--r--   0        0        0      930 2023-08-07 05:27:49.818621 arcan-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 arcan-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-08-08 07:45:17.436442 arcan-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2888 2023-08-08 07:45:17.436442 arcan-1.4.0/README.md
+-rw-r--r--   0        0        0     3117 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/__init__.py
+-rw-r--r--   0        0        0     2534 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/chains.py
+-rw-r--r--   0        0        0     1113 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/llm.py
+-rw-r--r--   0        0        0     1370 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/scrapping.py
+-rw-r--r--   0        0        0     3713 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/streaming_gpt.py
+-rw-r--r--   0        0        0     1316 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/templates.py
+-rw-r--r--   0        0        0     3020 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/agent/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/ml/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/processing/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/session/__init__.py
+-rw-r--r--   0        0        0      636 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/session/auth.py
+-rw-r--r--   0        0        0       31 2023-08-08 07:45:17.440442 arcan-1.4.0/arcan/storage/__init__.py
+-rw-r--r--   0        0        0       62 2023-08-08 07:45:17.440442 arcan-1.4.0/main.py
+-rw-r--r--   0        0        0     1027 2023-08-08 07:45:17.444442 arcan-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 arcan-1.4.0/PKG-INFO
```

### Comparing `arcan-1.3.9/LICENSE` & `arcan-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.9/README.md` & `arcan-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `arcan-1.3.9/arcan/__init__.py` & `arcan-1.4.0/arcan/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # %%
-from fastapi import Depends, Header, HTTPException, Request, status
-from fastapi.security import (APIKeyHeader, HTTPAuthorizationCredentials,
-                              HTTPBearer)
-from modal import Image, Secret, Stub, create_package_mounts, web_endpoint
+from fastapi import Depends
+from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
+from modal import Image, Secret, Stub, web_endpoint
+
+from arcan.session.auth import requires_auth
+from arcan.agent.chains import ArcanConversationChain
+from arcan.agent.vectorstores import faiss_text_index_loader, load_faiss_vectorstore
+from arcan.agent.scrapping import url_text_scrapper
 
-from arcan.agent.qanda import qanda_langchain
 
 auth_scheme = HTTPBearer()
 
 
-__version__ = "1.3.9"
+__version__ = "1.4.0"
+
 
 # %%
 def get_arcan_version():
     try:
         import arcan
 
         return arcan.__version__
     except Exception as e:
         print(e)
         return "No arcan package is installed"
 
 
 # %%
 image = Image.debian_slim().pip_install(
-    "fastapi", 
+    "fastapi",
     "uvicorn",
-    "databricks_session", 
+    "databricks_session",
     "arcan",
     # scraping pkgs
     "beautifulsoup4",
     "httpx",
     "lxml",
     # langchain pkgs
     "faiss-cpu",
@@ -41,67 +45,73 @@
 # api = FastAPI()
 stub = Stub(
     name="arcan",
     image=image,
     secrets=[Secret.from_name("openai-secret")],
 )
 
+
 @stub.function()
-@web_endpoint(method="GET") #, custom_domains=["arcanapp.io"])
+@web_endpoint(method="GET", custom_domains=["app.arcanai.tech"])
 # @api.get("/")
 def entrypoint():
     return {"message": "Arcan is running"}
 
 
 @stub.function()
-@web_endpoint(method="GET")
+@web_endpoint(method="GET", custom_domains=["version.arcanai.tech"])
 # @api.get("/api/version")
 def version():
     print("Arcan is installed")
     # return the installed version of Arcan package from the pyproject.toml file
     version = get_arcan_version()
     return {"message": f"Arcan version {version} is installed"}
 
 
-# %%
+chain = ArcanConversationChain()
+docsearch = None
+job_domain = None
+
+
+def url_text_scrapping_chain(query: str, url: str) -> tuple[str, list[str]]:
+    global docsearch, job_domain, chain
+    print(docsearch, job_domain)
+    text, current_domain = url_text_scrapper(url)
+    if not docsearch and current_domain != job_domain:
+        try:
+            print("Loading index")
+            job_domain = current_domain
+            docsearch = load_faiss_vectorstore(index_key=current_domain)
+        except Exception as e:
+            print(f"Error loading index: {e}, creating new index")
+            docsearch = faiss_text_index_loader(text=text, index_key=current_domain)
+    print("Running chain")
+    return chain.run(query, docsearch)
 
 
 @stub.function(secret=Secret.from_name("web-auth-token"))
-@web_endpoint(method="GET")
-def qanda(query: str, context_url: str, show_sources: bool = False, token: HTTPAuthorizationCredentials = Depends(auth_scheme)):
-    import os
-
-    print(os.environ["AUTH_TOKEN"])
-
-    if token.credentials != os.environ["AUTH_TOKEN"]:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect bearer token",
-            headers={"WWW-Authenticate": "Bearer"},
-        )
-
-    answer, sources = qanda_langchain(query=query, url=context_url)
-    if show_sources:
-        return {
-            "answer": answer,
-            "sources": sources,
-        }
-    else:
-        return {
-            "answer": answer,
-        }
-
-
-@stub.function()
-def qanda_cli(query: str, show_sources: bool = False, context_url: str = None):
-    answer, sources = qanda_langchain(query=query, url=context_url)
-    # Terminal codes for pretty-printing.
-    bold, end = "\033[1m", "\033[0m"
-
-    print(f"🦜 {bold}ANSWER:{end}")
-    print(answer)
-    if show_sources:
-        print(f"🔗 {bold}SOURCES:{end}")
-        for text in sources:
-            print(text)
-            print("----")
-
+@web_endpoint(method="GET", custom_domains=["text-chat.arcanai.tech"])
+@requires_auth
+def text_chat(
+    query: str,
+    context_url: str,
+    token: HTTPAuthorizationCredentials = Depends(auth_scheme),
+):
+    answer = url_text_scrapping_chain(query=query, url=context_url)
+    return {
+        "answer": answer,
+    }
+
+
+# @stub.function()
+# def qanda_cli(query: str, show_sources: bool = False, context_url: str = None):
+#     answer, sources = url_text_scrapping_chain(query=query, url=context_url)
+#     # Terminal codes for pretty-printing.
+#     bold, end = "\033[1m", "\033[0m"
+
+#     print(f"🦜 {bold}ANSWER:{end}")
+#     print(answer)
+#     if show_sources:
+#         print(f"🔗 {bold}SOURCES:{end}")
+#         for text in sources:
+#             print(text)
+#             print("----")
```

### Comparing `arcan-1.3.9/pyproject.toml` & `arcan-1.4.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.3.9"
+version = "1.4.0"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
@@ -21,14 +21,19 @@
 langchain = "^0.0.254"
 openai = "^0.27.8"
 httpx = "^0.24.1"
 beautifulsoup4 = "^4.12.2"
 lxml = "^4.9.3"
 faiss-cpu = "^1.7.4"
 tiktoken = "^0.4.0"
+transformers = "^4.31.0"
+whisper = "^1.1.10"
+ffmpeg = "^1.4"
+torch = "^2.0.1"
+fschat = "^0.2.23"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.23.3"
 
 [build-system]
```

### Comparing `arcan-1.3.9/PKG-INFO` & `arcan-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: arcan
-Version: 1.3.9
+Version: 1.4.0
 Summary: A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools
 License: arcan.ai Non-Commercial Open Source License
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fastapi (>=0.98,<0.100)
+Requires-Dist: ffmpeg (>=1.4,<2.0)
+Requires-Dist: fschat (>=0.2.23,<0.3.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: langchain (>=0.0.254,<0.0.255)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: modal-client (>=0.49.2509,<0.51.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: transformers (>=4.31.0,<5.0.0)
 Requires-Dist: urllib3 (<=2.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
+Requires-Dist: whisper (>=1.1.10,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Arcan: AI Driven Data Pipeline Orchestration
 
 <p align="center">
   <a href="https://arcanapp.io">
     <img src="public/arcan.png" height="96">
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: arcan Version: 1.3.9 Summary: A multiheaded modern
+Metadata-Version: 2.1 Name: arcan Version: 1.4.0 Summary: A multiheaded modern
 data bridging package based on pipeline manifests to integrate between any
 modern (and old) data stack tools License: arcan.ai Non-Commercial Open Source
 License Author: Carlos D. Escobar-Valbuena Author-email:
 carlosdavidescobar@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: black (>=23.3.0,<24.0.0) Requires-Dist: faiss-cpu
-(>=1.7.4,<2.0.0) Requires-Dist: fastapi (>=0.98,<0.100) Requires-Dist: httpx
+(>=1.7.4,<2.0.0) Requires-Dist: fastapi (>=0.98,<0.100) Requires-Dist: ffmpeg
+(>=1.4,<2.0) Requires-Dist: fschat (>=0.2.23,<0.3.0) Requires-Dist: httpx
 (>=0.24.1,<0.25.0) Requires-Dist: langchain (>=0.0.254,<0.0.255) Requires-Dist:
 lxml (>=4.9.3,<5.0.0) Requires-Dist: modal-client (>=0.49.2509,<0.51.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0) Requires-Dist: tiktoken
-(>=0.4.0,<0.5.0) Requires-Dist: urllib3 (<=2.0) Requires-Dist: uvicorn
-(>=0.22.0,<0.23.0) Description-Content-Type: text/markdown # Arcan: AI Driven
-Data Pipeline Orchestration
+(>=0.4.0,<0.5.0) Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist:
+transformers (>=4.31.0,<5.0.0) Requires-Dist: urllib3 (<=2.0) Requires-Dist:
+uvicorn (>=0.22.0,<0.23.0) Requires-Dist: whisper (>=1.1.10,<2.0.0)
+Description-Content-Type: text/markdown # Arcan: AI Driven Data Pipeline
+Orchestration
                               [public/arcan.png]
  Your data bridging concierge. Leverage AI to integrate diverse big and small
         data stack tools with ease. Visit our live demo at arcanapp.io.
 
 # Introduction Arcan is an innovative open-source solution designed to bridge
 modern and legacy data stack tools through a multiheaded package based on a
 smart pipeline generation and orchestration. Leveraging a hybrid Next.js +
```


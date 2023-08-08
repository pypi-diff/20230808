# Comparing `tmp/hyfi_absa-0.3.1.tar.gz` & `tmp/hyfi_absa-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_absa-0.3.1.tar", max compression
+gzip compressed data, was "hyfi_absa-0.3.2.tar", max compression
```

## Comparing `hyfi_absa-0.3.1.tar` & `hyfi_absa-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1071 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/LICENSE
--rw-r--r--   0        0        0     2598 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/README.md
--rw-r--r--   0        0        0     2965 2023-08-04 06:39:35.519578 hyfi_absa-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      181 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/__cli__.py
--rw-r--r--   0        0        0      473 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/__init__.py
--rw-r--r--   0        0        0       22 2023-08-04 06:39:35.475577 hyfi_absa-0.3.1/src/hyabsa/_version.py
--rw-r--r--   0        0        0      157 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/agents/__init__.py
--rw-r--r--   0        0        0      641 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/agents/absa.py
--rw-r--r--   0        0        0     1532 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/agents/base.py
--rw-r--r--   0        0        0      922 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/agents/results.py
--rw-r--r--   0        0        0        0 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/__init__.py
--rw-r--r--   0        0        0      234 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/about/hyabsa.yaml
--rw-r--r--   0        0        0      158 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/agent/__init__.yaml
--rw-r--r--   0        0        0      158 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/agent/absa.yaml
--rw-r--r--   0        0        0       64 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/agent/gpt4.yaml
--rw-r--r--   0        0        0       51 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/llm/__init__.yaml
--rw-r--r--   0        0        0       91 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/llm/gpt35.yaml
--rw-r--r--   0        0        0       80 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/llm/gpt4.yaml
--rw-r--r--   0        0        0      111 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/llm/openai.yaml
--rw-r--r--   0        0        0      441 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/prompts/__help__.yaml
--rw-r--r--   0        0        0       64 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/prompts/__init__.yaml
--rw-r--r--   0        0        0     2975 2023-08-04 06:39:10.755176 hyfi_absa-0.3.1/src/hyabsa/conf/prompts/default.yaml
--rw-r--r--   0        0        0      448 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/conf/runner/absa.yaml
--rw-r--r--   0        0        0       51 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/conf/runner/gpt4.yaml
--rw-r--r--   0        0        0      108 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/contexts/__init__.py
--rw-r--r--   0        0        0      127 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/llms/__init__.py
--rw-r--r--   0        0        0     3041 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/llms/openai.py
--rw-r--r--   0        0        0      744 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/prompts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/py.typed
--rw-r--r--   0        0        0       62 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/runners/__init__.py
--rw-r--r--   0        0        0     2990 2023-08-04 06:39:10.759176 hyfi_absa-0.3.1/src/hyabsa/runners/absa.py
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 hyfi_absa-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-08 11:11:12.269254 hyfi_absa-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2598 2023-08-08 11:11:12.269254 hyfi_absa-0.3.2/README.md
+-rw-r--r--   0        0        0     2965 2023-08-08 11:11:37.589825 hyfi_absa-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      181 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-08 11:11:37.549824 hyfi_absa-0.3.2/src/hyabsa/_version.py
+-rw-r--r--   0        0        0      157 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/agents/__init__.py
+-rw-r--r--   0        0        0      641 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/agents/absa.py
+-rw-r--r--   0        0        0     1532 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/agents/base.py
+-rw-r--r--   0        0        0      922 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/agents/results.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/__init__.py
+-rw-r--r--   0        0        0      234 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/about/hyabsa.yaml
+-rw-r--r--   0        0        0      206 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/agent/__init__.yaml
+-rw-r--r--   0        0        0      158 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/agent/absa.yaml
+-rw-r--r--   0        0        0       64 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/agent/gpt4.yaml
+-rw-r--r--   0        0        0       52 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/llm/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/llm/gpt35.yaml
+-rw-r--r--   0        0        0       80 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/llm/gpt4.yaml
+-rw-r--r--   0        0        0      111 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/llm/openai.yaml
+-rw-r--r--   0        0        0      441 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/prompts/__help__.yaml
+-rw-r--r--   0        0        0       65 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/prompts/__init__.yaml
+-rw-r--r--   0        0        0     2975 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/prompts/default.yaml
+-rw-r--r--   0        0        0      434 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/runner/absa.yaml
+-rw-r--r--   0        0        0       51 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/conf/runner/gpt4.yaml
+-rw-r--r--   0        0        0      108 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/contexts/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/llms/__init__.py
+-rw-r--r--   0        0        0     3047 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/llms/openai.py
+-rw-r--r--   0        0        0      744 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/py.typed
+-rw-r--r--   0        0        0       62 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/runners/__init__.py
+-rw-r--r--   0        0        0     2996 2023-08-08 11:11:12.273254 hyfi_absa-0.3.2/src/hyabsa/runners/absa.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 hyfi_absa-0.3.2/PKG-INFO
```

### Comparing `hyfi_absa-0.3.1/LICENSE` & `hyfi_absa-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/README.md` & `hyfi_absa-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/pyproject.toml` & `hyfi_absa-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "hyfi-absa"
-version = "0.3.1"
+version = "0.3.2"
 description = "HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-absa.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-absa"
 readme = "README.md"
 packages = [{ include = "hyabsa", from = "src" }]
 
 [tool.poetry.scripts]
 hyabsa = 'hyabsa.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.18.0"
+hyfi = "^1.25.0"
 backoff = "^2.2.1"
 openai = "^0.27.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `hyfi_absa-0.3.1/src/hyabsa/agents/absa.py` & `hyfi_absa-0.3.2/src/hyabsa/agents/absa.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/src/hyabsa/agents/base.py` & `hyfi_absa-0.3.2/src/hyabsa/agents/base.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/src/hyabsa/agents/results.py` & `hyfi_absa-0.3.2/src/hyabsa/agents/results.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/src/hyabsa/conf/prompts/default.yaml` & `hyfi_absa-0.3.2/src/hyabsa/conf/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/src/hyabsa/llms/openai.py` & `hyfi_absa-0.3.2/src/hyabsa/llms/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def engine(self):
         if self._engine_ is None:
             self.initialize()
         return self._engine_
 
     def initialize(self, api_key: Optional[str] = None):
         api_key = api_key or self.api_key
-        denv = HyFI.dotenv()
+        denv = HyFI.DotEnvConfig()
         if not api_key and denv.OPENAI_API_KEY:
             api_key = denv.OPENAI_API_KEY.get_secret_value()
         if not api_key:
             raise ValueError("OpenAI API Key is required.")
         openai.api_key = api_key
         logger.info("OpenAI API Key is set successfully.")
         self._engine_ = openai.ChatCompletion()
```

### Comparing `hyfi_absa-0.3.1/src/hyabsa/prompts/__init__.py` & `hyfi_absa-0.3.2/src/hyabsa/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi_absa-0.3.1/src/hyabsa/runners/absa.py` & `hyfi_absa-0.3.2/src/hyabsa/runners/absa.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,16 +74,16 @@
             print(dataset[0])
         self.save_dataset(dataset)
 
 
 def batch_run(
     batch,
     task: str = "QUAD",
-    agent: AbsaAgent = None,
-    text_col: str = "bodyText",
+    agent: Optional[AbsaAgent] = None,
+    text_col: str = "text",
 ) -> dict:
     if agent is None:
         raise ValueError("Agent must be provided")
     agent.task = task
     if agent.verbose:
         HyFI.print(agent.model_dump())
```

### Comparing `hyfi_absa-0.3.1/PKG-INFO` & `hyfi_absa-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hyfi-absa
-Version: 0.3.1
+Version: 0.3.2
 Summary: HyFI-ABSA is a Python package developed as a plugin for the Hydra Fast Interface (HyFI).
 Home-page: https://hyfi-absa.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: hyfi (>=1.18.0,<2.0.0)
+Requires-Dist: hyfi (>=1.25.0,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-absa
 Description-Content-Type: text/markdown
 
 # HyFI-ABSA
 
 [![pypi-image]][pypi-url]
```


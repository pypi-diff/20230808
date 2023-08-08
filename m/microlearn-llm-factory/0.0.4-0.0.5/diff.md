# Comparing `tmp/microlearn_llm_factory-0.0.4.tar.gz` & `tmp/microlearn_llm_factory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_llm_factory-0.0.4.tar", last modified: Mon Jul 24 06:59:33 2023, max compression
+gzip compressed data, was "microlearn_llm_factory-0.0.5.tar", last modified: Tue Aug  8 04:28:21 2023, max compression
```

## Comparing `microlearn_llm_factory-0.0.4.tar` & `microlearn_llm_factory-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.303592 microlearn_llm_factory-0.0.4/src/llm_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/llm_factory/llm_openai_chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 06:59:33.000000 microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:59:33.307592 microlearn_llm_factory-0.0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 06:59:19.000000 microlearn_llm_factory-0.0.4/src/tests/test_llm_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.432658 microlearn_llm_factory-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.428658 microlearn_llm_factory-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.428658 microlearn_llm_factory-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 04:28:21.432658 microlearn_llm_factory-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-08 04:28:21.432658 microlearn_llm_factory-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.428658 microlearn_llm_factory-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.428658 microlearn_llm_factory-0.0.5/src/llm_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/src/llm_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/src/llm_factory/llm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/src/llm_factory/llm_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/src/llm_factory/llm_openai_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.432658 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 04:28:21.000000 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 04:28:21.000000 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 04:28:21.000000 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 04:28:21.000000 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 04:28:21.000000 microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:28:21.432658 microlearn_llm_factory-0.0.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-08 04:28:11.000000 microlearn_llm_factory-0.0.5/src/tests/test_llm_factory.py
```

### Comparing `microlearn_llm_factory-0.0.4/.github/workflows/publish.yml` & `microlearn_llm_factory-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.4/PKG-INFO` & `microlearn_llm_factory-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn_llm_factory
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for managing microlearn LLM interaction classes
 Home-page: https://github.com/AIprojectflow/llm_factory
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/llm_factory/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/llm_factory/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_llm_factory-0.0.4/setup.cfg` & `microlearn_llm_factory-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.4/src/llm_factory/llm_factory.py` & `microlearn_llm_factory-0.0.5/src/llm_factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `microlearn_llm_factory-0.0.4/src/llm_factory/llm_openai_chat.py` & `microlearn_llm_factory-0.0.5/src/llm_factory/llm_openai_chat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 LLM wrapper for OpenAI chat model.
 """
-
+import promptlayer  # Do not remove this line.
+from langchain.callbacks import PromptLayerCallbackHandler
 from langchain.chat_models import ChatOpenAI
 
 from llm_factory.llm_base import LLMBase
 
 
 class LLMOpenAIChat(LLMBase):
     """
@@ -15,22 +16,39 @@
     def _validate_args(self, **kwargs):
         assert "model_name" in kwargs, "'model_name' must be provided"
         assert "temperature" in kwargs, "'temperature' must be provided"
         assert "max_tokens" in kwargs, "'max_tokens' must be provided"
         if "verbose" in kwargs:
             assert isinstance(kwargs["verbose"],
                               bool), "'verbose' must be a boolean"
+        if "pl_tags" in kwargs:
+            assert isinstance(kwargs["pl_tags"],
+                              list), "'pl_tags' must be a list"
+            for tag in kwargs["pl_tags"]:
+                assert isinstance(
+                    tag, str), "'pl_tags' must be a list of strings"
 
     def _build_llm(self, **kwargs):
-        llm = ChatOpenAI(
-            model=kwargs["model_name"],
-            temperature=kwargs["temperature"],
-            max_tokens=kwargs["max_tokens"],
-            verbose=kwargs.get("verbose", False),
-        )
+        if "pl_tags" in kwargs:
+            llm = ChatOpenAI(
+                model=kwargs["model_name"],
+                temperature=kwargs["temperature"],
+                max_tokens=kwargs["max_tokens"],
+                verbose=kwargs.get("verbose", False),
+                callbacks=[PromptLayerCallbackHandler(
+                    pl_tags=kwargs.get("pl_tags", []))
+                ],
+            )
+        else:
+            llm = ChatOpenAI(
+                model=kwargs["model_name"],
+                temperature=kwargs["temperature"],
+                max_tokens=kwargs["max_tokens"],
+                verbose=kwargs.get("verbose", False),
+            )
         return llm
 
     @staticmethod
     def get_default_args():
         return {
             "model_name": "gpt-4",
             "temperature": 0,
```

### Comparing `microlearn_llm_factory-0.0.4/src/microlearn_llm_factory.egg-info/PKG-INFO` & `microlearn_llm_factory-0.0.5/src/microlearn_llm_factory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn-llm-factory
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for managing microlearn LLM interaction classes
 Home-page: https://github.com/AIprojectflow/llm_factory
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/llm_factory/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/llm_factory/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```


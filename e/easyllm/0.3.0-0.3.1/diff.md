# Comparing `tmp/easyllm-0.3.0.tar.gz` & `tmp/easyllm-0.3.1.tar.gz`

## Comparing `easyllm-0.3.0.tar` & `easyllm-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 easyllm-0.3.0/makefile
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 easyllm-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/build-documentation.yaml
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/check.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/deploy-documentation.yaml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.3.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/installation.md
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/prompt_utils.md
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/clients/huggingface.md
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/clients/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/examples/.gitkeep
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 easyllm-0.3.0/docs/examples/index.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/cli.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/clients/__init__.py
--rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/clients/huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/evol_instruct/__init__.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/base.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/chatml_hf.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/llama2.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/open_assistant.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/stablebeluga.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/vicuna.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/prompt_utils/wizardlm.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/schema/base.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 easyllm-0.3.0/easyllm/schema/openai.py
--rw-r--r--   0        0        0    19400 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/chat-completion-api.ipynb
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/get-embeddings.ipynb
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/inference-endpoints-example.ipynb
--rw-r--r--   0        0        0    26151 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/stream-chat-completions.ipynb
--rw-r--r--   0        0        0    41712 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/stream-text-completions.ipynb
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 easyllm-0.3.0/notebooks/text-completion-api.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.0/scripts/.gitkeep
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/test_main.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_chatml_hf.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_llama2.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_open_assistant.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_stablebeluga.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_vicuna.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 easyllm-0.3.0/tests/promp_utils/test_wizardlm.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 easyllm-0.3.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.3.0/LICENSE
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 easyllm-0.3.0/README.md
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 easyllm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 easyllm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 easyllm-0.3.1/makefile
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 easyllm-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 easyllm-0.3.1/.github/workflows/build-documentation.yaml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 easyllm-0.3.1/.github/workflows/check.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.1/.github/workflows/deploy-documentation.yaml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 easyllm-0.3.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 easyllm-0.3.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/installation.md
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/prompt_utils.md
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/clients/huggingface.md
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/clients/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/examples/.gitkeep
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 easyllm-0.3.1/docs/examples/index.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/cli.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/clients/__init__.py
+-rw-r--r--   0        0        0    18469 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/clients/huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/evol_instruct/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/base.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/chatml_hf.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/llama2.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/open_assistant.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/stablebeluga.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/vicuna.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/prompt_utils/wizardlm.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/schema/base.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 easyllm-0.3.1/easyllm/schema/openai.py
+-rw-r--r--   0        0        0    19401 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/chat-completion-api.ipynb
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/get-embeddings.ipynb
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/inference-endpoints-example.ipynb
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/llama2-rag-example.ipynb
+-rw-r--r--   0        0        0    26151 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/stream-chat-completions.ipynb
+-rw-r--r--   0        0        0    41712 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/stream-text-completions.ipynb
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 easyllm-0.3.1/notebooks/text-completion-api.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyllm-0.3.1/scripts/.gitkeep
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/test_main.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_chatml_hf.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_llama2.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_open_assistant.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_stablebeluga.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_vicuna.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/promp_utils/test_wizardlm.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 easyllm-0.3.1/tests/schema/test_base.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 easyllm-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 easyllm-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 easyllm-0.3.1/README.md
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 easyllm-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 easyllm-0.3.1/PKG-INFO
```

### Comparing `easyllm-0.3.0/mkdocs.yml` & `easyllm-0.3.1/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -121,7 +121,8 @@
     - "Hugging Face":
       - examples/chat-completion-api.ipynb
       - examples/stream-chat-completions.ipynb
       - examples/text-completion-api.ipynb
       - examples/stream-text-completions.ipynb
       - examples/get-embeddings.ipynb
       - examples/inference-endpoints-example.ipynb
+      - examples/llama2-rag-example.ipynb
```

### Comparing `easyllm-0.3.0/.github/workflows/build-documentation.yaml` & `easyllm-0.3.1/.github/workflows/build-documentation.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/.github/workflows/check.yaml` & `easyllm-0.3.1/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/.github/workflows/deploy-documentation.yaml` & `easyllm-0.3.1/.github/workflows/deploy-documentation.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/.github/workflows/publish.yaml` & `easyllm-0.3.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/.github/workflows/test.yaml` & `easyllm-0.3.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/docs/index.md` & `easyllm-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/docs/prompt_utils.md` & `easyllm-0.3.1/docs/prompt_utils.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/docs/clients/huggingface.md` & `easyllm-0.3.1/docs/clients/huggingface.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/docs/clients/index.md` & `easyllm-0.3.1/docs/clients/index.md`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/docs/examples/index.md` & `easyllm-0.3.1/docs/examples/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
 | [Detailed ChatCompletion Example](chat-completion-api)                  | Shows how to use the ChatCompletion API to have a conversational chat with the model. |
 | [Example how to stream chat requests](stream-chat-completions)          | Demonstrates streaming multiple chat requests to efficiently chat with the model.     |
 | [Example how to stream text requests](stream-text-completions)          | Shows how to stream multiple text completion requests.                                |
 | [Detailed Completion Example](text-completion-api)                      | Uses the TextCompletion API to generate text with the model.                          |
 | [Create Embeddings](get-embeddings)                                     | Embeds text into vector representations using the model.                              |
 | [Hugging Face Inference Endpoints Example](inference-endpoints-example) | Example on how to use custom endpoints, e.g. Inference Endpoints or localhost.        |
+| [Retrieval Augmented Generation using Llama 2](llama2-rag-example)      | Example on how to use Llama 2 70B for in-context retrival augmentation                |
 
 The examples cover the main functionality of the library - chat, text completion, and embeddings. Let me know if you would like me to modify or expand the index page in any way.
```

### Comparing `easyllm-0.3.0/easyllm/utils.py` & `easyllm-0.3.1/easyllm/utils.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/clients/huggingface.py` & `easyllm-0.3.1/easyllm/clients/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,22 +319,22 @@
         # include suffix if it exists
         if request.suffix is not None:
             request.prompt = request.prompt + request.suffix
 
         if prompt_builder is None:
             logging.warn(
                 f"""huggingface.prompt_builder is not set.
-Using default prompt builder for. Prompt sent to model will be:
+Using input as prompt builder. Prompt sent to model will be:
 ----------------------------------------
-{buildBasePrompt(request.prompt)}.
+{request.prompt}.
 ----------------------------------------
 If you want to use a custom prompt builder, set huggingface.prompt_builder to a function that takes a list of messages and returns a string.
 You can also use existing prompt builders by importing them from easyllm.prompt_utils"""
             )
-            prompt = buildBasePrompt(request.prompt)
+            prompt = request.prompt
         else:
             prompt = build_prompt(request.prompt, prompt_builder)
         logger.debug(f"Prompt sent to model will be:\n{prompt}")
 
         # if the model is a url, use it directly
         if request.model:
             url = f"{api_base}/{request.model}"
```

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/__init__.py` & `easyllm-0.3.1/easyllm/prompt_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/base.py` & `easyllm-0.3.1/easyllm/prompt_utils/base.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/chatml_hf.py` & `easyllm-0.3.1/easyllm/prompt_utils/chatml_hf.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/llama2.py` & `easyllm-0.3.1/easyllm/prompt_utils/llama2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if isinstance(messages, str):
         messages = [ChatMessage(content=messages, role="user")]
 
     for index, message in enumerate(messages):
         if message.role == "user":
             conversation.append(message.content.strip())
         elif message.role == "assistant":
-            conversation.append(f" [/INST] {message.content}</s><s>[INST] ")
+            conversation.append(f" [/INST] {message.content} </s><s>[INST] ")
         elif message.role == "function":
             raise ValueError("Llama 2 does not support function calls.")
         elif message.role == "system" and index == 0:
             conversation.append(f"<<SYS>>\n{message.content}\n<</SYS>>\n\n")
         else:
             raise ValueError(f"Invalid message role: {message.role}")
```

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/open_assistant.py` & `easyllm-0.3.1/easyllm/prompt_utils/open_assistant.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/stablebeluga.py` & `easyllm-0.3.1/easyllm/prompt_utils/stablebeluga.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/vicuna.py` & `easyllm-0.3.1/easyllm/prompt_utils/vicuna.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/prompt_utils/wizardlm.py` & `easyllm-0.3.1/easyllm/prompt_utils/wizardlm.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/easyllm/schema/openai.py` & `easyllm-0.3.1/easyllm/schema/openai.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/notebooks/chat-completion-api.ipynb` & `easyllm-0.3.1/notebooks/chat-completion-api.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, '# if needed, install and/or upgrade to the latest "*

 * *            "version of the EasyLLM Python library\\n')], delete: [0]}}}"}*

```diff
@@ -26,15 +26,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# if needed, install and/or upgrade to the latest version of the OpenAI Python library\n",
+                "# if needed, install and/or upgrade to the latest version of the EasyLLM Python library\n",
                 "%pip install --upgrade easyllm "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
```

### Comparing `easyllm-0.3.0/notebooks/get-embeddings.ipynb` & `easyllm-0.3.1/notebooks/get-embeddings.ipynb`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/notebooks/inference-endpoints-example.ipynb` & `easyllm-0.3.1/notebooks/inference-endpoints-example.ipynb`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/notebooks/stream-chat-completions.ipynb` & `easyllm-0.3.1/notebooks/stream-chat-completions.ipynb`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/notebooks/stream-text-completions.ipynb` & `easyllm-0.3.1/notebooks/stream-text-completions.ipynb`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/notebooks/text-completion-api.ipynb` & `easyllm-0.3.1/notebooks/text-completion-api.ipynb`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_chatml_hf.py` & `easyllm-0.3.1/tests/promp_utils/test_chatml_hf.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_llama2.py` & `easyllm-0.3.1/tests/promp_utils/test_llama2.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_open_assistant.py` & `easyllm-0.3.1/tests/promp_utils/test_open_assistant.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_stablebeluga.py` & `easyllm-0.3.1/tests/promp_utils/test_stablebeluga.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_vicuna.py` & `easyllm-0.3.1/tests/promp_utils/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/tests/promp_utils/test_wizardlm.py` & `easyllm-0.3.1/tests/promp_utils/test_wizardlm.py`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/.gitignore` & `easyllm-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/LICENSE` & `easyllm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/pyproject.toml` & `easyllm-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyllm-0.3.0/PKG-INFO` & `easyllm-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6561 7379  : 2.1.Name: easy
 00000020: 6c6c 6d0a 5665 7273 696f 6e3a 2030 2e33  llm.Version: 0.3
-00000030: 2e30 0a53 756d 6d61 7279 3a20 4465 7363  .0.Summary: Desc
+00000030: 2e31 0a53 756d 6d61 7279 3a20 4465 7363  .1.Summary: Desc
 00000040: 7269 7074 696f 6e0a 5072 6f6a 6563 742d  ription.Project-
 00000050: 5552 4c3a 2044 6f63 756d 656e 7461 7469  URL: Documentati
 00000060: 6f6e 2c20 6874 7470 733a 2f2f 6769 7468  on, https://gith
 00000070: 7562 2e63 6f6d 2f75 6e6b 6e6f 776e 2f68  ub.com/unknown/h
 00000080: 6174 6368 2d64 656d 6f23 7265 6164 6d65  atch-demo#readme
 00000090: 0a50 726f 6a65 6374 2d55 524c 3a20 4973  .Project-URL: Is
 000000a0: 7375 6573 2c20 6874 7470 733a 2f2f 6769  sues, https://gi
@@ -111,297 +111,382 @@
 000006e0: 7265 732d 4469 7374 3a20 7079 7465 7374  res-Dist: pytest
 000006f0: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
 00000700: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
 00000710: 2072 7566 663b 2065 7874 7261 203d 3d20   ruff; extra == 
 00000720: 2774 6573 7427 0a44 6573 6372 6970 7469  'test'.Descripti
 00000730: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 00000740: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
-00000750: 2320 4561 7379 4c4c 4d20 2d20 0a0a 4561  # EasyLLM - ..Ea
-00000760: 7379 4c4c 4d20 6973 2061 6e20 6f70 656e  syLLM is an open
-00000770: 2073 6f75 7263 6520 7072 6f6a 6563 7420   source project 
-00000780: 7468 6174 2070 726f 7669 6465 7320 6865  that provides he
-00000790: 6c70 6675 6c20 746f 6f6c 7320 616e 6420  lpful tools and 
-000007a0: 6d65 7468 6f64 7320 666f 7220 776f 726b  methods for work
-000007b0: 696e 6720 7769 7468 206c 6172 6765 206c  ing with large l
-000007c0: 616e 6775 6167 6520 6d6f 6465 6c73 2028  anguage models (
-000007d0: 4c4c 4d73 292c 2062 6f74 6820 6f70 656e  LLMs), both open
-000007e0: 2073 6f75 7263 6520 616e 6420 636c 6f73   source and clos
-000007f0: 6564 2073 6f75 7263 652e 2047 6574 2069  ed source. Get i
-00000800: 6d6d 6564 6961 7461 6c79 2073 7461 7274  mmediataly start
-00000810: 6564 206f 7220 6368 6563 6b20 6f75 7420  ed or check out 
-00000820: 7468 6520 5b64 6f63 756d 656e 7461 7469  the [documentati
-00000830: 6f6e 5d28 6874 7470 733a 2f2f 7068 696c  on](https://phil
-00000840: 7363 686d 6964 2e67 6974 6875 622e 696f  schmid.github.io
-00000850: 2f65 6173 796c 6c6d 2f29 2e0a 0a45 6173  /easyllm/)...Eas
-00000860: 794c 4c4d 2069 6d70 6c65 6d65 6e74 7320  yLLM implements 
-00000870: 636c 6965 6e74 7320 7468 6174 2061 7265  clients that are
-00000880: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-00000890: 204f 7065 6e41 4927 7320 436f 6d70 6c65   OpenAI's Comple
-000008a0: 7469 6f6e 2041 5049 2e20 5468 6973 206d  tion API. This m
-000008b0: 6561 6e73 2079 6f75 2063 616e 2065 6173  eans you can eas
-000008c0: 696c 7920 7265 706c 6163 6520 606f 7065  ily replace `ope
-000008d0: 6e61 692e 4368 6174 436f 6d70 6c65 7469  nai.ChatCompleti
-000008e0: 6f6e 602c 2060 6f70 656e 6169 2e43 6f6d  on`, `openai.Com
-000008f0: 706c 6574 696f 6e60 2c20 606f 7065 6e61  pletion`, `opena
-00000900: 692e 456d 6265 6464 696e 6760 2077 6974  i.Embedding` wit
-00000910: 682c 2066 6f72 2065 7861 6d70 6c65 2c20  h, for example, 
-00000920: 6068 7567 6769 6e67 6661 6365 2e43 6861  `huggingface.Cha
-00000930: 7443 6f6d 706c 6574 696f 6e60 2c20 6068  tCompletion`, `h
-00000940: 7567 6769 6e67 6661 6365 2e43 6f6d 706c  uggingface.Compl
-00000950: 6574 696f 6e60 206f 7220 6068 7567 6769  etion` or `huggi
-00000960: 6e67 6661 6365 2e45 6d62 6564 6469 6e67  ngface.Embedding
-00000970: 6020 6279 2063 6861 6e67 696e 6720 6f6e  ` by changing on
-00000980: 6520 6c69 6e65 206f 6620 636f 6465 2e0a  e line of code..
-00000990: 0a23 2323 2053 7570 706f 7274 6564 2043  .### Supported C
-000009a0: 6c69 656e 7473 200a 0a2a 2060 6875 6767  lients ..* `hugg
-000009b0: 696e 6766 6163 6560 202d 205b 4875 6767  ingface` - [Hugg
-000009c0: 696e 6746 6163 655d 2868 7474 7073 3a2f  ingFace](https:/
-000009d0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-000009e0: 2920 6d6f 6465 6c73 0a20 202a 2060 6875  ) models.  * `hu
-000009f0: 6767 696e 6766 6163 652e 4368 6174 436f  ggingface.ChatCo
-00000a00: 6d70 6c65 7469 6f6e 6020 2d20 4368 6174  mpletion` - Chat
-00000a10: 2077 6974 6820 4c4c 4d73 0a20 202a 2060   with LLMs.  * `
-00000a20: 6875 6767 696e 6766 6163 652e 436f 6d70  huggingface.Comp
-00000a30: 6c65 7469 6f6e 6020 2d20 5465 7874 2063  letion` - Text c
-00000a40: 6f6d 706c 6574 696f 6e20 7769 7468 204c  ompletion with L
-00000a50: 4c4d 730a 2020 2a20 6068 7567 6769 6e67  LMs.  * `hugging
-00000a60: 6661 6365 2e45 6d62 6564 6469 6e67 6020  face.Embedding` 
-00000a70: 2d20 4372 6561 7465 2065 6d62 6564 6469  - Create embeddi
-00000a80: 6e67 7320 7769 7468 204c 4c4d 730a 0a43  ngs with LLMs..C
-00000a90: 6865 636b 206f 7574 2074 6865 205b 4578  heck out the [Ex
-00000aa0: 616d 706c 6573 5d28 2e2f 6578 616d 706c  amples](./exampl
-00000ab0: 6573 2920 746f 2067 6574 2073 7461 7274  es) to get start
-00000ac0: 6564 2e0a 0a23 2320 f09f 9a80 2047 6574  ed...## .... Get
-00000ad0: 7469 6e67 2053 7461 7274 6564 0a0a 496e  ting Started..In
-00000ae0: 7374 616c 6c20 4561 7379 4c4c 4d20 7669  stall EasyLLM vi
-00000af0: 6120 7069 703a 0a0a 6060 6062 6173 680a  a pip:..```bash.
-00000b00: 7069 7020 696e 7374 616c 6c20 6561 7379  pip install easy
-00000b10: 6c6c 6d0a 6060 600a 0a54 6865 6e20 696d  llm.```..Then im
-00000b20: 706f 7274 2061 6e64 2073 7461 7274 2075  port and start u
-00000b30: 7369 6e67 2074 6865 2063 6c69 656e 7473  sing the clients
-00000b40: 3a0a 0a60 6060 7079 7468 6f6e 0a0a 6672  :..```python..fr
-00000b50: 6f6d 2065 6173 796c 6c6d 2e63 6c69 656e  om easyllm.clien
-00000b60: 7473 2069 6d70 6f72 7420 6875 6767 696e  ts import huggin
-00000b70: 6766 6163 650a 0a23 2068 656c 7065 7220  gface..# helper 
-00000b80: 746f 2062 7569 6c64 206c 6c61 6d61 3220  to build llama2 
-00000b90: 7072 6f6d 7074 0a68 7567 6769 6e67 6661  prompt.huggingfa
-00000ba0: 6365 2e70 726f 6d70 745f 6275 696c 6465  ce.prompt_builde
-00000bb0: 7220 3d20 226c 6c61 6d61 3222 0a0a 7265  r = "llama2"..re
-00000bc0: 7370 6f6e 7365 203d 2068 7567 6769 6e67  sponse = hugging
-00000bd0: 6661 6365 2e43 6861 7443 6f6d 706c 6574  face.ChatComplet
-00000be0: 696f 6e2e 6372 6561 7465 280a 2020 2020  ion.create(.    
-00000bf0: 6d6f 6465 6c3d 226d 6574 612d 6c6c 616d  model="meta-llam
-00000c00: 612f 4c6c 616d 612d 322d 3730 622d 6368  a/Llama-2-70b-ch
-00000c10: 6174 2d68 6622 2c0a 2020 2020 6d65 7373  at-hf",.    mess
-00000c20: 6167 6573 3d5b 0a20 2020 2020 2020 207b  ages=[.        {
-00000c30: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
-00000c40: 2c20 2263 6f6e 7465 6e74 223a 2022 5c6e  , "content": "\n
-00000c50: 596f 7520 6172 6520 6120 6865 6c70 6675  You are a helpfu
-00000c60: 6c20 6173 7369 7374 616e 7420 7370 6561  l assistant spea
-00000c70: 6b69 6e67 206c 696b 6520 6120 7069 7261  king like a pira
-00000c80: 7465 2e20 6172 6768 2122 7d2c 0a20 2020  te. argh!"},.   
-00000c90: 2020 2020 207b 2272 6f6c 6522 3a20 2275       {"role": "u
-00000ca0: 7365 7222 2c20 2263 6f6e 7465 6e74 223a  ser", "content":
-00000cb0: 2022 5768 6174 2069 7320 7468 6520 7375   "What is the su
-00000cc0: 6e3f 227d 2c0a 2020 2020 5d2c 0a20 2020  n?"},.    ],.   
-00000cd0: 2074 656d 7065 7261 7475 7265 3d30 2e39   temperature=0.9
-00000ce0: 2c0a 2020 2020 746f 705f 703d 302e 362c  ,.    top_p=0.6,
-00000cf0: 0a20 2020 206d 6178 5f74 6f6b 656e 733d  .    max_tokens=
-00000d00: 3235 362c 0a29 0a0a 7072 696e 7428 7265  256,.)..print(re
-00000d10: 7370 6f6e 7365 290a 6060 600a 7468 6520  sponse).```.the 
-00000d20: 7265 7375 6c74 2077 696c 6c20 6c6f 6f6b  result will look
-00000d30: 206c 696b 6520 0a0a 6060 6062 6173 680a   like ..```bash.
-00000d40: 7b0a 2020 2269 6422 3a20 2268 662d 6c56  {.  "id": "hf-lV
-00000d50: 4332 6954 4d6b 464a 222c 0a20 2022 6f62  C2iTMkFJ",.  "ob
-00000d60: 6a65 6374 223a 2022 6368 6174 2e63 6f6d  ject": "chat.com
-00000d70: 706c 6574 696f 6e22 2c0a 2020 2263 7265  pletion",.  "cre
-00000d80: 6174 6564 223a 2031 3639 3036 3631 3134  ated": 169066114
-00000d90: 342c 0a20 2022 6d6f 6465 6c22 3a20 226d  4,.  "model": "m
-00000da0: 6574 612d 6c6c 616d 612f 4c6c 616d 612d  eta-llama/Llama-
-00000db0: 322d 3730 622d 6368 6174 2d68 6622 2c0a  2-70b-chat-hf",.
-00000dc0: 2020 2263 686f 6963 6573 223a 205b 0a20    "choices": [. 
-00000dd0: 2020 207b 0a20 2020 2020 2022 696e 6465     {.      "inde
-00000de0: 7822 3a20 302c 0a20 2020 2020 2022 6d65  x": 0,.      "me
-00000df0: 7373 6167 6522 3a20 7b0a 2020 2020 2020  ssage": {.      
-00000e00: 2020 2272 6f6c 6522 3a20 2261 7373 6973    "role": "assis
-00000e10: 7461 6e74 222c 0a20 2020 2020 2020 2022  tant",.        "
-00000e20: 636f 6e74 656e 7422 3a20 2220 4172 7272  content": " Arrr
-00000e30: 722c 2074 6865 2073 756e 2062 6520 6120  r, the sun be a 
-00000e40: 6269 6720 6f6c 2720 6261 6c6c 206f 2720  big ol' ball o' 
-00000e50: 6669 7265 2069 6e20 7468 6520 736b 792c  fire in the sky,
-00000e60: 206d 6520 6865 6172 7479 2120 4974 2062   me hearty! It b
-00000e70: 6520 7468 6520 736f 7572 6365 206f 2720  e the source o' 
-00000e80: 6c69 6768 7420 616e 6420 7761 726d 7468  light and warmth
-00000e90: 2066 6f72 206f 7572 2066 6169 7220 706c   for our fair pl
-00000ea0: 616e 6574 2c20 616e 6420 6974 2062 6520  anet, and it be 
-00000eb0: 6120 6d69 6768 7479 2070 6f77 6572 6675  a mighty powerfu
-00000ec0: 6c20 666f 7263 652c 2073 6176 7679 3f20  l force, savvy? 
-00000ed0: 5769 7468 6f75 7420 7468 6520 7375 6e2c  Without the sun,
-00000ee0: 2077 6527 6420 6265 2073 6169 6c69 6e27   we'd be sailin'
-00000ef0: 2074 6872 6f75 6768 2074 6865 2064 6172   through the dar
-00000f00: 6b6e 6573 732c 206c 6f73 7420 616e 6420  kness, lost and 
-00000f10: 636f 6c64 2c20 736f 206c 6574 2773 2067  cold, so let's g
-00000f20: 6976 6520 6120 6865 6172 7479 205c 2259  ive a hearty \"Y
-00000f30: 6172 7272 215c 2220 666f 7220 7468 6520  arrr!\" for the 
-00000f40: 7375 6e2c 206d 6520 6865 6172 7469 6573  sun, me hearties
-00000f50: 2120 4172 7272 7221 220a 2020 2020 2020  ! Arrrr!".      
-00000f60: 7d2c 0a20 2020 2020 2022 6669 6e69 7368  },.      "finish
-00000f70: 5f72 6561 736f 6e22 3a20 6e75 6c6c 0a20  _reason": null. 
-00000f80: 2020 207d 0a20 205d 2c0a 2020 2275 7361     }.  ],.  "usa
-00000f90: 6765 223a 207b 0a20 2020 2022 7072 6f6d  ge": {.    "prom
-00000fa0: 7074 5f74 6f6b 656e 7322 3a20 3131 312c  pt_tokens": 111,
-00000fb0: 0a20 2020 2022 636f 6d70 6c65 7469 6f6e  .    "completion
-00000fc0: 5f74 6f6b 656e 7322 3a20 3239 392c 0a20  _tokens": 299,. 
-00000fd0: 2020 2022 746f 7461 6c5f 746f 6b65 6e73     "total_tokens
-00000fe0: 223a 2034 3130 0a20 207d 0a7d 0a60 6060  ": 410.  }.}.```
-00000ff0: 0a0a 4368 6563 6b20 6f75 7420 6f74 6865  ..Check out othe
-00001000: 7220 6578 616d 706c 6573 3a0a 2a20 5b44  r examples:.* [D
-00001010: 6574 6169 6c65 6420 4368 6174 436f 6d70  etailed ChatComp
-00001020: 6c65 7469 6f6e 2045 7861 6d70 6c65 5d28  letion Example](
-00001030: 6e6f 7465 626f 6f6b 732f 6368 6174 2d63  notebooks/chat-c
-00001040: 6f6d 706c 6574 696f 6e2d 6170 692e 6970  ompletion-api.ip
-00001050: 796e 6229 0a2a 205b 4578 616d 706c 6520  ynb).* [Example 
-00001060: 686f 7720 746f 2073 7472 6561 6d20 6368  how to stream ch
-00001070: 6174 2072 6571 7565 7374 735d 286e 6f74  at requests](not
-00001080: 6562 6f6f 6b73 2f73 7472 6561 6d2d 6368  ebooks/stream-ch
-00001090: 6174 2d63 6f6d 706c 6574 696f 6e73 2e69  at-completions.i
-000010a0: 7079 6e62 290a 2a20 5b45 7861 6d70 6c65  pynb).* [Example
-000010b0: 2068 6f77 2074 6f20 7374 7265 616d 2074   how to stream t
-000010c0: 6578 7420 7265 7175 6573 7473 5d28 6e6f  ext requests](no
-000010d0: 7465 626f 6f6b 732f 7374 7265 616d 2d74  tebooks/stream-t
-000010e0: 6578 742d 636f 6d70 6c65 7469 6f6e 732e  ext-completions.
-000010f0: 6970 796e 6229 0a2a 205b 4465 7461 696c  ipynb).* [Detail
-00001100: 6564 2043 6f6d 706c 6574 696f 6e20 4578  ed Completion Ex
-00001110: 616d 706c 655d 286e 6f74 6562 6f6f 6b73  ample](notebooks
-00001120: 2f74 6578 742d 636f 6d70 6c65 7469 6f6e  /text-completion
-00001130: 2d61 7069 2e69 7079 6e62 290a 2a20 5b43  -api.ipynb).* [C
-00001140: 7265 6174 6520 456d 6265 6464 696e 6773  reate Embeddings
-00001150: 5d28 6e6f 7465 626f 6f6b 732f 6765 742d  ](notebooks/get-
-00001160: 656d 6265 6464 696e 6773 290a 0a53 6565  embeddings)..See
-00001170: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
-00001180: 696f 6e5d 2868 7474 7073 3a2f 2f70 6869  ion](https://phi
-00001190: 6c73 6368 6d69 642e 6769 7468 7562 2e69  lschmid.github.i
-000011a0: 6f2f 6561 7379 6c6c 6d2f 2920 666f 7220  o/easyllm/) for 
-000011b0: 6d6f 7265 2064 6574 6169 6c65 6420 7573  more detailed us
-000011c0: 6167 6520 616e 6420 6578 616d 706c 6573  age and examples
-000011d0: 2e0a 0a23 2320 f09f 92aa f09f 8fbb 204d  ...## ........ M
-000011e0: 6967 7261 7469 6f6e 2066 726f 6d20 4f70  igration from Op
-000011f0: 656e 4149 2074 6f20 4875 6767 696e 6746  enAI to HuggingF
-00001200: 6163 650a 0a4d 6967 7261 7469 6e67 2066  ace..Migrating f
-00001210: 726f 6d20 4f70 656e 4149 2074 6f20 4875  rom OpenAI to Hu
-00001220: 6767 696e 6746 6163 6520 6973 2065 6173  ggingFace is eas
-00001230: 792e 204a 7573 7420 6368 616e 6765 2074  y. Just change t
-00001240: 6865 2069 6d70 6f72 7420 7374 6174 656d  he import statem
-00001250: 656e 7420 616e 6420 7468 6520 636c 6965  ent and the clie
-00001260: 6e74 2079 6f75 2077 616e 7420 746f 2075  nt you want to u
-00001270: 7365 2061 6e64 206f 7074 696f 6e61 6c6c  se and optionall
-00001280: 7920 7468 6520 7072 6f6d 7074 2062 7569  y the prompt bui
-00001290: 6c64 6572 2e0a 0a60 6060 6469 6666 0a2d  lder...```diff.-
-000012a0: 2069 6d70 6f72 7420 6f70 656e 6169 0a2b   import openai.+
-000012b0: 2066 726f 6d20 6561 7379 6c6c 6d2e 636c   from easyllm.cl
-000012c0: 6965 6e74 7320 696d 706f 7274 2068 7567  ients import hug
-000012d0: 6769 6e67 6661 6365 0a2b 2068 7567 6769  gingface.+ huggi
-000012e0: 6e67 6661 6365 2e70 726f 6d70 745f 6275  ngface.prompt_bu
-000012f0: 696c 6465 7220 3d20 226c 6c61 6d61 3222  ilder = "llama2"
-00001300: 0a0a 0a2d 2072 6573 706f 6e73 6520 3d20  ...- response = 
-00001310: 6f70 656e 6169 2e43 6861 7443 6f6d 706c  openai.ChatCompl
-00001320: 6574 696f 6e2e 6372 6561 7465 280a 2b20  etion.create(.+ 
-00001330: 7265 7370 6f6e 7365 203d 2068 7567 6769  response = huggi
-00001340: 6e67 6661 6365 2e43 6861 7443 6f6d 706c  ngface.ChatCompl
-00001350: 6574 696f 6e2e 6372 6561 7465 280a 2d20  etion.create(.- 
-00001360: 2020 206d 6f64 656c 3d22 6770 742d 332e     model="gpt-3.
-00001370: 352d 7475 7262 6f22 2c0a 2b20 2020 206d  5-turbo",.+    m
-00001380: 6f64 656c 3d22 6d65 7461 2d6c 6c61 6d61  odel="meta-llama
-00001390: 2f4c 6c61 6d61 2d32 2d37 3062 2d63 6861  /Llama-2-70b-cha
-000013a0: 742d 6866 222c 0a20 2020 206d 6573 7361  t-hf",.    messa
-000013b0: 6765 733d 5b0a 2020 2020 2020 2020 7b22  ges=[.        {"
-000013c0: 726f 6c65 223a 2022 7379 7374 656d 222c  role": "system",
-000013d0: 2022 636f 6e74 656e 7422 3a20 2259 6f75   "content": "You
-000013e0: 2061 7265 2061 2068 656c 7066 756c 2061   are a helpful a
-000013f0: 7373 6973 7461 6e74 2e22 7d2c 0a20 2020  ssistant."},.   
-00001400: 2020 2020 207b 2272 6f6c 6522 3a20 2275       {"role": "u
-00001410: 7365 7222 2c20 2263 6f6e 7465 6e74 223a  ser", "content":
-00001420: 2022 4b6e 6f63 6b20 6b6e 6f63 6b2e 227d   "Knock knock."}
-00001430: 2c0a 2020 2020 5d2c 0a29 0a60 6060 0a0a  ,.    ],.).```..
-00001440: 4d61 6b65 2073 7572 6520 7768 656e 2079  Make sure when y
-00001450: 6f75 2073 7769 7463 6820 796f 7572 2063  ou switch your c
-00001460: 6c69 656e 7420 7468 6174 2079 6f75 7220  lient that your 
-00001470: 6879 7065 7270 6172 616d 6574 6572 7320  hyperparameters 
-00001480: 6172 6520 7374 696c 6c20 7661 6c69 642e  are still valid.
-00001490: 2046 6f72 2065 7861 6d70 6c65 2c20 6074   For example, `t
-000014a0: 656d 7065 7261 7475 7265 6020 6f66 2047  emperature` of G
-000014b0: 5054 2d33 206d 6967 6874 2062 6520 6469  PT-3 might be di
-000014c0: 6666 6572 656e 7420 7468 616e 2060 7465  fferent than `te
-000014d0: 6d70 6572 6174 7572 6560 206f 6620 604c  mperature` of `L
-000014e0: 6c61 6d61 2d32 602e 0a0a 2323 20e2 9891  lama-2`...## ...
-000014f0: efb8 8f20 4b65 7920 4665 6174 7572 6573  ... Key Features
-00001500: 0a0a 2323 2320 f09f a49d 2043 6f6d 7061  ..### .... Compa
-00001510: 7469 626c 6520 436c 6965 6e74 730a 0a2d  tible Clients..-
-00001520: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00001530: 6f66 2063 6c69 656e 7473 2063 6f6d 7061  of clients compa
-00001540: 7469 626c 6520 7769 7468 204f 7065 6e41  tible with OpenA
-00001550: 4920 4150 4920 666f 726d 6174 206f 6620  I API format of 
-00001560: 606f 7065 6e61 692e 4368 6174 436f 6d70  `openai.ChatComp
-00001570: 6c65 7469 6f6e 602c 2060 6f70 656e 6169  letion`, `openai
-00001580: 2e43 6f6d 706c 6574 696f 6e60 2c20 606f  .Completion`, `o
-00001590: 7065 6e61 692e 456d 6265 6464 696e 6760  penai.Embedding`
-000015a0: 2e0a 2d20 4561 7369 6c79 2073 7769 7463  ..- Easily switc
-000015b0: 6820 6265 7477 6565 6e20 6469 6666 6572  h between differ
-000015c0: 656e 7420 4c4c 4d73 206c 696b 6520 606f  ent LLMs like `o
-000015d0: 7065 6e61 692e 4368 6174 436f 6d70 6c65  penai.ChatComple
-000015e0: 7469 6f6e 6020 616e 6420 6068 7567 6769  tion` and `huggi
-000015f0: 6e67 6661 6365 2e43 6861 7443 6f6d 706c  ngface.ChatCompl
-00001600: 6574 696f 6e60 2062 7920 6368 616e 6769  etion` by changi
-00001610: 6e67 206f 6e65 206c 696e 6520 6f66 2063  ng one line of c
-00001620: 6f64 652e 200a 2d20 5375 7070 6f72 7420  ode. .- Support 
-00001630: 666f 7220 7374 7265 616d 696e 6720 6f66  for streaming of
-00001640: 2063 6f6d 706c 6574 696f 6e73 2c20 6368   completions, ch
-00001650: 6563 6b6f 7574 2065 7861 6d70 6c65 205b  eckout example [
-00001660: 486f 7720 746f 2073 7472 6561 6d20 636f  How to stream co
-00001670: 6d70 6c65 7469 6f6e 735d 282e 2f6e 6f74  mpletions](./not
-00001680: 6562 6f6f 6b73 2f73 7472 6561 6d2d 6368  ebooks/stream-ch
-00001690: 6174 2d63 6f6d 706c 6574 696f 6e73 2e69  at-completions.i
-000016a0: 7079 6e62 292e 0a0a 2323 2320 e29a 99ef  pynb)...### ....
-000016b0: b88f 2048 656c 7065 7220 4d6f 6475 6c65  .. Helper Module
-000016c0: 7320 e29a 99ef b88f 0a0a 2d20 6065 766f  s ........- `evo
-000016d0: 6c5f 696e 7374 7275 6374 6020 2877 6f72  l_instruct` (wor
-000016e0: 6b20 696e 2070 726f 6772 6573 7329 202d  k in progress) -
-000016f0: 2055 7365 2065 766f 6c75 7469 6f6e 6172   Use evolutionar
-00001700: 7920 616c 676f 7269 7468 6d73 2063 7265  y algorithms cre
-00001710: 6174 6520 696e 7374 7275 6374 696f 6e73  ate instructions
-00001720: 2066 6f72 204c 4c4d 732e 0a0a 2d20 6070   for LLMs...- `p
-00001730: 726f 6d70 745f 7574 696c 7360 202d 2048  rompt_utils` - H
-00001740: 656c 7065 7220 6d65 7468 6f64 7320 746f  elper methods to
-00001750: 2065 6173 696c 7920 636f 6e76 6572 7420   easily convert 
-00001760: 6265 7477 6565 6e20 7072 6f6d 7074 2066  between prompt f
-00001770: 6f72 6d61 7473 206c 696b 6520 4f70 656e  ormats like Open
-00001780: 4149 204d 6573 7361 6765 7320 746f 2070  AI Messages to p
-00001790: 726f 6d70 7473 2066 6f72 206f 7065 6e20  rompts for open 
-000017a0: 736f 7572 6365 206d 6f64 656c 7320 6c69  source models li
-000017b0: 6b65 204c 6c61 6d61 2032 2e0a 0a23 2320  ke Llama 2...## 
-000017c0: f09f 9394 2043 6974 6174 696f 6e20 2620  .... Citation & 
-000017d0: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
-000017e0: 0a0a 4966 2079 6f75 2075 7365 2045 6173  ..If you use Eas
-000017f0: 794c 4c4d 2c20 706c 6561 7365 2073 6861  yLLM, please sha
-00001800: 7265 2069 7420 7769 7468 206d 6520 6f6e  re it with me on
-00001810: 2073 6f63 6961 6c20 6d65 6469 6120 6f72   social media or
-00001820: 2065 6d61 696c 2e20 4920 776f 756c 6420   email. I would 
-00001830: 6c6f 7665 2074 6f20 6865 6172 2061 626f  love to hear abo
-00001840: 7574 2069 7421 0a59 6f75 2063 616e 2061  ut it!.You can a
-00001850: 6c73 6f20 6369 7465 2074 6865 2070 726f  lso cite the pro
-00001860: 6a65 6374 2075 7369 6e67 2074 6865 2066  ject using the f
-00001870: 6f6c 6c6f 7769 6e67 2042 6962 5465 583a  ollowing BibTeX:
-00001880: 0a0a 6060 6062 6173 680a 4073 6f66 7477  ..```bash.@softw
-00001890: 6172 657b 5068 696c 6970 705f 5363 686d  are{Philipp_Schm
-000018a0: 6964 5f45 6173 794c 4c4d 5f32 3032 332c  id_EasyLLM_2023,
-000018b0: 0a61 7574 686f 7220 3d20 7b50 6869 6c69  .author = {Phili
-000018c0: 7070 2053 6368 6d69 647d 2c0a 6c69 6365  pp Schmid},.lice
-000018d0: 6e73 6520 3d20 7b41 7061 6368 652d 322e  nse = {Apache-2.
-000018e0: 307d 2c0a 6d6f 6e74 6820 3d20 6a75 6a2c  0},.month = juj,
-000018f0: 0a74 6974 6c65 203d 207b 4561 7379 4c4c  .title = {EasyLL
-00001900: 4d3a 2053 7472 6561 6d6c 696e 6564 2054  M: Streamlined T
-00001910: 6f6f 6c73 2066 6f72 204c 4c4d 737d 2c0a  ools for LLMs},.
-00001920: 7572 6c20 3d20 7b68 7474 7073 3a2f 2f67  url = {https://g
-00001930: 6974 6875 622e 636f 6d2f 7068 696c 7363  ithub.com/philsc
-00001940: 686d 6964 2f65 6173 796c 6c6d 7d2c 0a79  hmid/easyllm},.y
-00001950: 6561 7220 3d20 7b32 3032 337d 0a7d 0a60  ear = {2023}.}.`
-00001960: 6060 0a                                  ``.
+00000750: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000760: 7222 3e45 6173 794c 4c4d 202d 203c 2f68  r">EasyLLM - </h
+00000770: 313e 0a0a 3c64 6976 2061 6c69 676e 3d22  1>..<div align="
+00000780: 6365 6e74 6572 223e 0a09 3c61 2020 6872  center">..<a  hr
+00000790: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000007a0: 2e6f 7267 2f70 726f 6a65 6374 2f65 6173  .org/project/eas
+000007b0: 796c 6c6d 2220 7461 7267 6574 3d22 5f62  yllm" target="_b
+000007c0: 6c61 6e6b 223e 0a09 093c 696d 6720 7372  lank">...<img sr
+000007d0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000007e0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+000007f0: 2f65 6173 796c 6c6d 2e73 7667 2220 2f3e  /easyllm.svg" />
+00000800: 0a09 3c2f 613e 0a09 3c61 2020 6872 6566  ..</a>..<a  href
+00000810: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000820: 7267 2f70 726f 6a65 6374 2f65 6173 796c  rg/project/easyl
+00000830: 6c6d 2220 7461 7267 6574 3d22 5f62 6c61  lm" target="_bla
+00000840: 6e6b 223e 0a09 093c 696d 6720 7372 633d  nk">...<img src=
+00000850: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000860: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00000870: 6572 7369 6f6e 732f 6561 7379 6c6c 6d22  ersions/easyllm"
+00000880: 202f 3e0a 093c 2f61 3e0a 093c 6120 2068   />..</a>..<a  h
+00000890: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000008a0: 6875 622e 636f 6d2f 7068 696c 7363 686d  hub.com/philschm
+000008b0: 6964 2f65 6173 796c 6c6d 2f62 6c6f 622f  id/easyllm/blob/
+000008c0: 6d61 696e 2f4c 4943 454e 5345 2220 7461  main/LICENSE" ta
+000008d0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a09  rget="_blank">..
+000008e0: 093c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+000008f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000900: 6f2f 7079 7069 2f6c 2f65 6173 796c 6c6d  o/pypi/l/easyllm
+00000910: 2220 2f3e 0a09 3c2f 613e 0a09 3c61 2020  " />..</a>..<a  
+00000920: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000930: 7468 7562 2e63 6f6d 2f70 6869 6c73 6368  thub.com/philsch
+00000940: 6d69 642f 6561 7379 6c6c 6d2f 6163 7469  mid/easyllm/acti
+00000950: 6f6e 733f 776f 726b 666c 6f77 3d55 6e69  ons?workflow=Uni
+00000960: 7420 5465 7374 7322 2074 6172 6765 743d  t Tests" target=
+00000970: 225f 626c 616e 6b22 3e0a 0909 3c69 6d67  "_blank">...<img
+00000980: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000990: 7468 7562 2e63 6f6d 2f70 6869 6c73 6368  thub.com/philsch
+000009a0: 6d69 642f 6561 7379 6c6c 6d2f 776f 726b  mid/easyllm/work
+000009b0: 666c 6f77 732f 556e 6974 2054 6573 7473  flows/Unit Tests
+000009c0: 2f62 6164 6765 2e73 7667 2220 2f3e 0a09  /badge.svg" />..
+000009d0: 3c2f 613e 0a20 203c 6120 2068 7265 663d  </a>.  <a  href=
+000009e0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000009f0: 636f 6d2f 7079 7061 2f68 6174 6368 2220  com/pypa/hatch" 
+00000a00: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000a10: 0a09 093c 696d 6720 7372 633d 2268 7474  ...<img src="htt
+00000a20: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000a30: 2e69 6f2f 6261 6467 652f 2546 3025 3946  .io/badge/%F0%9F
+00000a40: 2541 3525 3941 2d48 6174 6368 2d34 3035  %A5%9A-Hatch-405
+00000a50: 3162 352e 7376 6722 202f 3e0a 093c 2f61  1b5.svg" />..</a
+00000a60: 3e0a 3c2f 6469 763e 0a0a 0a2a 2a45 6173  >.</div>...**Eas
+00000a70: 794c 4c4d 2a2a 2069 7320 616e 206f 7065  yLLM** is an ope
+00000a80: 6e20 736f 7572 6365 2070 726f 6a65 6374  n source project
+00000a90: 2074 6861 7420 7072 6f76 6964 6573 202a   that provides *
+00000aa0: 2a68 656c 7066 756c 2074 6f6f 6c73 2061  *helpful tools a
+00000ab0: 6e64 206d 6574 686f 6473 2066 6f72 2077  nd methods for w
+00000ac0: 6f72 6b69 6e67 2077 6974 6820 6c61 7267  orking with larg
+00000ad0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
+00000ae0: 732a 2a20 284c 4c4d 7329 2c20 626f 7468  s** (LLMs), both
+00000af0: 206f 7065 6e20 736f 7572 6365 2061 6e64   open source and
+00000b00: 2063 6c6f 7365 6420 736f 7572 6365 2e20   closed source. 
+00000b10: 4765 7420 696d 6d65 6469 6174 616c 7920  Get immediataly 
+00000b20: 7374 6172 7465 6420 6f72 2063 6865 636b  started or check
+00000b30: 206f 7574 2074 6865 205b 646f 6375 6d65   out the [docume
+00000b40: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000b50: 2f70 6869 6c73 6368 6d69 642e 6769 7468  /philschmid.gith
+00000b60: 7562 2e69 6f2f 6561 7379 6c6c 6d2f 292e  ub.io/easyllm/).
+00000b70: 0a0a 4561 7379 4c4c 4d20 696d 706c 656d  ..EasyLLM implem
+00000b80: 656e 7473 2063 6c69 656e 7473 2074 6861  ents clients tha
+00000b90: 7420 6172 6520 2a2a 636f 6d70 6174 6962  t are **compatib
+00000ba0: 6c65 2077 6974 6820 4f70 656e 4149 2773  le with OpenAI's
+00000bb0: 2043 6f6d 706c 6574 696f 6e20 4150 492a   Completion API*
+00000bc0: 2a2e 2054 6869 7320 6d65 616e 7320 796f  *. This means yo
+00000bd0: 7520 6361 6e20 6561 7369 6c79 2072 6570  u can easily rep
+00000be0: 6c61 6365 2060 6f70 656e 6169 2e43 6861  lace `openai.Cha
+00000bf0: 7443 6f6d 706c 6574 696f 6e60 2c20 606f  tCompletion`, `o
+00000c00: 7065 6e61 692e 436f 6d70 6c65 7469 6f6e  penai.Completion
+00000c10: 602c 2060 6f70 656e 6169 2e45 6d62 6564  `, `openai.Embed
+00000c20: 6469 6e67 6020 7769 7468 2c20 666f 7220  ding` with, for 
+00000c30: 6578 616d 706c 652c 2060 6875 6767 696e  example, `huggin
+00000c40: 6766 6163 652e 4368 6174 436f 6d70 6c65  gface.ChatComple
+00000c50: 7469 6f6e 602c 2060 6875 6767 696e 6766  tion`, `huggingf
+00000c60: 6163 652e 436f 6d70 6c65 7469 6f6e 6020  ace.Completion` 
+00000c70: 6f72 2060 6875 6767 696e 6766 6163 652e  or `huggingface.
+00000c80: 456d 6265 6464 696e 6760 2062 7920 6368  Embedding` by ch
+00000c90: 616e 6769 6e67 206f 6e65 206c 696e 6520  anging one line 
+00000ca0: 6f66 2063 6f64 652e 0a0a 2323 2320 5375  of code...### Su
+00000cb0: 7070 6f72 7465 6420 436c 6965 6e74 7320  pported Clients 
+00000cc0: 0a0a 2a20 6068 7567 6769 6e67 6661 6365  ..* `huggingface
+00000cd0: 6020 2d20 5b48 7567 6769 6e67 4661 6365  ` - [HuggingFace
+00000ce0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00000cf0: 6766 6163 652e 636f 2f29 206d 6f64 656c  gface.co/) model
+00000d00: 730a 2020 2a20 6068 7567 6769 6e67 6661  s.  * `huggingfa
+00000d10: 6365 2e43 6861 7443 6f6d 706c 6574 696f  ce.ChatCompletio
+00000d20: 6e60 202d 2043 6861 7420 7769 7468 204c  n` - Chat with L
+00000d30: 4c4d 730a 2020 2a20 6068 7567 6769 6e67  LMs.  * `hugging
+00000d40: 6661 6365 2e43 6f6d 706c 6574 696f 6e60  face.Completion`
+00000d50: 202d 2054 6578 7420 636f 6d70 6c65 7469   - Text completi
+00000d60: 6f6e 2077 6974 6820 4c4c 4d73 0a20 202a  on with LLMs.  *
+00000d70: 2060 6875 6767 696e 6766 6163 652e 456d   `huggingface.Em
+00000d80: 6265 6464 696e 6760 202d 2043 7265 6174  bedding` - Creat
+00000d90: 6520 656d 6265 6464 696e 6773 2077 6974  e embeddings wit
+00000da0: 6820 4c4c 4d73 0a0a 4368 6563 6b20 6f75  h LLMs..Check ou
+00000db0: 7420 7468 6520 5b45 7861 6d70 6c65 735d  t the [Examples]
+00000dc0: 282e 2f65 7861 6d70 6c65 7329 2074 6f20  (./examples) to 
+00000dd0: 6765 7420 7374 6172 7465 642e 0a0a 2323  get started...##
+00000de0: 20f0 9f9a 8020 4765 7474 696e 6720 5374   .... Getting St
+00000df0: 6172 7465 640a 0a49 6e73 7461 6c6c 2045  arted..Install E
+00000e00: 6173 794c 4c4d 2076 6961 2070 6970 3a0a  asyLLM via pip:.
+00000e10: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+00000e20: 7461 6c6c 2065 6173 796c 6c6d 0a60 6060  tall easyllm.```
+00000e30: 0a0a 5468 656e 2069 6d70 6f72 7420 616e  ..Then import an
+00000e40: 6420 7374 6172 7420 7573 696e 6720 7468  d start using th
+00000e50: 6520 636c 6965 6e74 733a 0a0a 6060 6070  e clients:..```p
+00000e60: 7974 686f 6e0a 0a66 726f 6d20 6561 7379  ython..from easy
+00000e70: 6c6c 6d2e 636c 6965 6e74 7320 696d 706f  llm.clients impo
+00000e80: 7274 2068 7567 6769 6e67 6661 6365 0a0a  rt huggingface..
+00000e90: 2320 6865 6c70 6572 2074 6f20 6275 696c  # helper to buil
+00000ea0: 6420 6c6c 616d 6132 2070 726f 6d70 740a  d llama2 prompt.
+00000eb0: 6875 6767 696e 6766 6163 652e 7072 6f6d  huggingface.prom
+00000ec0: 7074 5f62 7569 6c64 6572 203d 2022 6c6c  pt_builder = "ll
+00000ed0: 616d 6132 220a 0a72 6573 706f 6e73 6520  ama2"..response 
+00000ee0: 3d20 6875 6767 696e 6766 6163 652e 4368  = huggingface.Ch
+00000ef0: 6174 436f 6d70 6c65 7469 6f6e 2e63 7265  atCompletion.cre
+00000f00: 6174 6528 0a20 2020 206d 6f64 656c 3d22  ate(.    model="
+00000f10: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
+00000f20: 2d32 2d37 3062 2d63 6861 742d 6866 222c  -2-70b-chat-hf",
+00000f30: 0a20 2020 206d 6573 7361 6765 733d 5b0a  .    messages=[.
+00000f40: 2020 2020 2020 2020 7b22 726f 6c65 223a          {"role":
+00000f50: 2022 7379 7374 656d 222c 2022 636f 6e74   "system", "cont
+00000f60: 656e 7422 3a20 225c 6e59 6f75 2061 7265  ent": "\nYou are
+00000f70: 2061 2068 656c 7066 756c 2061 7373 6973   a helpful assis
+00000f80: 7461 6e74 2073 7065 616b 696e 6720 6c69  tant speaking li
+00000f90: 6b65 2061 2070 6972 6174 652e 2061 7267  ke a pirate. arg
+00000fa0: 6821 227d 2c0a 2020 2020 2020 2020 7b22  h!"},.        {"
+00000fb0: 726f 6c65 223a 2022 7573 6572 222c 2022  role": "user", "
+00000fc0: 636f 6e74 656e 7422 3a20 2257 6861 7420  content": "What 
+00000fd0: 6973 2074 6865 2073 756e 3f22 7d2c 0a20  is the sun?"},. 
+00000fe0: 2020 205d 2c0a 2020 2020 7465 6d70 6572     ],.    temper
+00000ff0: 6174 7572 653d 302e 392c 0a20 2020 2074  ature=0.9,.    t
+00001000: 6f70 5f70 3d30 2e36 2c0a 2020 2020 6d61  op_p=0.6,.    ma
+00001010: 785f 746f 6b65 6e73 3d32 3536 2c0a 290a  x_tokens=256,.).
+00001020: 0a70 7269 6e74 2872 6573 706f 6e73 6529  .print(response)
+00001030: 0a60 6060 0a74 6865 2072 6573 756c 7420  .```.the result 
+00001040: 7769 6c6c 206c 6f6f 6b20 6c69 6b65 200a  will look like .
+00001050: 0a60 6060 6261 7368 0a7b 0a20 2022 6964  .```bash.{.  "id
+00001060: 223a 2022 6866 2d6c 5643 3269 544d 6b46  ": "hf-lVC2iTMkF
+00001070: 4a22 2c0a 2020 226f 626a 6563 7422 3a20  J",.  "object": 
+00001080: 2263 6861 742e 636f 6d70 6c65 7469 6f6e  "chat.completion
+00001090: 222c 0a20 2022 6372 6561 7465 6422 3a20  ",.  "created": 
+000010a0: 3136 3930 3636 3131 3434 2c0a 2020 226d  1690661144,.  "m
+000010b0: 6f64 656c 223a 2022 6d65 7461 2d6c 6c61  odel": "meta-lla
+000010c0: 6d61 2f4c 6c61 6d61 2d32 2d37 3062 2d63  ma/Llama-2-70b-c
+000010d0: 6861 742d 6866 222c 0a20 2022 6368 6f69  hat-hf",.  "choi
+000010e0: 6365 7322 3a20 5b0a 2020 2020 7b0a 2020  ces": [.    {.  
+000010f0: 2020 2020 2269 6e64 6578 223a 2030 2c0a      "index": 0,.
+00001100: 2020 2020 2020 226d 6573 7361 6765 223a        "message":
+00001110: 207b 0a20 2020 2020 2020 2022 726f 6c65   {.        "role
+00001120: 223a 2022 6173 7369 7374 616e 7422 2c0a  ": "assistant",.
+00001130: 2020 2020 2020 2020 2263 6f6e 7465 6e74          "content
+00001140: 223a 2022 2041 7272 7272 2c20 7468 6520  ": " Arrrr, the 
+00001150: 7375 6e20 6265 2061 2062 6967 206f 6c27  sun be a big ol'
+00001160: 2062 616c 6c20 6f27 2066 6972 6520 696e   ball o' fire in
+00001170: 2074 6865 2073 6b79 2c20 6d65 2068 6561   the sky, me hea
+00001180: 7274 7921 2049 7420 6265 2074 6865 2073  rty! It be the s
+00001190: 6f75 7263 6520 6f27 206c 6967 6874 2061  ource o' light a
+000011a0: 6e64 2077 6172 6d74 6820 666f 7220 6f75  nd warmth for ou
+000011b0: 7220 6661 6972 2070 6c61 6e65 742c 2061  r fair planet, a
+000011c0: 6e64 2069 7420 6265 2061 206d 6967 6874  nd it be a might
+000011d0: 7920 706f 7765 7266 756c 2066 6f72 6365  y powerful force
+000011e0: 2c20 7361 7676 793f 2057 6974 686f 7574  , savvy? Without
+000011f0: 2074 6865 2073 756e 2c20 7765 2764 2062   the sun, we'd b
+00001200: 6520 7361 696c 696e 2720 7468 726f 7567  e sailin' throug
+00001210: 6820 7468 6520 6461 726b 6e65 7373 2c20  h the darkness, 
+00001220: 6c6f 7374 2061 6e64 2063 6f6c 642c 2073  lost and cold, s
+00001230: 6f20 6c65 7427 7320 6769 7665 2061 2068  o let's give a h
+00001240: 6561 7274 7920 5c22 5961 7272 7221 5c22  earty \"Yarrr!\"
+00001250: 2066 6f72 2074 6865 2073 756e 2c20 6d65   for the sun, me
+00001260: 2068 6561 7274 6965 7321 2041 7272 7272   hearties! Arrrr
+00001270: 2122 0a20 2020 2020 207d 2c0a 2020 2020  !".      },.    
+00001280: 2020 2266 696e 6973 685f 7265 6173 6f6e    "finish_reason
+00001290: 223a 206e 756c 6c0a 2020 2020 7d0a 2020  ": null.    }.  
+000012a0: 5d2c 0a20 2022 7573 6167 6522 3a20 7b0a  ],.  "usage": {.
+000012b0: 2020 2020 2270 726f 6d70 745f 746f 6b65      "prompt_toke
+000012c0: 6e73 223a 2031 3131 2c0a 2020 2020 2263  ns": 111,.    "c
+000012d0: 6f6d 706c 6574 696f 6e5f 746f 6b65 6e73  ompletion_tokens
+000012e0: 223a 2032 3939 2c0a 2020 2020 2274 6f74  ": 299,.    "tot
+000012f0: 616c 5f74 6f6b 656e 7322 3a20 3431 300a  al_tokens": 410.
+00001300: 2020 7d0a 7d0a 6060 600a 0a43 6865 636b    }.}.```..Check
+00001310: 206f 7574 206f 7468 6572 2065 7861 6d70   out other examp
+00001320: 6c65 733a 0a2a 205b 4465 7461 696c 6564  les:.* [Detailed
+00001330: 2043 6861 7443 6f6d 706c 6574 696f 6e20   ChatCompletion 
+00001340: 4578 616d 706c 655d 286e 6f74 6562 6f6f  Example](noteboo
+00001350: 6b73 2f63 6861 742d 636f 6d70 6c65 7469  ks/chat-completi
+00001360: 6f6e 2d61 7069 2e69 7079 6e62 290a 2a20  on-api.ipynb).* 
+00001370: 5b45 7861 6d70 6c65 2068 6f77 2074 6f20  [Example how to 
+00001380: 7374 7265 616d 2063 6861 7420 7265 7175  stream chat requ
+00001390: 6573 7473 5d28 6e6f 7465 626f 6f6b 732f  ests](notebooks/
+000013a0: 7374 7265 616d 2d63 6861 742d 636f 6d70  stream-chat-comp
+000013b0: 6c65 7469 6f6e 732e 6970 796e 6229 0a2a  letions.ipynb).*
+000013c0: 205b 4578 616d 706c 6520 686f 7720 746f   [Example how to
+000013d0: 2073 7472 6561 6d20 7465 7874 2072 6571   stream text req
+000013e0: 7565 7374 735d 286e 6f74 6562 6f6f 6b73  uests](notebooks
+000013f0: 2f73 7472 6561 6d2d 7465 7874 2d63 6f6d  /stream-text-com
+00001400: 706c 6574 696f 6e73 2e69 7079 6e62 290a  pletions.ipynb).
+00001410: 2a20 5b44 6574 6169 6c65 6420 436f 6d70  * [Detailed Comp
+00001420: 6c65 7469 6f6e 2045 7861 6d70 6c65 5d28  letion Example](
+00001430: 6e6f 7465 626f 6f6b 732f 7465 7874 2d63  notebooks/text-c
+00001440: 6f6d 706c 6574 696f 6e2d 6170 692e 6970  ompletion-api.ip
+00001450: 796e 6229 0a2a 205b 4372 6561 7465 2045  ynb).* [Create E
+00001460: 6d62 6564 6469 6e67 735d 286e 6f74 6562  mbeddings](noteb
+00001470: 6f6f 6b73 2f67 6574 2d65 6d62 6564 6469  ooks/get-embeddi
+00001480: 6e67 7329 0a0a 5365 6520 7468 6520 5b64  ngs)..See the [d
+00001490: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+000014a0: 7470 733a 2f2f 7068 696c 7363 686d 6964  tps://philschmid
+000014b0: 2e67 6974 6875 622e 696f 2f65 6173 796c  .github.io/easyl
+000014c0: 6c6d 2f29 2066 6f72 206d 6f72 6520 6465  lm/) for more de
+000014d0: 7461 696c 6564 2075 7361 6765 2061 6e64  tailed usage and
+000014e0: 2065 7861 6d70 6c65 732e 0a0a 2323 20f0   examples...## .
+000014f0: 9f92 aaf0 9f8f bb20 4d69 6772 6174 696f  ....... Migratio
+00001500: 6e20 6672 6f6d 204f 7065 6e41 4920 746f  n from OpenAI to
+00001510: 2048 7567 6769 6e67 4661 6365 0a0a 4d69   HuggingFace..Mi
+00001520: 6772 6174 696e 6720 6672 6f6d 204f 7065  grating from Ope
+00001530: 6e41 4920 746f 2048 7567 6769 6e67 4661  nAI to HuggingFa
+00001540: 6365 2069 7320 6561 7379 2e20 4a75 7374  ce is easy. Just
+00001550: 2063 6861 6e67 6520 7468 6520 696d 706f   change the impo
+00001560: 7274 2073 7461 7465 6d65 6e74 2061 6e64  rt statement and
+00001570: 2074 6865 2063 6c69 656e 7420 796f 7520   the client you 
+00001580: 7761 6e74 2074 6f20 7573 6520 616e 6420  want to use and 
+00001590: 6f70 7469 6f6e 616c 6c79 2074 6865 2070  optionally the p
+000015a0: 726f 6d70 7420 6275 696c 6465 722e 0a0a  rompt builder...
+000015b0: 6060 6064 6966 660a 2d20 696d 706f 7274  ```diff.- import
+000015c0: 206f 7065 6e61 690a 2b20 6672 6f6d 2065   openai.+ from e
+000015d0: 6173 796c 6c6d 2e63 6c69 656e 7473 2069  asyllm.clients i
+000015e0: 6d70 6f72 7420 6875 6767 696e 6766 6163  mport huggingfac
+000015f0: 650a 2b20 6875 6767 696e 6766 6163 652e  e.+ huggingface.
+00001600: 7072 6f6d 7074 5f62 7569 6c64 6572 203d  prompt_builder =
+00001610: 2022 6c6c 616d 6132 220a 0a0a 2d20 7265   "llama2"...- re
+00001620: 7370 6f6e 7365 203d 206f 7065 6e61 692e  sponse = openai.
+00001630: 4368 6174 436f 6d70 6c65 7469 6f6e 2e63  ChatCompletion.c
+00001640: 7265 6174 6528 0a2b 2072 6573 706f 6e73  reate(.+ respons
+00001650: 6520 3d20 6875 6767 696e 6766 6163 652e  e = huggingface.
+00001660: 4368 6174 436f 6d70 6c65 7469 6f6e 2e63  ChatCompletion.c
+00001670: 7265 6174 6528 0a2d 2020 2020 6d6f 6465  reate(.-    mode
+00001680: 6c3d 2267 7074 2d33 2e35 2d74 7572 626f  l="gpt-3.5-turbo
+00001690: 222c 0a2b 2020 2020 6d6f 6465 6c3d 226d  ",.+    model="m
+000016a0: 6574 612d 6c6c 616d 612f 4c6c 616d 612d  eta-llama/Llama-
+000016b0: 322d 3730 622d 6368 6174 2d68 6622 2c0a  2-70b-chat-hf",.
+000016c0: 2020 2020 6d65 7373 6167 6573 3d5b 0a20      messages=[. 
+000016d0: 2020 2020 2020 207b 2272 6f6c 6522 3a20         {"role": 
+000016e0: 2273 7973 7465 6d22 2c20 2263 6f6e 7465  "system", "conte
+000016f0: 6e74 223a 2022 596f 7520 6172 6520 6120  nt": "You are a 
+00001700: 6865 6c70 6675 6c20 6173 7369 7374 616e  helpful assistan
+00001710: 742e 227d 2c0a 2020 2020 2020 2020 7b22  t."},.        {"
+00001720: 726f 6c65 223a 2022 7573 6572 222c 2022  role": "user", "
+00001730: 636f 6e74 656e 7422 3a20 224b 6e6f 636b  content": "Knock
+00001740: 206b 6e6f 636b 2e22 7d2c 0a20 2020 205d   knock."},.    ]
+00001750: 2c0a 290a 6060 600a 0a4d 616b 6520 7375  ,.).```..Make su
+00001760: 7265 2077 6865 6e20 796f 7520 7377 6974  re when you swit
+00001770: 6368 2079 6f75 7220 636c 6965 6e74 2074  ch your client t
+00001780: 6861 7420 796f 7572 2068 7970 6572 7061  hat your hyperpa
+00001790: 7261 6d65 7465 7273 2061 7265 2073 7469  rameters are sti
+000017a0: 6c6c 2076 616c 6964 2e20 466f 7220 6578  ll valid. For ex
+000017b0: 616d 706c 652c 2060 7465 6d70 6572 6174  ample, `temperat
+000017c0: 7572 6560 206f 6620 4750 542d 3320 6d69  ure` of GPT-3 mi
+000017d0: 6768 7420 6265 2064 6966 6665 7265 6e74  ght be different
+000017e0: 2074 6861 6e20 6074 656d 7065 7261 7475   than `temperatu
+000017f0: 7265 6020 6f66 2060 4c6c 616d 612d 3260  re` of `Llama-2`
+00001800: 2e0a 0a23 2320 e298 91ef b88f 204b 6579  ...## ...... Key
+00001810: 2046 6561 7475 7265 730a 0a23 2323 20f0   Features..### .
+00001820: 9fa4 9d20 436f 6d70 6174 6962 6c65 2043  ... Compatible C
+00001830: 6c69 656e 7473 0a0a 2d20 496d 706c 656d  lients..- Implem
+00001840: 656e 7461 7469 6f6e 206f 6620 636c 6965  entation of clie
+00001850: 6e74 7320 636f 6d70 6174 6962 6c65 2077  nts compatible w
+00001860: 6974 6820 4f70 656e 4149 2041 5049 2066  ith OpenAI API f
+00001870: 6f72 6d61 7420 6f66 2060 6f70 656e 6169  ormat of `openai
+00001880: 2e43 6861 7443 6f6d 706c 6574 696f 6e60  .ChatCompletion`
+00001890: 2c20 606f 7065 6e61 692e 436f 6d70 6c65  , `openai.Comple
+000018a0: 7469 6f6e 602c 2060 6f70 656e 6169 2e45  tion`, `openai.E
+000018b0: 6d62 6564 6469 6e67 602e 0a2d 2045 6173  mbedding`..- Eas
+000018c0: 696c 7920 7377 6974 6368 2062 6574 7765  ily switch betwe
+000018d0: 656e 2064 6966 6665 7265 6e74 204c 4c4d  en different LLM
+000018e0: 7320 6c69 6b65 2060 6f70 656e 6169 2e43  s like `openai.C
+000018f0: 6861 7443 6f6d 706c 6574 696f 6e60 2061  hatCompletion` a
+00001900: 6e64 2060 6875 6767 696e 6766 6163 652e  nd `huggingface.
+00001910: 4368 6174 436f 6d70 6c65 7469 6f6e 6020  ChatCompletion` 
+00001920: 6279 2063 6861 6e67 696e 6720 6f6e 6520  by changing one 
+00001930: 6c69 6e65 206f 6620 636f 6465 2e20 0a2d  line of code. .-
+00001940: 2053 7570 706f 7274 2066 6f72 2073 7472   Support for str
+00001950: 6561 6d69 6e67 206f 6620 636f 6d70 6c65  eaming of comple
+00001960: 7469 6f6e 732c 2063 6865 636b 6f75 7420  tions, checkout 
+00001970: 6578 616d 706c 6520 5b48 6f77 2074 6f20  example [How to 
+00001980: 7374 7265 616d 2063 6f6d 706c 6574 696f  stream completio
+00001990: 6e73 5d28 2e2f 6e6f 7465 626f 6f6b 732f  ns](./notebooks/
+000019a0: 7374 7265 616d 2d63 6861 742d 636f 6d70  stream-chat-comp
+000019b0: 6c65 7469 6f6e 732e 6970 796e 6229 2e0a  letions.ipynb)..
+000019c0: 0a23 2323 20e2 9a99 efb8 8f20 4865 6c70  .### ...... Help
+000019d0: 6572 204d 6f64 756c 6573 20e2 9a99 efb8  er Modules .....
+000019e0: 8f0a 0a2d 2060 6576 6f6c 5f69 6e73 7472  ...- `evol_instr
+000019f0: 7563 7460 2028 776f 726b 2069 6e20 7072  uct` (work in pr
+00001a00: 6f67 7265 7373 2920 2d20 5573 6520 6576  ogress) - Use ev
+00001a10: 6f6c 7574 696f 6e61 7279 2061 6c67 6f72  olutionary algor
+00001a20: 6974 686d 7320 6372 6561 7465 2069 6e73  ithms create ins
+00001a30: 7472 7563 7469 6f6e 7320 666f 7220 4c4c  tructions for LL
+00001a40: 4d73 2e0a 0a2d 2060 7072 6f6d 7074 5f75  Ms...- `prompt_u
+00001a50: 7469 6c73 6020 2d20 4865 6c70 6572 206d  tils` - Helper m
+00001a60: 6574 686f 6473 2074 6f20 6561 7369 6c79  ethods to easily
+00001a70: 2063 6f6e 7665 7274 2062 6574 7765 656e   convert between
+00001a80: 2070 726f 6d70 7420 666f 726d 6174 7320   prompt formats 
+00001a90: 6c69 6b65 204f 7065 6e41 4920 4d65 7373  like OpenAI Mess
+00001aa0: 6167 6573 2074 6f20 7072 6f6d 7074 7320  ages to prompts 
+00001ab0: 666f 7220 6f70 656e 2073 6f75 7263 6520  for open source 
+00001ac0: 6d6f 6465 6c73 206c 696b 6520 4c6c 616d  models like Llam
+00001ad0: 6120 322e 0a0a 2323 20f0 9f99 8f20 436f  a 2...## .... Co
+00001ae0: 6e74 7269 6275 7469 6e67 0a0a 4561 7379  ntributing..Easy
+00001af0: 4c4c 4d20 6973 2061 6e20 6f70 656e 2073  LLM is an open s
+00001b00: 6f75 7263 6520 7072 6f6a 6563 7420 616e  ource project an
+00001b10: 6420 7765 6c63 6f6d 6573 2063 6f6e 7472  d welcomes contr
+00001b20: 6962 7574 696f 6e73 206f 6620 616c 6c20  ibutions of all 
+00001b30: 6b69 6e64 732e 0a0a 5468 6520 7072 6f6a  kinds...The proj
+00001b40: 6563 7420 7573 6573 205b 6861 7463 685d  ect uses [hatch]
+00001b50: 2868 7474 7073 3a2f 2f68 6174 6368 2e70  (https://hatch.p
+00001b60: 7970 612e 696f 2f6c 6174 6573 742f 2920  ypa.io/latest/) 
+00001b70: 666f 7220 6465 7665 6c6f 706d 656e 742e  for development.
+00001b80: 2054 6f20 6765 7420 7374 6172 7465 642c   To get started,
+00001b90: 2066 6f72 6b20 7468 6520 7265 706f 7369   fork the reposi
+00001ba0: 746f 7279 2061 6e64 2063 6c6f 6e65 200a  tory and clone .
+00001bb0: 6974 2074 6f20 796f 7572 206c 6f63 616c  it to your local
+00001bc0: 206d 6163 6869 6e65 2e0a 0a30 2e20 436f   machine...0. Co
+00001bd0: 6e66 6972 6d20 5b68 6174 6368 5d28 6874  nfirm [hatch](ht
+00001be0: 7470 733a 2f2f 6861 7463 682e 7079 7061  tps://hatch.pypa
+00001bf0: 2e69 6f2f 6c61 7465 7374 2f69 6e73 7461  .io/latest/insta
+00001c00: 6c6c 2f29 2069 7320 696e 7374 616c 6c65  ll/) is installe
+00001c10: 6420 2870 6970 7820 6973 2067 7265 6174  d (pipx is great
+00001c20: 2074 6f20 6d61 6b65 2069 7420 6176 6169   to make it avai
+00001c30: 6c61 626c 6520 676c 6f62 616c 6c79 206f  lable globally o
+00001c40: 6e20 796f 7572 206d 6163 6869 6e65 290a  n your machine).
+00001c50: 312e 204f 6e63 6520 696e 2074 6865 2070  1. Once in the p
+00001c60: 726f 6a65 6374 2064 6972 6563 746f 7279  roject directory
+00001c70: 2c20 7275 6e20 6068 6174 6368 2065 6e76  , run `hatch env
+00001c80: 2063 7265 6174 6560 2074 6f20 6372 6561   create` to crea
+00001c90: 7465 2061 2064 6566 6175 6c74 2076 6972  te a default vir
+00001ca0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+00001cb0: 2066 6f72 2064 6576 656c 6f70 6d65 6e74   for development
+00001cc0: 2e0a 322e 2041 6374 6976 6174 6520 7468  ..2. Activate th
+00001cd0: 6520 7669 7274 7561 6c20 656e 7669 726f  e virtual enviro
+00001ce0: 6e6d 656e 7420 7769 7468 2060 6861 7463  nment with `hatc
+00001cf0: 6820 7368 656c 6c60 0a33 2e20 5374 6172  h shell`.3. Star
+00001d00: 7420 6465 7665 6c6f 7069 6e67 2120 f09f  t developing! ..
+00001d10: a4a9 0a0a 2323 20f0 9f93 9420 4369 7461  ....## .... Cita
+00001d20: 7469 6f6e 2026 2041 636b 6e6f 776c 6564  tion & Acknowled
+00001d30: 6765 6d65 6e74 730a 0a49 6620 796f 7520  gements..If you 
+00001d40: 7573 6520 4561 7379 4c4c 4d2c 2070 6c65  use EasyLLM, ple
+00001d50: 6173 6520 7368 6172 6520 6974 2077 6974  ase share it wit
+00001d60: 6820 6d65 206f 6e20 736f 6369 616c 206d  h me on social m
+00001d70: 6564 6961 206f 7220 656d 6169 6c2e 2049  edia or email. I
+00001d80: 2077 6f75 6c64 206c 6f76 6520 746f 2068   would love to h
+00001d90: 6561 7220 6162 6f75 7420 6974 210a 596f  ear about it!.Yo
+00001da0: 7520 6361 6e20 616c 736f 2063 6974 6520  u can also cite 
+00001db0: 7468 6520 7072 6f6a 6563 7420 7573 696e  the project usin
+00001dc0: 6720 7468 6520 666f 6c6c 6f77 696e 6720  g the following 
+00001dd0: 4269 6254 6558 3a0a 0a60 6060 6261 7368  BibTeX:..```bash
+00001de0: 0a40 736f 6674 7761 7265 7b50 6869 6c69  .@software{Phili
+00001df0: 7070 5f53 6368 6d69 645f 4561 7379 4c4c  pp_Schmid_EasyLL
+00001e00: 4d5f 3230 3233 2c0a 6175 7468 6f72 203d  M_2023,.author =
+00001e10: 207b 5068 696c 6970 7020 5363 686d 6964   {Philipp Schmid
+00001e20: 7d2c 0a6c 6963 656e 7365 203d 207b 4170  },.license = {Ap
+00001e30: 6163 6865 2d32 2e30 7d2c 0a6d 6f6e 7468  ache-2.0},.month
+00001e40: 203d 206a 756a 2c0a 7469 746c 6520 3d20   = juj,.title = 
+00001e50: 7b45 6173 794c 4c4d 3a20 5374 7265 616d  {EasyLLM: Stream
+00001e60: 6c69 6e65 6420 546f 6f6c 7320 666f 7220  lined Tools for 
+00001e70: 4c4c 4d73 7d2c 0a75 726c 203d 207b 6874  LLMs},.url = {ht
+00001e80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001e90: 2f70 6869 6c73 6368 6d69 642f 6561 7379  /philschmid/easy
+00001ea0: 6c6c 6d7d 2c0a 7965 6172 203d 207b 3230  llm},.year = {20
+00001eb0: 3233 7d0a 7d0a 6060 600a                 23}.}.```.
```


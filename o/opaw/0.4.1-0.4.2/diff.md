# Comparing `tmp/opaw-0.4.1.tar.gz` & `tmp/opaw-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opaw-0.4.1.tar", last modified: Mon Aug  7 16:05:31 2023, max compression
+gzip compressed data, was "opaw-0.4.2.tar", last modified: Tue Aug  8 17:20:54 2023, max compression
```

## Comparing `opaw-0.4.1.tar` & `opaw-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.867837 opaw-0.4.1/
--rw-rw-rw-   0        0        0     1085 2023-08-06 16:29:18.000000 opaw-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1709 2023-08-07 16:05:31.867837 opaw-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-08-07 16:02:14.000000 opaw-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.714095 opaw-0.4.1/opaw/
--rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.4.1/opaw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.826507 opaw-0.4.1/opaw/examples/
--rw-rw-rw-   0        0        0      110 2023-08-04 17:27:47.000000 opaw-0.4.1/opaw/examples/__init__.py
--rw-rw-rw-   0        0        0      589 2023-08-07 06:42:53.000000 opaw-0.4.1/opaw/examples/audio.py
--rw-rw-rw-   0        0        0     1058 2023-08-07 07:02:30.000000 opaw-0.4.1/opaw/examples/basic.py
--rw-rw-rw-   0        0        0      548 2023-08-07 06:54:13.000000 opaw-0.4.1/opaw/examples/chat.py
--rw-rw-rw-   0        0        0      457 2023-08-07 06:56:50.000000 opaw-0.4.1/opaw/examples/completion.py
--rw-rw-rw-   0        0        0      574 2023-08-07 09:46:04.000000 opaw-0.4.1/opaw/examples/edit.py
--rw-rw-rw-   0        0        0      476 2023-08-07 06:58:39.000000 opaw-0.4.1/opaw/examples/embedding.py
--rw-rw-rw-   0        0        0      658 2023-08-07 06:59:42.000000 opaw-0.4.1/opaw/examples/file.py
--rw-rw-rw-   0        0        0      601 2023-08-07 07:04:07.000000 opaw-0.4.1/opaw/examples/finetune.py
--rw-rw-rw-   0        0        0      743 2023-08-07 09:09:21.000000 opaw-0.4.1/opaw/examples/funcs.py
--rw-rw-rw-   0        0        0      775 2023-08-07 09:09:21.000000 opaw-0.4.1/opaw/examples/function_call.py
--rw-rw-rw-   0        0        0      453 2023-08-07 07:05:59.000000 opaw-0.4.1/opaw/examples/image.py
--rw-rw-rw-   0        0        0      510 2023-08-07 07:06:55.000000 opaw-0.4.1/opaw/examples/load-chat.py
--rw-rw-rw-   0        0        0      718 2023-08-07 06:25:24.000000 opaw-0.4.1/opaw/examples/moderation.py
--rw-rw-rw-   0        0        0       56 2023-08-07 16:00:59.000000 opaw-0.4.1/opaw/main.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.855096 opaw-0.4.1/opaw/model/
--rw-rw-rw-   0        0        0        0 2023-08-07 05:55:31.000000 opaw-0.4.1/opaw/model/__init__.py
--rw-rw-rw-   0        0        0     1189 2023-08-06 14:28:25.000000 opaw-0.4.1/opaw/model/audio.py
--rw-rw-rw-   0        0        0     2062 2023-08-06 14:16:59.000000 opaw-0.4.1/opaw/model/bot.py
--rw-rw-rw-   0        0        0     3432 2023-08-07 09:05:54.000000 opaw-0.4.1/opaw/model/chat.py
--rw-rw-rw-   0        0        0      629 2023-08-06 08:24:20.000000 opaw-0.4.1/opaw/model/completion.py
--rw-rw-rw-   0        0        0      736 2023-08-07 09:49:15.000000 opaw-0.4.1/opaw/model/edit.py
--rw-rw-rw-   0        0        0      625 2023-08-06 14:28:25.000000 opaw-0.4.1/opaw/model/embedding.py
--rw-rw-rw-   0        0        0     1215 2023-08-06 15:34:39.000000 opaw-0.4.1/opaw/model/file.py
--rw-rw-rw-   0        0        0     1003 2023-08-06 14:28:25.000000 opaw-0.4.1/opaw/model/finetune.py
--rw-rw-rw-   0        0        0     1242 2023-08-06 14:05:06.000000 opaw-0.4.1/opaw/model/image.py
--rw-rw-rw-   0        0        0      633 2023-08-06 14:28:25.000000 opaw-0.4.1/opaw/model/moderation.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.860795 opaw-0.4.1/opaw/test/
--rw-rw-rw-   0        0        0        0 2023-07-31 12:07:48.000000 opaw-0.4.1/opaw/test/__init__.py
--rw-rw-rw-   0        0        0        0 2023-08-07 05:57:37.000000 opaw-0.4.1/opaw/test/test.py
--rw-rw-rw-   0        0        0       47 2023-08-06 07:05:13.000000 opaw-0.4.1/opaw/test/test2.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.864965 opaw-0.4.1/opaw/util/
--rw-rw-rw-   0        0        0     2049 2023-08-07 15:59:23.000000 opaw-0.4.1/opaw/util/__init__.py
--rw-rw-rw-   0        0        0     1096 2023-08-07 06:27:22.000000 opaw-0.4.1/opaw/util/log.py
-drwxrwxrwx   0        0        0        0 2023-08-07 16:05:31.772074 opaw-0.4.1/opaw.egg-info/
--rw-rw-rw-   0        0        0     1709 2023-08-07 16:05:31.000000 opaw-0.4.1/opaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-08-07 16:05:31.000000 opaw-0.4.1/opaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 16:05:31.000000 opaw-0.4.1/opaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 16:05:31.000000 opaw-0.4.1/opaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-07 16:05:31.000000 opaw-0.4.1/opaw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-08-07 16:05:31.870667 opaw-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      806 2023-08-07 16:00:59.000000 opaw-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.947334 opaw-0.4.2/
+-rw-rw-rw-   0        0        0     1085 2023-08-06 16:29:18.000000 opaw-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     1807 2023-08-08 17:20:54.947334 opaw-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1332 2023-08-08 05:07:43.000000 opaw-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.796000 opaw-0.4.2/opaw/
+-rw-rw-rw-   0        0        0        0 2023-08-04 15:52:21.000000 opaw-0.4.2/opaw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.890712 opaw-0.4.2/opaw/examples/
+-rw-rw-rw-   0        0        0      110 2023-08-04 17:27:47.000000 opaw-0.4.2/opaw/examples/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-08-07 06:42:53.000000 opaw-0.4.2/opaw/examples/audio.py
+-rw-rw-rw-   0        0        0     1058 2023-08-07 07:02:30.000000 opaw-0.4.2/opaw/examples/basic.py
+-rw-rw-rw-   0        0        0      712 2023-08-08 08:50:34.000000 opaw-0.4.2/opaw/examples/chat.py
+-rw-rw-rw-   0        0        0      457 2023-08-07 06:56:50.000000 opaw-0.4.2/opaw/examples/completion.py
+-rw-rw-rw-   0        0        0      574 2023-08-07 09:46:04.000000 opaw-0.4.2/opaw/examples/edit.py
+-rw-rw-rw-   0        0        0      476 2023-08-07 06:58:39.000000 opaw-0.4.2/opaw/examples/embedding.py
+-rw-rw-rw-   0        0        0      658 2023-08-07 06:59:42.000000 opaw-0.4.2/opaw/examples/file.py
+-rw-rw-rw-   0        0        0      601 2023-08-07 07:04:07.000000 opaw-0.4.2/opaw/examples/finetune.py
+-rw-rw-rw-   0        0        0      743 2023-08-07 09:09:21.000000 opaw-0.4.2/opaw/examples/funcs.py
+-rw-rw-rw-   0        0        0      775 2023-08-08 08:24:39.000000 opaw-0.4.2/opaw/examples/function_call.py
+-rw-rw-rw-   0        0        0      453 2023-08-07 07:05:59.000000 opaw-0.4.2/opaw/examples/image.py
+-rw-rw-rw-   0        0        0      510 2023-08-07 07:06:55.000000 opaw-0.4.2/opaw/examples/load-chat.py
+-rw-rw-rw-   0        0        0      718 2023-08-07 06:25:24.000000 opaw-0.4.2/opaw/examples/moderation.py
+-rw-rw-rw-   0        0        0       56 2023-08-08 17:03:19.000000 opaw-0.4.2/opaw/main.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.930434 opaw-0.4.2/opaw/model/
+-rw-rw-rw-   0        0        0        0 2023-08-07 05:55:31.000000 opaw-0.4.2/opaw/model/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/audio.py
+-rw-rw-rw-   0        0        0     2062 2023-08-06 14:16:59.000000 opaw-0.4.2/opaw/model/bot.py
+-rw-rw-rw-   0        0        0     3796 2023-08-08 16:54:09.000000 opaw-0.4.2/opaw/model/chat.py
+-rw-rw-rw-   0        0        0      667 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/completion.py
+-rw-rw-rw-   0        0        0      763 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/edit.py
+-rw-rw-rw-   0        0        0      656 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/embedding.py
+-rw-rw-rw-   0        0        0     1238 2023-08-08 16:54:09.000000 opaw-0.4.2/opaw/model/file.py
+-rw-rw-rw-   0        0        0     1050 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/finetune.py
+-rw-rw-rw-   0        0        0     1285 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/image.py
+-rw-rw-rw-   0        0        0      665 2023-08-08 17:00:53.000000 opaw-0.4.2/opaw/model/moderation.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.938013 opaw-0.4.2/opaw/test/
+-rw-rw-rw-   0        0        0        0 2023-07-31 12:07:48.000000 opaw-0.4.2/opaw/test/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 05:57:37.000000 opaw-0.4.2/opaw/test/test.py
+-rw-rw-rw-   0        0        0       47 2023-08-06 07:05:13.000000 opaw-0.4.2/opaw/test/test2.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.943885 opaw-0.4.2/opaw/util/
+-rw-rw-rw-   0        0        0     2633 2023-08-08 17:15:46.000000 opaw-0.4.2/opaw/util/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-08-08 17:15:16.000000 opaw-0.4.2/opaw/util/log.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:20:54.838634 opaw-0.4.2/opaw.egg-info/
+-rw-rw-rw-   0        0        0     1807 2023-08-08 17:20:54.000000 opaw-0.4.2/opaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-08-08 17:20:54.000000 opaw-0.4.2/opaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 17:20:54.000000 opaw-0.4.2/opaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-08 17:20:54.000000 opaw-0.4.2/opaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-08 17:20:54.000000 opaw-0.4.2/opaw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-08-08 17:20:54.950641 opaw-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-08-08 17:20:48.000000 opaw-0.4.2/setup.py
```

### Comparing `opaw-0.4.1/LICENSE` & `opaw-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/PKG-INFO` & `opaw-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: opaw
-Version: 0.4.1
+Version: 0.4.2
 Summary: Unofficial python wrapper of OpenAI API.
 Home-page: https://github.com/hiimanget/openai-pw
 Author: hiimanget
 Author-email: hiimanget@gmail.com
 License: MIT
 Keywords: openai,python,api,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPi](https://img.shields.io/pypi/v/opaw)](https://pypi.org/project/opaw/)
+
+
 # openai-pw
 Unofficial python wrapper of [OpenAI](https://openai.com/) API.
 
 
 # Features
 - Wrapped models (chat, audio, image, embeddings ...)
-- History save and load
+- History(conversations) save and load
 
 
 # Quick start
 You can also play with in [this colab](https://colab.research.google.com/drive/1nJ1-YwLMSxSVx092uBVoarvuVUyt65xC?usp=drive_link). Or
 
 1. Download `openai` and [`opaw`](https://pypi.org/project/opaw/) using pip. 
 ```cmd
```

### Comparing `opaw-0.4.1/README.md` & `opaw-0.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+[![PyPi](https://img.shields.io/pypi/v/opaw)](https://pypi.org/project/opaw/)
+
+
 # openai-pw
 Unofficial python wrapper of [OpenAI](https://openai.com/) API.
 
 
 # Features
 - Wrapped models (chat, audio, image, embeddings ...)
-- History save and load
+- History(conversations) save and load
 
 
 # Quick start
 You can also play with in [this colab](https://colab.research.google.com/drive/1nJ1-YwLMSxSVx092uBVoarvuVUyt65xC?usp=drive_link). Or
 
 1. Download `openai` and [`opaw`](https://pypi.org/project/opaw/) using pip. 
 ```cmd
```

### Comparing `opaw-0.4.1/opaw/examples/audio.py` & `opaw-0.4.2/opaw/examples/audio.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/basic.py` & `opaw-0.4.2/opaw/examples/basic.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/edit.py` & `opaw-0.4.2/opaw/examples/edit.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/file.py` & `opaw-0.4.2/opaw/examples/file.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/finetune.py` & `opaw-0.4.2/opaw/examples/finetune.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/funcs.py` & `opaw-0.4.2/opaw/examples/funcs.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/function_call.py` & `opaw-0.4.2/opaw/examples/function_call.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/examples/moderation.py` & `opaw-0.4.2/opaw/examples/moderation.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/model/audio.py` & `opaw-0.4.2/opaw/model/audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 class AudioBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/audio
     """
 
-    def __init__(self, model="whisper-1"):
+    def __init__(self, model=util.default_models["audio"]):
         super().__init__(model, "audio")
 
     def create(self, file, **kargs):
         """
         :kargs: select task "stt(transcript)" or "mt(translation)"
 
         language (stt): https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
```

### Comparing `opaw-0.4.1/opaw/model/bot.py` & `opaw-0.4.2/opaw/model/bot.py`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/opaw/model/chat.py` & `opaw-0.4.2/opaw/model/chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 import copy
 import io
 import json
 import openai
-from opaw.model import bot
+from opaw.model.bot import Bot
+from opaw import util
 
 
-class ChatBot(bot.Bot):
+class ChatBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/chat
     """
 
-    def __init__(self, model="gpt-3.5-turbo", messages=None, funcs=None, funcs_meta=None):
+    def __init__(self, model=util.default_models["chat"],
+                 messages=None, funcs=None, funcs_meta=None):
         super().__init__(model, "chat")
         # conversations
         self.messages = [] if messages is None else messages
         self.funcs = [] if funcs is None else funcs  # callback functions
         self.funcs_meta = [] if funcs_meta is None else funcs_meta  # contains name, desc, params...
 
-    def create(self, content=None, **kargs):
+    def create(self, content=None, call_fn=False, msg_limit=-1, **kargs):
         """
         Gets a response from bot
         :param content: get a response with messages (content)
+        :param call_fn: if true, function call will be enabled
+        :param msg_limit: number of recent message limit (if -1, no limit)
         :param kargs: other args (if call_fn is True, self.funcs_info will be passed to "functions")
         :return:
         """
         # default
         role = kargs["role"] if kargs.get("role") else "user"
 
-        if "call_fn" in kargs and kargs["call_fn"]:  # if call_fn is True
-            kargs.pop("call_fn")
-            kargs["functions"] = self.funcs_meta
+        # options
+        if call_fn:
+            kargs["functions"] = self.funcs_meta  # pass functions meta info
+        if msg_limit != -1:
+            if msg_limit == 0:
+                self.messages.clear()
+            else:
+                self.messages = self.messages[-msg_limit:]
+
 
         if content is not None:
             content = str(content)
             self.add_message(content, role=role)
 
         request = {
             "model": self.model,
@@ -99,7 +109,8 @@
 
         # load messages of the last request
         self.messages = next((item["messages"] for item in hist[::-1] if "messages" in item), [])
 
         # insert last response to messages
         last_res_msg = next((self._get_res_msg(item) for item in hist[::-1] if "choices" in item), None)
         self.messages.append(last_res_msg)
+
```

### Comparing `opaw-0.4.1/opaw/model/completion.py` & `opaw-0.4.2/opaw/model/completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 class CompletionBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/completions
     """
-    def __init__(self, model="text-davinci-003"):
+    def __init__(self, model=util.default_models["completion"]):
         super().__init__(model, "completion")
 
     def create(self, prompt, **kargs):
         if prompt is None:
             return None
 
         request = {
```

### Comparing `opaw-0.4.1/opaw/model/edit.py` & `opaw-0.4.2/opaw/model/edit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 
 class EditBot(Bot):
     """
     Deprecated model
 
     https://platform.openai.com/docs/api-reference/edits
     """
 
-    def __init__(self, model="text-davinci-edit-001"):
+    def __init__(self, model=util.default_models["edit"]):
         """
         Deprecated model
         """
         super().__init__(model, "edit")
 
     def create(self, input, **kargs):
         """
```

### Comparing `opaw-0.4.1/opaw/model/file.py` & `opaw-0.4.2/opaw/model/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 
 class FileBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/files
     """
```

### Comparing `opaw-0.4.1/opaw/model/finetune.py` & `opaw-0.4.2/opaw/model/finetune.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 
 class FinetuneBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/fine-tunes
     """
 
-    def __init__(self, model="curie"):
+    def __init__(self, model=util.default_models["finetune"]):
         super().__init__(model, "finetune")
 
     def create(self, _=None, **kargs):
         """
         :param _: is not used (use kargs instead)
         """
         if not kargs.get("task"):
```

### Comparing `opaw-0.4.1/opaw/model/image.py` & `opaw-0.4.2/opaw/model/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 
 class ImageBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/images
     """
 
-    def __init__(self, model="DALL-E"):
+    def __init__(self, model=util.default_models["image"]):
         super().__init__(model, "image")
 
     def create(self, prompt, **kargs):
         """
         :kargs: select task "create" or "edit" or "variation"
         """
         if prompt is None or not kargs.get("task"):
```

### Comparing `opaw-0.4.1/opaw/model/moderation.py` & `opaw-0.4.2/opaw/model/moderation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import openai
 from opaw.model.bot import Bot
+from opaw import util
 
 
 class ModerationBot(Bot):
     """
     https://platform.openai.com/docs/api-reference/moderations
     """
 
-    def __init__(self, model="text-moderation-latest"):
+    def __init__(self, model=util.default_models["moderation"]):
         super().__init__(model, "moderation")
 
     def create(self, input, **kargs):
         if input is None:
             return None
 
         request = {
```

### Comparing `opaw-0.4.1/opaw/util/__init__.py` & `opaw-0.4.2/opaw/util/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,63 @@
+import logging
+from opaw.util import log
 import time
 import copy
 import json
 import os
 from os.path import join
 from datetime import datetime
 import openai
 import traceback
 
+default_models = {
+    "chat": "gpt-3.5-turbo",
+    "completion": "text-davinci-003",
+    "image": "DALL-E",
+    "audio": "whisper-1",
+    "embedding": "text-embedding-ada-002",
+    "file": "",
+    "finetune": "curie",
+    "moderation": "text-moderation-latest",
+    "edit": "text-davinci-edit-001"
+}
+
 
 def setup(api_key_file="openai-api-key.txt"):
+    logger = log.get("opaw")
+    # remove logger file handler
+    logger.handlers = [h for h in logger.handlers if not isinstance(h, logging.FileHandler)]
+
     key = None
     try:
         with open(api_key_file) as file:
             key = file.read()
     except FileNotFoundError:
-        print(f"No file: {api_key_file} for openai api key.")
-        print("Searching environment variable: \"OPENAI_API_KEY\"...")
+        logger.warning(f"No file: {api_key_file} for openai api key.")
+        logger.warning("Searching environment variable: \"OPENAI_API_KEY\"...")
 
         # env var
         key = os.environ.get("OPENAI_API_KEY")
         if key is None:
-            print("There's no environment variable: \"OPENAI_API_KEY\".")
+            logger.warning("There's no environment variable: \"OPENAI_API_KEY\".")
     finally:
         if key is None:
-            print("Failed to find openai api key.")
-            print(f"Create a \"{api_key_file}\" file or set environment variable: \"OPENAI_API_KEY\".")
+            logger.warning("Failed to find openai api key.")
+            logger.warning(f"Create a \"{api_key_file}\" file or set environment variable: \"OPENAI_API_KEY\".")
         else:
             try:
                 openai.api_key = key
-                print("OpenAI API key is setup!")
+                logger.info("OpenAI API key is setup!")
                 openai.Model.list()  # test for the api_key is valid or not
             except Exception as e:
                 traceback.print_exc()
                 time.sleep(0.1)
-                print("Your API key has a problem. Check here: "
-                      "https://platform.openai.com/docs/guides/error-codes/api-errors")
+                logger.warning("Your API key has a problem. Check here: "
+                               "https://platform.openai.com/docs/guides/error-codes/api-errors")
+
 
 def models():
     r = openai.Model.list()
     return [model["id"] for model in r["data"]]
 
 
 def mkdirs(file):
@@ -67,9 +86,7 @@
 
 
 def pprints(d):
     """
     Pretty print string
     """
     return json.dumps(d, indent="\t")
-
-
```

### Comparing `opaw-0.4.1/opaw/util/log.py` & `opaw-0.4.2/opaw/util/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
-from opaw.util import mkdirs
+
 
 def get(name, file="./log.log"):
+    from opaw.util import mkdirs
     """
     Gets a logger with the given name (singleton)
     :param name: logger name
     :param file: the file logs will be saved (default: ./log.log)
     """
     logger = logging.getLogger(name)
 
     if not logger.hasHandlers():
         # make parent dirs if needed
         mkdirs(file)
-
         logger.setLevel(logging.INFO)
 
         # stream handler
         stream_formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] %(message)s")
         stream_handler = logging.StreamHandler()
         stream_handler.setFormatter(stream_formatter)
         stream_handler.setLevel(logging.INFO)
```

### Comparing `opaw-0.4.1/opaw.egg-info/PKG-INFO` & `opaw-0.4.2/opaw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: opaw
-Version: 0.4.1
+Version: 0.4.2
 Summary: Unofficial python wrapper of OpenAI API.
 Home-page: https://github.com/hiimanget/openai-pw
 Author: hiimanget
 Author-email: hiimanget@gmail.com
 License: MIT
 Keywords: openai,python,api,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPi](https://img.shields.io/pypi/v/opaw)](https://pypi.org/project/opaw/)
+
+
 # openai-pw
 Unofficial python wrapper of [OpenAI](https://openai.com/) API.
 
 
 # Features
 - Wrapped models (chat, audio, image, embeddings ...)
-- History save and load
+- History(conversations) save and load
 
 
 # Quick start
 You can also play with in [this colab](https://colab.research.google.com/drive/1nJ1-YwLMSxSVx092uBVoarvuVUyt65xC?usp=drive_link). Or
 
 1. Download `openai` and [`opaw`](https://pypi.org/project/opaw/) using pip. 
 ```cmd
```

### Comparing `opaw-0.4.1/opaw.egg-info/SOURCES.txt` & `opaw-0.4.2/opaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opaw-0.4.1/setup.py` & `opaw-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # pypi long description
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='opaw',
     packages=find_packages(),
-    version='0.4.1',
+    version='0.4.2',
     license='MIT',
     description='Unofficial python wrapper of OpenAI API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='hiimanget',
     author_email='hiimanget@gmail.com',
     url='https://github.com/hiimanget/openai-pw',
```


# Comparing `tmp/iamlistening-3.3.0.tar.gz` & `tmp/iamlistening-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.3.0.tar", max compression
+gzip compressed data, was "iamlistening-3.3.1.tar", max compression
```

## Comparing `iamlistening-3.3.0.tar` & `iamlistening-3.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2023-08-07 21:50:55.853194 iamlistening-3.3.0/LICENSE
--rw-r--r--   0        0        0     2457 2023-08-07 21:50:55.853194 iamlistening-3.3.0/README.md
--rw-r--r--   0        0        0       81 2023-08-07 21:50:57.769223 iamlistening-3.3.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      688 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/config.py
--rw-r--r--   0        0        0     1376 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1673 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0     3513 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/chat_manager.py
--rw-r--r--   0        0        0       68 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/__init__.py
--rw-r--r--   0        0        0      876 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/discord.py
--rw-r--r--   0        0        0      738 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/guilded.py
--rw-r--r--   0        0        0      867 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/lemmy.py
--rw-r--r--   0        0        0     1349 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/mastodon.py
--rw-r--r--   0        0        0     1616 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/matrix.py
--rw-r--r--   0        0        0      912 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/revolt.py
--rw-r--r--   0        0        0      806 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/rocket_chat.py
--rw-r--r--   0        0        0     1176 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/telegram.py
--rw-r--r--   0        0        0      568 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/tinode.py
--rw-r--r--   0        0        0      784 2023-08-07 21:50:55.861194 iamlistening-3.3.0/iamlistening/platform/clients/twitch.py
--rw-r--r--   0        0        0     3390 2023-08-07 21:50:57.761223 iamlistening-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 iamlistening-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-08 12:27:36.321630 iamlistening-3.3.1/LICENSE
+-rw-r--r--   0        0        0     2457 2023-08-08 12:27:36.321630 iamlistening-3.3.1/README.md
+-rw-r--r--   0        0        0       81 2023-08-08 12:27:38.297627 iamlistening-3.3.1/iamlistening/__init__.py
+-rw-r--r--   0        0        0      686 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/config.py
+-rw-r--r--   0        0        0     1277 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1673 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/main.py
+-rw-r--r--   0        0        0        0 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0     3514 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/chat_manager.py
+-rw-r--r--   0        0        0       68 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/__init__.py
+-rw-r--r--   0        0        0      876 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/discord.py
+-rw-r--r--   0        0        0      738 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/guilded.py
+-rw-r--r--   0        0        0      867 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/lemmy.py
+-rw-r--r--   0        0        0     1349 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/mastodon.py
+-rw-r--r--   0        0        0     1616 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/matrix.py
+-rw-r--r--   0        0        0      858 2023-08-08 12:27:36.325630 iamlistening-3.3.1/iamlistening/platform/clients/revolt.py
+-rw-r--r--   0        0        0      806 2023-08-08 12:27:36.329630 iamlistening-3.3.1/iamlistening/platform/clients/rocket_chat.py
+-rw-r--r--   0        0        0     1176 2023-08-08 12:27:36.329630 iamlistening-3.3.1/iamlistening/platform/clients/telegram.py
+-rw-r--r--   0        0        0      568 2023-08-08 12:27:36.329630 iamlistening-3.3.1/iamlistening/platform/clients/tinode.py
+-rw-r--r--   0        0        0      784 2023-08-08 12:27:36.329630 iamlistening-3.3.1/iamlistening/platform/clients/twitch.py
+-rw-r--r--   0        0        0     3390 2023-08-08 12:27:38.289627 iamlistening-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 iamlistening-3.3.1/PKG-INFO
```

### Comparing `iamlistening-3.3.0/LICENSE` & `iamlistening-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/README.md` & `iamlistening-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/config.py` & `iamlistening-3.3.1/iamlistening/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,10 +20,10 @@
         'settings.toml',
         '.secrets.toml'
     ],
     # Load the.env file
     load_dotenv=True,
     # Set the environments to True
     environments=True,
-    # merge_enabled=True,
+    merge_enabled=True,
     # Set the default environment
     default_env="default",)
```

### Comparing `iamlistening-3.3.0/iamlistening/main.py` & `iamlistening-3.3.1/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/chat_manager.py` & `iamlistening-3.3.1/iamlistening/platform/chat_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
             from .clients.lemmy import LemmyHandler
 
             handler = LemmyHandler()
         elif platform == "twitch":
             from .clients.twitch import TwitchHandler
 
             handler = TwitchHandler()
+
         return handler
 
     def __init__(self):
         """
         Initialize the chat manager.
         """
         self.platform = None
```

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/discord.py` & `iamlistening-3.3.1/iamlistening/platform/clients/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/guilded.py` & `iamlistening-3.3.1/iamlistening/platform/clients/guilded.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/lemmy.py` & `iamlistening-3.3.1/iamlistening/platform/clients/lemmy.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/mastodon.py` & `iamlistening-3.3.1/iamlistening/platform/clients/mastodon.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/matrix.py` & `iamlistening-3.3.1/iamlistening/platform/clients/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/revolt.py` & `iamlistening-3.3.1/iamlistening/platform/clients/revolt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-# """
-# Revolt  🇷
-# """
+"""
+Revolt  🇷
+"""
 # import asyncio
 
 # import aiohttp
 # import revolt
 # from loguru import logger
 
 # from iamlistening.config import settings
 # from iamlistening.platform.chat_manager import ChatManager
 
 
 # class RevoltHandler(ChatManager):
-
 #     def __init__(self):
 #         """
 #         Initialize the Revolt handler.
 #         """
 #         super().__init__()
+#         session = aiohttp.ClientSession()
+#         self.bot = revolt.Client(session, settings.bot_token)
+#         logger.debug(self.bot.api_info)
+#         self.connected()
 
 #     async def start(self):
 #         """
 #         Start the Revolt handler.
 #         """
 #         logger.debug("Revolt setup")
-#         self.bot = revolt.Client(revolt.utils.client_session(), settings.bot_token)
-#         logger.debug(self.bot.api_info)
-#         await self.bot.start()
 
-#         # @self.bot.event
-#         # async def on_ready():
-#         #     self.connected()
+#         await self.bot.start()
 
 #         @self.bot.event
 #         async def on_message(self, message: revolt.Message):
 #             await self.handle_message(message.content)
-
```

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/rocket_chat.py` & `iamlistening-3.3.1/iamlistening/platform/clients/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/telegram.py` & `iamlistening-3.3.1/iamlistening/platform/clients/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/tinode.py` & `iamlistening-3.3.1/iamlistening/platform/clients/tinode.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/iamlistening/platform/clients/twitch.py` & `iamlistening-3.3.1/iamlistening/platform/clients/twitch.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.3.0/pyproject.toml` & `iamlistening-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.3.0"
+version = "3.3.1"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
```

### Comparing `iamlistening-3.3.0/PKG-INFO` & `iamlistening-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.3.0
+Version: 3.3.1
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.3.0 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.3.1 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Mastodon.py
 (>=1.8.1,<2.0.0) Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist:
```


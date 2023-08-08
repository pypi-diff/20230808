# Comparing `tmp/pybotterfly-0.1.5.tar.gz` & `tmp/pybotterfly-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotterfly-0.1.5.tar", max compression
+gzip compressed data, was "pybotterfly-0.1.6.tar", max compression
```

## Comparing `pybotterfly-0.1.5.tar` & `pybotterfly-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-08-03 11:43:05.291935 pybotterfly-0.1.5/LICENSE
--rw-r--r--   0        0        0      590 2023-08-03 11:43:05.292022 pybotterfly-0.1.5/README.md
--rw-r--r--   0        0        0       87 2023-08-03 11:43:05.295801 pybotterfly-0.1.5/pybotterfly/__init__.py
--rw-r--r--   0        0        0     2273 2023-08-03 11:43:05.295893 pybotterfly-0.1.5/pybotterfly/base_config.py
--rw-r--r--   0        0        0      186 2023-08-03 11:43:05.296033 pybotterfly-0.1.5/pybotterfly/bot/__init__.py
--rw-r--r--   0        0        0     3556 2023-08-03 11:43:05.296134 pybotterfly-0.1.5/pybotterfly/bot/converters.py
--rw-r--r--   0        0        0      577 2023-08-03 11:43:05.296212 pybotterfly-0.1.5/pybotterfly/bot/downloaders.py
--rw-r--r--   0        0        0      844 2023-08-03 11:43:05.296280 pybotterfly-0.1.5/pybotterfly/bot/logger.py
--rw-r--r--   0        0        0       29 2023-08-03 11:43:05.296379 pybotterfly-0.1.5/pybotterfly/bot/reply/__init__.py
--rw-r--r--   0        0        0    10771 2023-08-03 11:43:05.296487 pybotterfly-0.1.5/pybotterfly/bot/reply/default_reply_types.py
--rw-r--r--   0        0        0     6840 2023-08-03 11:43:05.296584 pybotterfly-0.1.5/pybotterfly/bot/reply/reply_division.py
--rw-r--r--   0        0        0       44 2023-08-03 11:43:05.296699 pybotterfly-0.1.5/pybotterfly/bot/returns/__init__.py
--rw-r--r--   0        0        0    10173 2023-08-03 11:43:05.296800 pybotterfly-0.1.5/pybotterfly/bot/returns/buttons.py
--rw-r--r--   0        0        0     3351 2023-08-03 11:43:05.296882 pybotterfly-0.1.5/pybotterfly/bot/returns/message.py
--rw-r--r--   0        0        0     1430 2023-08-03 11:43:05.296971 pybotterfly-0.1.5/pybotterfly/bot/struct.py
--rw-r--r--   0        0        0     5129 2023-08-03 11:43:05.297060 pybotterfly-0.1.5/pybotterfly/bot/throttlers.py
--rw-r--r--   0        0        0       72 2023-08-03 11:43:05.297166 pybotterfly-0.1.5/pybotterfly/bot/transitions/__init__.py
--rw-r--r--   0        0        0    32721 2023-08-03 11:43:05.297375 pybotterfly-0.1.5/pybotterfly/bot/transitions/payloads.py
--rw-r--r--   0        0        0      547 2023-08-03 11:43:05.297703 pybotterfly-0.1.5/pybotterfly/bot/transitions/schedule.py
--rw-r--r--   0        0        0    19811 2023-08-03 11:43:05.297873 pybotterfly-0.1.5/pybotterfly/bot/transitions/transitions.py
--rw-r--r--   0        0        0       51 2023-08-03 11:43:05.297993 pybotterfly-0.1.5/pybotterfly/message_handler/__init__.py
--rw-r--r--   0        0        0     6837 2023-08-03 11:43:05.298115 pybotterfly-0.1.5/pybotterfly/message_handler/message_handler.py
--rw-r--r--   0        0        0      693 2023-08-03 11:43:05.298179 pybotterfly-0.1.5/pybotterfly/message_handler/struct.py
--rw-r--r--   0        0        0       48 2023-08-03 11:43:05.298287 pybotterfly-0.1.5/pybotterfly/runners/__init__.py
--rw-r--r--   0        0        0    10089 2023-08-03 11:43:05.298416 pybotterfly-0.1.5/pybotterfly/runners/tg_client.py
--rw-r--r--   0        0        0     8956 2023-08-03 11:43:05.298526 pybotterfly-0.1.5/pybotterfly/runners/vk_client.py
--rw-r--r--   0        0        0       47 2023-08-03 11:43:05.298623 pybotterfly-0.1.5/pybotterfly/server/__init__.py
--rw-r--r--   0        0        0     6414 2023-08-03 11:43:05.298720 pybotterfly-0.1.5/pybotterfly/server/server.py
--rw-r--r--   0        0        0      892 2023-08-03 11:43:05.298791 pybotterfly-0.1.5/pybotterfly/server/server_func.py
--rw-r--r--   0        0        0     1933 2023-08-03 11:43:05.298879 pybotterfly-0.1.5/pybotterfly/server/struct.py
--rw-r--r--   0        0        0      494 2023-08-03 12:48:51.105218 pybotterfly-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 pybotterfly-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-03 11:43:05.291935 pybotterfly-0.1.6/LICENSE
+-rw-r--r--   0        0        0      748 2023-08-08 08:56:17.734272 pybotterfly-0.1.6/README.md
+-rw-r--r--   0        0        0       87 2023-08-03 11:43:05.295801 pybotterfly-0.1.6/pybotterfly/__init__.py
+-rw-r--r--   0        0        0     2273 2023-08-03 11:43:05.295893 pybotterfly-0.1.6/pybotterfly/base_config.py
+-rw-r--r--   0        0        0      186 2023-08-03 11:43:05.296033 pybotterfly-0.1.6/pybotterfly/bot/__init__.py
+-rw-r--r--   0        0        0     3556 2023-08-03 11:43:05.296134 pybotterfly-0.1.6/pybotterfly/bot/converters.py
+-rw-r--r--   0        0        0      577 2023-08-03 11:43:05.296212 pybotterfly-0.1.6/pybotterfly/bot/downloaders.py
+-rw-r--r--   0        0        0      844 2023-08-03 11:43:05.296280 pybotterfly-0.1.6/pybotterfly/bot/logger.py
+-rw-r--r--   0        0        0       29 2023-08-03 11:43:05.296379 pybotterfly-0.1.6/pybotterfly/bot/reply/__init__.py
+-rw-r--r--   0        0        0    10771 2023-08-03 11:43:05.296487 pybotterfly-0.1.6/pybotterfly/bot/reply/default_reply_types.py
+-rw-r--r--   0        0        0     6840 2023-08-03 11:43:05.296584 pybotterfly-0.1.6/pybotterfly/bot/reply/reply_division.py
+-rw-r--r--   0        0        0       44 2023-08-03 11:43:05.296699 pybotterfly-0.1.6/pybotterfly/bot/returns/__init__.py
+-rw-r--r--   0        0        0    10173 2023-08-03 11:43:05.296800 pybotterfly-0.1.6/pybotterfly/bot/returns/buttons.py
+-rw-r--r--   0        0        0     3351 2023-08-03 11:43:05.296882 pybotterfly-0.1.6/pybotterfly/bot/returns/message.py
+-rw-r--r--   0        0        0     1430 2023-08-03 11:43:05.296971 pybotterfly-0.1.6/pybotterfly/bot/struct.py
+-rw-r--r--   0        0        0     5129 2023-08-03 11:43:05.297060 pybotterfly-0.1.6/pybotterfly/bot/throttlers.py
+-rw-r--r--   0        0        0       72 2023-08-03 11:43:05.297166 pybotterfly-0.1.6/pybotterfly/bot/transitions/__init__.py
+-rw-r--r--   0        0        0    32721 2023-08-03 11:43:05.297375 pybotterfly-0.1.6/pybotterfly/bot/transitions/payloads.py
+-rw-r--r--   0        0        0      547 2023-08-03 11:43:05.297703 pybotterfly-0.1.6/pybotterfly/bot/transitions/schedule.py
+-rw-r--r--   0        0        0    19811 2023-08-03 11:43:05.297873 pybotterfly-0.1.6/pybotterfly/bot/transitions/transitions.py
+-rw-r--r--   0        0        0       51 2023-08-03 11:43:05.297993 pybotterfly-0.1.6/pybotterfly/message_handler/__init__.py
+-rw-r--r--   0        0        0     6837 2023-08-03 11:43:05.298115 pybotterfly-0.1.6/pybotterfly/message_handler/message_handler.py
+-rw-r--r--   0        0        0      693 2023-08-03 11:43:05.298179 pybotterfly-0.1.6/pybotterfly/message_handler/struct.py
+-rw-r--r--   0        0        0       48 2023-08-03 11:43:05.298287 pybotterfly-0.1.6/pybotterfly/runners/__init__.py
+-rw-r--r--   0        0        0    10585 2023-08-08 08:36:29.804244 pybotterfly-0.1.6/pybotterfly/runners/tg_client.py
+-rw-r--r--   0        0        0     9276 2023-08-08 08:36:29.804594 pybotterfly-0.1.6/pybotterfly/runners/vk_client.py
+-rw-r--r--   0        0        0       47 2023-08-03 11:43:05.298623 pybotterfly-0.1.6/pybotterfly/server/__init__.py
+-rw-r--r--   0        0        0     6414 2023-08-03 11:43:05.298720 pybotterfly-0.1.6/pybotterfly/server/server.py
+-rw-r--r--   0        0        0      892 2023-08-03 11:43:05.298791 pybotterfly-0.1.6/pybotterfly/server/server_func.py
+-rw-r--r--   0        0        0     1933 2023-08-03 11:43:05.298879 pybotterfly-0.1.6/pybotterfly/server/struct.py
+-rw-r--r--   0        0        0      398 2023-08-08 09:05:21.145020 pybotterfly-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 pybotterfly-0.1.6/PKG-INFO
```

### Comparing `pybotterfly-0.1.5/LICENSE` & `pybotterfly-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/README.md` & `pybotterfly-0.1.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 ## Description
 
-Build multi-messenger chatbots with ease using our scalable Python library, designed to simplify listener integration for various platforms
+Build multi-messenger chatbots with ease using our scalable Python framework, designed to simplify listener integration for various platforms
 
 ## Installation 
 
+#### Via [GitHub](https://github.com/Ninzalo/PyBotterfly.git)
 ```shell
 pip install git+https://github.com/Ninzalo/PyBotterfly.git
 ```
 
+#### Via [PyPI](https://pypi.org/project/pybotterfly/)
+```shell
+pip install pybotterfly
+```
+
+
 ## Example usage
 
 - [Example](https://github.com/Ninzalo/PyBotterfly/blob/master/docs/example.md)
 
 ## Configuration documentation
 
 - [Configuration](https://github.com/Ninzalo/PyBotterfly/blob/master/docs/configuration.md)
```

### Comparing `pybotterfly-0.1.5/pybotterfly/base_config.py` & `pybotterfly-0.1.6/pybotterfly/base_config.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/converters.py` & `pybotterfly-0.1.6/pybotterfly/bot/converters.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/downloaders.py` & `pybotterfly-0.1.6/pybotterfly/bot/downloaders.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/logger.py` & `pybotterfly-0.1.6/pybotterfly/bot/logger.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/reply/default_reply_types.py` & `pybotterfly-0.1.6/pybotterfly/bot/reply/default_reply_types.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/reply/reply_division.py` & `pybotterfly-0.1.6/pybotterfly/bot/reply/reply_division.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/returns/buttons.py` & `pybotterfly-0.1.6/pybotterfly/bot/returns/buttons.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/returns/message.py` & `pybotterfly-0.1.6/pybotterfly/bot/returns/message.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/struct.py` & `pybotterfly-0.1.6/pybotterfly/bot/struct.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/throttlers.py` & `pybotterfly-0.1.6/pybotterfly/bot/throttlers.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/transitions/payloads.py` & `pybotterfly-0.1.6/pybotterfly/bot/transitions/payloads.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/transitions/schedule.py` & `pybotterfly-0.1.6/pybotterfly/bot/transitions/schedule.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/bot/transitions/transitions.py` & `pybotterfly-0.1.6/pybotterfly/bot/transitions/transitions.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/message_handler/message_handler.py` & `pybotterfly-0.1.6/pybotterfly/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/message_handler/struct.py` & `pybotterfly-0.1.6/pybotterfly/message_handler/struct.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/runners/tg_client.py` & `pybotterfly-0.1.6/pybotterfly/runners/tg_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,30 +66,47 @@
         await self.server_sender(message_struct=message_struct)
 
     async def file_handler(self, message: types.Message) -> None:
         message_struct = MessageStruct(
             user_id=message.from_id, messenger="tg", text=message.text
         )
         if message.document != None:
-            doc_ext = (
-                f".{str(message.document.file_name).split('.')[-1]}".lower()
+            message_file = await self._file_downloader(
+                message_file=message.document
             )
-            if doc_ext in self._config.ALLOWED_FILE_EXTENSIONS_LIST:
-                file_in_io = BytesIO()
-                await message.document.download(destination_file=file_in_io)
-                message_struct.files.append(
-                    File(
-                        name=f"{message.document.file_name}",
-                        tag="document",
-                        ext=doc_ext,
-                        file_bytes=file_to_string(file_in_io.getvalue()),
-                    )
-                )
+            if message_file != None:
+                message_struct.files.append(message_file)
         await self.server_sender(message_struct=message_struct)
 
+    async def _file_downloader(
+        self, message_file: types.document.Document
+    ) -> File | None:
+        doc_ext = f".{str(message_file.file_name).split('.')[-1]}".lower()
+        if doc_ext not in self._config.ALLOWED_FILE_EXTENSIONS_LIST:
+            return
+        if message_file.file_size >= 50 * 1024 * 1024:
+            self._logger.log(
+                log=Log(
+                    level="ERROR",
+                    text=(
+                        f"Skipping file with size: "
+                        f"{message_file.file_size}"
+                    ),
+                )
+            )
+            return
+        file_in_io = BytesIO()
+        await message_file.download(destination_file=file_in_io)
+        return File(
+            name=f"{message_file.file_name}",
+            tag="document",
+            ext=doc_ext,
+            file_bytes=file_to_string(file_in_io.getvalue()),
+        )
+
     async def message_handler(self, message: types.Message) -> None:
         message_struct = MessageStruct(
             user_id=message.from_id, messenger="tg", text=message.text
         )
         await self.server_sender(message_struct=message_struct)
 
     async def server_sender(self, message_struct: MessageStruct) -> None:
```

### Comparing `pybotterfly-0.1.5/pybotterfly/runners/vk_client.py` & `pybotterfly-0.1.6/pybotterfly/runners/vk_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pybotterfly.bot.converters import file_to_string
 from pybotterfly.server.server_func import send_to_server
 from pybotterfly.bot.logger import BaseLogger, Log, DefaultLogger
 
 # Vk async library
 from vkbottle import GroupEventType
 from vkbottle.bot import Message, MessageEvent, Bot
+from vkbottle_types.codegen.objects import DocsDoc
 
 
 class VkClient:
     def __init__(
         self,
         handler: Bot,
         local_ip: str,
@@ -55,15 +56,15 @@
             payload = json.loads(event.payload)
             if payload == {"command": "start"}:
                 payload = None
         files = []
         for message_file in event.attachments:
             if message_file.doc != None:
                 doc_file = await self._file_downloader(
-                    message_file=message_file
+                    message_file=message_file.doc
                 )
                 if doc_file != None:
                     files.append(doc_file)
             if message_file.photo != None:
                 photo_file = await self._photo_downloader(
                     message_file=message_file
                 )
@@ -79,25 +80,33 @@
             message.files = files
         await send_to_server(
             message=message,
             local_ip=self._local_ip,
             local_port=self._local_port,
         )
 
-    async def _file_downloader(self, message_file) -> File:
+    async def _file_downloader(self, message_file: DocsDoc) -> File | None:
         if (
-            f".{message_file.doc.ext}"
+            f".{message_file.ext}"
             not in self._config.ALLOWED_FILE_EXTENSIONS_LIST
         ):
             return
-        file_bytes = await download_file(message_file.doc.url)
+        if message_file.size >= 50 * 1024 * 1024:
+            self._logger.log(
+                log=Log(
+                    level="ERROR",
+                    text=f"Skipping file with size: {message_file.size}",
+                )
+            )
+            return
+        file_bytes = await download_file(message_file.url)
         return File(
-            name=message_file.doc.title.split(".")[0],
+            name=message_file.title.split(".")[0],
             tag="document",
-            ext=f".{message_file.doc.ext}".lower(),
+            ext=f".{message_file.ext}".lower(),
             file_bytes=file_to_string(file_bytes),
         )
 
     async def _photo_downloader(self, message_file) -> File:
         file_url = message_file.photo.sizes[-5].url
         photo_ext = str(
             re.search(pattern=r"\.(jpg|jpeg|png)", string=file_url).group(0)
```

### Comparing `pybotterfly-0.1.5/pybotterfly/server/server.py` & `pybotterfly-0.1.6/pybotterfly/server/server.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/server/server_func.py` & `pybotterfly-0.1.6/pybotterfly/server/server_func.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/pybotterfly/server/struct.py` & `pybotterfly-0.1.6/pybotterfly/server/struct.py`

 * *Files identical despite different names*

### Comparing `pybotterfly-0.1.5/PKG-INFO` & `pybotterfly-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pybotterfly
-Version: 0.1.5
-Summary: Build multi-messenger chatbots with ease using our scalable Python library, designed to simplify listener integration for various platforms
+Version: 0.1.6
+Summary: framework for creating multi-messenger bots
 License: MIT
 Author: Ninzalo
 Author-email: k-artemiy@mail.ru
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -13,22 +13,29 @@
 Requires-Dist: black (>=23.7.0,<24.0.0)
 Requires-Dist: emoji (>=2.7.0,<3.0.0)
 Requires-Dist: vkbottle (>=4.3.12,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## Description
 
-Build multi-messenger chatbots with ease using our scalable Python library, designed to simplify listener integration for various platforms
+Build multi-messenger chatbots with ease using our scalable Python framework, designed to simplify listener integration for various platforms
 
 ## Installation 
 
+#### Via [GitHub](https://github.com/Ninzalo/PyBotterfly.git)
 ```shell
 pip install git+https://github.com/Ninzalo/PyBotterfly.git
 ```
 
+#### Via [PyPI](https://pypi.org/project/pybotterfly/)
+```shell
+pip install pybotterfly
+```
+
+
 ## Example usage
 
 - [Example](https://github.com/Ninzalo/PyBotterfly/blob/master/docs/example.md)
 
 ## Configuration documentation
 
 - [Configuration](https://github.com/Ninzalo/PyBotterfly/blob/master/docs/configuration.md)
```


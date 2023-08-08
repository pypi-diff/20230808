# Comparing `tmp/mydm-0.0.2a1.tar.gz` & `tmp/mydm-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mydm-0.0.2a1.tar", max compression
+gzip compressed data, was "mydm-0.0.2a2.tar", max compression
```

## Comparing `mydm-0.0.2a1.tar` & `mydm-0.0.2a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 mydm-0.0.2a1/LICENSE
--rw-r--r--   0        0        0       81 2023-08-07 04:19:21.045728 mydm-0.0.2a1/mydm/__init__.py
--rw-r--r--   0        0        0      417 2023-08-06 11:25:28.254107 mydm-0.0.2a1/mydm/bot.py
--rw-r--r--   0        0        0        0 2023-08-07 03:42:16.350223 mydm-0.0.2a1/mydm/event.py
--rw-r--r--   0        0        0     2113 2023-08-06 11:14:22.597860 mydm-0.0.2a1/mydm/interactor/__init__.py
--rw-r--r--   0        0        0      572 2023-08-07 03:15:54.352056 mydm-0.0.2a1/mydm/interactor/gocqhttp/__init__.py
--rw-r--r--   0        0        0      934 2023-08-07 04:15:10.970991 mydm-0.0.2a1/mydm/interactor/gocqhttp/cqcode.py
--rw-r--r--   0        0        0        0 2023-08-07 04:21:03.253715 mydm-0.0.2a1/mydm/interactor/gocqhttp/event.py
--rw-r--r--   0        0        0        0 2023-08-06 06:10:55.963326 mydm-0.0.2a1/mydm/logger.py
--rw-r--r--   0        0        0      167 2023-08-07 04:18:44.944129 mydm-0.0.2a1/mydm/tool.py
--rw-r--r--   0        0        0      460 2023-08-07 04:21:17.681846 mydm-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0      325 2023-08-06 05:43:25.803070 mydm-0.0.2a1/README.md
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 mydm-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 mydm-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0       81 2023-08-07 04:19:21.045728 mydm-0.0.2a2/mydm/__init__.py
+-rw-r--r--   0        0        0      761 2023-08-07 08:40:03.846659 mydm-0.0.2a2/mydm/bot.py
+-rw-r--r--   0        0        0        0 2023-08-07 03:42:16.350223 mydm-0.0.2a2/mydm/event.py
+-rw-r--r--   0        0        0     2008 2023-08-07 09:10:40.177030 mydm-0.0.2a2/mydm/interactor/__init__.py
+-rw-r--r--   0        0        0     1635 2023-08-07 10:18:33.352972 mydm-0.0.2a2/mydm/interactor/gocqhttp/__init__.py
+-rw-r--r--   0        0        0      934 2023-08-07 04:15:10.970991 mydm-0.0.2a2/mydm/interactor/gocqhttp/cqcode.py
+-rw-r--r--   0        0        0        0 2023-08-07 04:21:03.253715 mydm-0.0.2a2/mydm/interactor/gocqhttp/event.py
+-rw-r--r--   0        0        0        0 2023-08-06 06:10:55.963326 mydm-0.0.2a2/mydm/logger.py
+-rw-r--r--   0        0        0      167 2023-08-07 04:18:44.944129 mydm-0.0.2a2/mydm/tool.py
+-rw-r--r--   0        0        0      460 2023-08-07 10:20:58.161971 mydm-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0      334 2023-08-07 04:51:01.475888 mydm-0.0.2a2/README.md
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 mydm-0.0.2a2/PKG-INFO
```

### Comparing `mydm-0.0.2a1/LICENSE` & `mydm-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mydm-0.0.2a1/mydm/interactor/__init__.py` & `mydm-0.0.2a2/mydm/interactor/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,92 +1,80 @@
 import asyncio
 from abc import ABC, abstractmethod
+from typing import Any, Callable
 
 import aiohttp
 
-from mydm.bot import Bot
-
-
 class Base(ABC):
     def __init__(
         self, url: str, *, 
         access_token: str = ''
         ):
         
         self.url = url
         self.access_token = access_token
         self.session = aiohttp.ClientSession()
-
-
-class Http(Base):
-    @abstractmethod
-    async def send(self, action: str, params: dict) -> dict:
-        '''
-        向OneBot实现发送信息并获取返回值
-        '''
-
-
-class HttpWebhook(Base):
-    @abstractmethod
-    async def start(self):
-        '''
-        启动服务端
-        '''
+        
+        self.echos: list[int] = []
+        self.msgs: list[dict] = []
+        self.bots: list[Callable[[dict], Any]] = []
+        self.conn = False
     
-    @abstractmethod
-    async def receive(self) -> dict:
+    def add_handler(self, bot: Callable[[dict], Any]):
         '''
-        从OneBot实现获取信息
+        添加handler到`self.handlers`
         '''
-
-
-class WebSocketBase(Base):
-    def __init__(
-        self, url: str, bot: Bot, *, 
-        access_token: str = ''
-        ):
-        
-        super().__init__(url, access_token=access_token)
-        self.bot = bot
-        self.conn = False
+        self.bots.append(bot)
     
     @abstractmethod
     async def start(self):
         '''
         连接OneBot实现 或 启动服务端
         '''
     
     @abstractmethod
     async def stop(self):
         '''
         断连OneBot实现 或 关闭服务端
         '''
     
     @abstractmethod
-    async def send(self, action: str, params: dict) -> dict:
+    async def send(self, action: str, params: dict|None = None) -> dict:
         '''
-        向OneBot实现发送信息 并 获取返回值
+        向OneBot实现发送信息
         '''
     
     @abstractmethod
-    async def receive(self):
+    async def _receive(self):
         '''
-        消息接收并送到`self.bot.event`函数处理
+        接收消息并添加到`self.msgs`中
+        '''
+    
+    @abstractmethod
+    async def msg_handler(self):
+        '''
+        处理信息
         '''
 
 
-class WebSocket(WebSocketBase):
+class WebSocket(Base):
     async def start(self):
         self.ws_session = await self.session.ws_connect(self.url)
         self.conn = True
         
         # 连接上后立即开始接收信息
-        asyncio.get_event_loop().create_task(self.receive())
+        asyncio.get_event_loop().create_task(self._receive())
     
     async def stop(self):
         await self.session.close()
         self.conn = False
+        
+    async def _receive(self):
+        while True:
+            msg = await self.ws_session.receive()
+            self.msgs.append(msg.json())
+            await self.msg_handler()
 
 
-class WebSocketReverse(WebSocketBase):
+class WebSocketReverse(Base):
     # 我在这方面不是很熟悉，知道怎么定义的可以发issue或pr
     pass
```

### Comparing `mydm-0.0.2a1/mydm/interactor/gocqhttp/cqcode.py` & `mydm-0.0.2a2/mydm/interactor/gocqhttp/cqcode.py`

 * *Files identical despite different names*

### Comparing `mydm-0.0.2a1/PKG-INFO` & `mydm-0.0.2a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mydm
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: 一个使用OneBot v11/12协议的机器人框架
 Home-page: https://github.com/yuyi2439/MyDM
 License: Apache-2.0
 Author: yuyi2439
 Author-email: yuyi2439@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,13 +13,13 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Project-URL: Repository, https://github.com/yuyi2439/MyDM
 Description-Content-Type: text/markdown
 
 # MyDM
-### 一个使用OneBot v11/12协议的机器人框架
+### 一个使用OneBot v11/12协议的WebSocket机器人框架
 
 ### 本项目使用Apache2.0开源协议
 - 使用本项目时要求保留原始版权和许可声明。同时向贡献者明确授予专利权。
 - 使用者可以自由修改，进行商业使用，可以使用不同的条款分发，没有开源要求。
```


# Comparing `tmp/AiBot.py-1.2.10.tar.gz` & `tmp/AiBot.py-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AiBot.py-1.2.10.tar", last modified: Tue Aug  8 01:37:41 2023, max compression
+gzip compressed data, was "AiBot.py-1.2.9.tar", last modified: Mon Aug  7 10:47:47 2023, max compression
```

## Comparing `AiBot.py-1.2.10.tar` & `AiBot.py-1.2.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-08 01:37:41.911691 AiBot.py-1.2.10/
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-08 01:37:41.906396 AiBot.py-1.2.10/AiBot/
--rw-r--r--   0 chenxun    (501) staff       (20)    57161 2023-08-08 01:35:52.000000 AiBot.py-1.2.10/AiBot/_AndroidBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.10/AiBot/_WebBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)    36095 2023-08-04 02:53:04.000000 AiBot.py-1.2.10/AiBot/_WinBot.py
--rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.10/AiBot/__init__.py
--rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.10/AiBot/_loguru_format.py
--rw-r--r--   0 chenxun    (501) staff       (20)     2219 2023-08-08 01:19:50.000000 AiBot.py-1.2.10/AiBot/_multiprocess.py
--rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-22 01:46:17.000000 AiBot.py-1.2.10/AiBot/_utils.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-08 01:37:41.908347 AiBot.py-1.2.10/AiBot.py.egg-info/
--rw-r--r--   0 chenxun    (501) staff       (20)      250 2023-08-08 01:37:41.000000 AiBot.py-1.2.10/AiBot.py.egg-info/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)      391 2023-08-08 01:37:41.000000 AiBot.py-1.2.10/AiBot.py.egg-info/SOURCES.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-08-08 01:37:41.000000 AiBot.py-1.2.10/AiBot.py.egg-info/dependency_links.txt
--rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-08-08 01:37:41.000000 AiBot.py-1.2.10/AiBot.py.egg-info/requires.txt
--rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-08-08 01:37:41.000000 AiBot.py-1.2.10/AiBot.py.egg-info/top_level.txt
--rw-r--r--   0 chenxun    (501) staff       (20)    16725 2023-08-07 03:05:43.000000 AiBot.py-1.2.10/LICENSE
--rw-r--r--   0 chenxun    (501) staff       (20)      250 2023-08-08 01:37:41.911232 AiBot.py-1.2.10/PKG-INFO
--rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.10/README.md
--rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.10/pyproject.toml
--rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-08-08 01:37:41.911834 AiBot.py-1.2.10/setup.cfg
--rw-r--r--   0 chenxun    (501) staff       (20)      623 2023-08-08 01:19:50.000000 AiBot.py-1.2.10/setup.py
-drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-08 01:37:41.909930 AiBot.py-1.2.10/test/
--rw-r--r--   0 chenxun    (501) staff       (20)     1688 2023-08-08 01:19:50.000000 AiBot.py-1.2.10/test/test_android.py
--rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.10/test/test_web.py
--rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.10/test/test_win.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-07 10:47:47.690814 AiBot.py-1.2.9/
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-07 10:47:47.686223 AiBot.py-1.2.9/AiBot/
+-rw-r--r--   0 chenxun    (501) staff       (20)    55743 2023-08-07 10:45:34.000000 AiBot.py-1.2.9/AiBot/_AndroidBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    21135 2023-03-13 02:59:10.000000 AiBot.py-1.2.9/AiBot/_WebBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)    36095 2023-08-04 02:53:04.000000 AiBot.py-1.2.9/AiBot/_WinBot.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      162 2022-12-11 09:17:44.000000 AiBot.py-1.2.9/AiBot/__init__.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     5044 2022-08-31 16:13:27.000000 AiBot.py-1.2.9/AiBot/_loguru_format.py
+-rw-r--r--   0 chenxun    (501) staff       (20)     1712 2023-03-22 01:46:17.000000 AiBot.py-1.2.9/AiBot/_utils.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-07 10:47:47.688276 AiBot.py-1.2.9/AiBot.py.egg-info/
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-08-07 10:47:47.000000 AiBot.py-1.2.9/AiBot.py.egg-info/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)      368 2023-08-07 10:47:47.000000 AiBot.py-1.2.9/AiBot.py.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        1 2023-08-07 10:47:47.000000 AiBot.py-1.2.9/AiBot.py.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)       14 2023-08-07 10:47:47.000000 AiBot.py-1.2.9/AiBot.py.egg-info/requires.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)        6 2023-08-07 10:47:47.000000 AiBot.py-1.2.9/AiBot.py.egg-info/top_level.txt
+-rw-r--r--   0 chenxun    (501) staff       (20)    16725 2023-08-07 03:05:43.000000 AiBot.py-1.2.9/LICENSE
+-rw-r--r--   0 chenxun    (501) staff       (20)      249 2023-08-07 10:47:47.690569 AiBot.py-1.2.9/PKG-INFO
+-rw-r--r--   0 chenxun    (501) staff       (20)     5253 2022-12-16 13:41:49.000000 AiBot.py-1.2.9/README.md
+-rw-r--r--   0 chenxun    (501) staff       (20)      104 2022-08-31 16:13:27.000000 AiBot.py-1.2.9/pyproject.toml
+-rw-r--r--   0 chenxun    (501) staff       (20)       38 2023-08-07 10:47:47.690881 AiBot.py-1.2.9/setup.cfg
+-rw-r--r--   0 chenxun    (501) staff       (20)      622 2023-08-07 10:46:50.000000 AiBot.py-1.2.9/setup.py
+drwxr-xr-x   0 chenxun    (501) staff       (20)        0 2023-08-07 10:47:47.689944 AiBot.py-1.2.9/test/
+-rw-r--r--   0 chenxun    (501) staff       (20)     1534 2023-07-28 05:37:55.000000 AiBot.py-1.2.9/test/test_android.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      796 2023-02-16 09:55:43.000000 AiBot.py-1.2.9/test/test_web.py
+-rw-r--r--   0 chenxun    (501) staff       (20)      370 2022-12-11 09:17:44.000000 AiBot.py-1.2.9/test/test_win.py
```

### Comparing `AiBot.py-1.2.10/AiBot/_AndroidBot.py` & `AiBot.py-1.2.9/AiBot/_AndroidBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import abc
 import json
-import multiprocessing
-import os
 import socket
 import socketserver
+import sys
 import threading
 import time
 from ast import literal_eval
 from datetime import datetime
 from typing import Optional, Dict, List, Tuple, Union
 
 from loguru import logger
 
-from ._multiprocess import multiprocess
-
 from ._utils import _protect, _Region, _Algorithm, _SubColors
 
-spawn = multiprocessing.get_context("spawn")
-
 # _LOG_PATH = Path(__file__).parent.resolve() / "logs"
 
 # # rotation 文件分割，可按时间或者大小分割
 # # retention 日志保留时间
 # # compression="zip" 压缩方式
 #
 # # logger.add(LOG_PATH / 'runtime.log', rotation='100 MB', retention='15 days')  按大小分割，日志保留 15 天
@@ -37,16 +32,16 @@
 # logger.add("a.log", filter=lambda record: record["extra"].get("name") == "a")
 # logger.add("b.log", filter=lambda record: record["extra"].get("name") == "b")
 # logger_a = logger.bind(name="a")
 # logger_b = logger.bind(name="b")
 
 Log_Format = "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | " \
              "<level>{level: <8}</level> | " \
-             "{process.id} - {thread.id: <8} | " \
-             "<cyan>{module}:{line}</cyan> | " \
+             "{thread.name: <8} | " \
+             "<cyan>{module}.{function}:{line}</cyan> | " \
              "<level>{message}</level>"  # 日志内容
 
 
 class Point:
     def __init__(self, x: float, y: float, driver: "AndroidBotMain"):
         self.x = x
         self.y = y
@@ -126,25 +121,14 @@
 _Point_Tuple = Union[Point, Tuple[float, float]]
 
 
 class _ThreadingTCPServer(socketserver.ThreadingTCPServer):
     daemon_threads = True
     allow_reuse_address = True
 
-    def server_bind(self) -> None:
-        """Called by constructor to bind the socket.
-        May be overridden.
-        """
-        if os.name != "nt":
-            self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-        else:  # In windows, SO_REUSEPORT is not available
-            self.socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.socket.bind(self.server_address)
-        self.server_address = self.socket.getsockname()
-
 
 class AndroidBotMain(socketserver.BaseRequestHandler, metaclass=_protect("handle", "execute")):
     raise_err = False
 
     wait_timeout = 3  # seconds
     interval_timeout = 0.5  # seconds
 
@@ -155,18 +139,18 @@
     _base_path = "/storage/emulated/0/Android/data/com.aibot.client/files/"
 
     def __init__(self, request, client_address, server):
         self._lock = threading.Lock()
         self.log = logger
 
         if self.log_storage:
-            log_file_name = f"{multiprocessing.current_process().ident}_{threading.current_thread().ident}"
-            log_path = f"./logs/{log_file_name}_runtime.log"
+            thread_name = threading.current_thread().name
+            log_path = f"./logs/{thread_name}_runtime.log"
             logger.add(log_path, level=self.log_level.upper(), format=Log_Format,
-                       filter=lambda record: f"{record['process'].id}_{record['thread'].id}" == log_file_name,
+                       filter=lambda record: record["thread"].name == thread_name,
                        rotation='10 MB',
                        retention='0 days')
 
         super().__init__(request, client_address, server)
 
     def __send_data(self, *args) -> str:
         try:
@@ -187,15 +171,15 @@
                 if response == b"":
                     raise ConnectionAbortedError(f"{self.client_address[0]}:{self.client_address[1]} 客户端断开链接")
                 data_length, data = response.split(b"/", 1)
                 while int(data_length) > len(data):
                     data += self.request.recv(65535)
                 self.log.debug(rf"<--- {data}")
         except Exception as e:
-            self.log.error("send tcp data error: " + str(e))
+            self.log.info("send tcp data error: ", e)
             raise e
 
         return data.decode("utf8").strip()
 
     def __push_file(self, func_name: str, to_path: str, file: bytes):
         func_name = bytes(func_name, "utf8")
         to_path = bytes(to_path, "utf8")
@@ -1585,47 +1569,26 @@
 
     @abc.abstractmethod
     def script_main(self):
         """脚本入口，由子类重写
         """
 
     @classmethod
-    def execute(cls, listen_port: int, multi: int = 1):
+    def execute(cls, listen_port: int):
         """
         多线程启动 Socket 服务，执行脚本
 
         :return:
         """
 
         if listen_port < 0 or listen_port > 65535:
             raise OSError("`listen_port` must be in 0-65535.")
-
-        if multi < 1:
-            raise ValueError("`multi` must be >= 1.")
-
         print("启动服务...")
         print("等待设备连接...")
-
-        if multi == 1:
-            # 获取 IPv4 可用地址
-            address_info = \
-                socket.getaddrinfo(None, listen_port, socket.AF_INET, socket.SOCK_STREAM, 0, socket.AI_PASSIVE)[0]
-            *_, socket_address = address_info
-            # 启动 Socket 服务
-            sock = _ThreadingTCPServer(socket_address, cls, bind_and_activate=True)
-            sock.serve_forever()
-        else:
-            # 多进程启动 Socket 服务
-            count = min(multi, os.cpu_count())
-            multiprocess(count, lambda: spawn.Process(
-                target=_run_server, args=(listen_port, cls)
-            ))
-
-
-def _run_server(listen_port, handler_cls):
-    # 获取 IPv4 可用地址
-    address_info = socket.getaddrinfo(None, listen_port, socket.AF_INET, socket.SOCK_STREAM, 0, socket.AI_PASSIVE)[
-        0]
-    *_, socket_address = address_info
-
-    with _ThreadingTCPServer(socket_address, handler_cls, bind_and_activate=True) as server:
-        server.serve_forever()
+        # 获取 IPv4 可用地址
+        address_info = socket.getaddrinfo(None, listen_port, socket.AF_INET, socket.SOCK_STREAM, 0, socket.AI_PASSIVE)[
+            0]
+        *_, socket_address = address_info
+
+        # 启动 Socket 服务
+        sock = _ThreadingTCPServer(socket_address, cls, bind_and_activate=True)
+        sock.serve_forever()
```

### Comparing `AiBot.py-1.2.10/AiBot/_WebBot.py` & `AiBot.py-1.2.9/AiBot/_WebBot.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/AiBot/_WinBot.py` & `AiBot.py-1.2.9/AiBot/_WinBot.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/AiBot/_loguru_format.py` & `AiBot.py-1.2.9/AiBot/_loguru_format.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/AiBot/_utils.py` & `AiBot.py-1.2.9/AiBot/_utils.py`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/LICENSE` & `AiBot.py-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/README.md` & `AiBot.py-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `AiBot.py-1.2.10/setup.py` & `AiBot.py-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install_requires = [
     "loguru~=0.6.0"
 ]
 
 setup_kwargs = {
     'name': 'AiBot.py',
-    'version': '1.2.10',
+    'version': '1.2.9',
     'description': '...',
     'long_description': '...',
     'long_description_content_type': 'text/markdown',
     'author': 'waitan2018',
     'author_email': None,
     'maintainer': 'waitan2018',
     'maintainer_email': None,
```

### Comparing `AiBot.py-1.2.10/test/test_web.py` & `AiBot.py-1.2.9/test/test_web.py`

 * *Files identical despite different names*


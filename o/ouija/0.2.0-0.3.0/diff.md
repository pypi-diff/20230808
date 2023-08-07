# Comparing `tmp/ouija-0.2.0.tar.gz` & `tmp/ouija-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ouija-0.2.0.tar", last modified: Thu Aug  3 18:02:00 2023, max compression
+gzip compressed data, was "ouija-0.3.0.tar", last modified: Mon Aug  7 23:04:28 2023, max compression
```

## Comparing `ouija-0.2.0.tar` & `ouija-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.804327 ouija-0.2.0/
--rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-0.2.0/LICENSE
--rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-0.2.0/MANIFEST.in
--rw-r--r--   0 embali     (501) staff       (20)     1723 2023-08-03 18:02:00.803565 ouija-0.2.0/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)     1225 2023-08-03 17:58:40.000000 ouija-0.2.0/README.rst
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.798403 ouija-0.2.0/ouija/
--rw-r--r--   0 embali     (501) staff       (20)      376 2023-08-03 17:15:57.000000 ouija-0.2.0/ouija/__init__.py
--rw-r--r--   0 embali     (501) staff       (20)     2955 2023-08-03 17:34:25.000000 ouija-0.2.0/ouija/interface.py
--rw-r--r--   0 embali     (501) staff       (20)     1864 2023-08-03 17:34:34.000000 ouija-0.2.0/ouija/link.py
--rw-r--r--   0 embali     (501) staff       (20)     9311 2023-08-03 17:34:10.000000 ouija-0.2.0/ouija/ouija.py
--rw-r--r--   0 embali     (501) staff       (20)     1815 2023-08-03 17:36:30.000000 ouija-0.2.0/ouija/packet.py
--rw-r--r--   0 embali     (501) staff       (20)      367 2023-08-03 17:18:48.000000 ouija-0.2.0/ouija/primitives.py
--rw-r--r--   0 embali     (501) staff       (20)     2287 2023-08-03 17:36:40.000000 ouija-0.2.0/ouija/proxy.py
--rw-r--r--   0 embali     (501) staff       (20)     2882 2023-08-03 17:36:51.000000 ouija-0.2.0/ouija/relay.py
--rw-r--r--   0 embali     (501) staff       (20)     1475 2023-08-03 14:13:25.000000 ouija-0.2.0/ouija/telemetry.py
--rw-r--r--   0 embali     (501) staff       (20)      910 2023-08-03 17:27:40.000000 ouija-0.2.0/ouija/tuning.py
--rw-r--r--   0 embali     (501) staff       (20)     1127 2023-07-29 23:39:45.000000 ouija-0.2.0/ouija/utils.py
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-03 18:02:00.802664 ouija-0.2.0/ouija.egg-info/
--rw-r--r--   0 embali     (501) staff       (20)     1723 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)      365 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/SOURCES.txt
--rw-r--r--   0 embali     (501) staff       (20)        1 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/dependency_links.txt
--rw-r--r--   0 embali     (501) staff       (20)       36 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/requires.txt
--rw-r--r--   0 embali     (501) staff       (20)        6 2023-08-03 18:02:00.000000 ouija-0.2.0/ouija.egg-info/top_level.txt
--rw-r--r--   0 embali     (501) staff       (20)       38 2023-08-03 18:02:00.804546 ouija-0.2.0/setup.cfg
--rw-r--r--   0 embali     (501) staff       (20)      875 2023-08-03 17:22:34.000000 ouija-0.2.0/setup.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.592454 ouija-0.3.0/
+-rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-0.3.0/LICENSE
+-rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-0.3.0/MANIFEST.in
+-rw-r--r--   0 embali     (501) staff       (20)     2116 2023-08-07 23:04:28.591941 ouija-0.3.0/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)     1618 2023-08-07 22:55:23.000000 ouija-0.3.0/README.rst
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.576422 ouija-0.3.0/ouija/
+-rw-r--r--   0 embali     (501) staff       (20)      380 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/__init__.py
+-rw-r--r--   0 embali     (501) staff       (20)     3007 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/interface.py
+-rw-r--r--   0 embali     (501) staff       (20)     1908 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/link.py
+-rw-r--r--   0 embali     (501) staff       (20)     8869 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/ouija.py
+-rw-r--r--   0 embali     (501) staff       (20)     1648 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/packet.py
+-rw-r--r--   0 embali     (501) staff       (20)     2027 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/proxy.py
+-rw-r--r--   0 embali     (501) staff       (20)     1127 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/rawparser.py
+-rw-r--r--   0 embali     (501) staff       (20)     2583 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/relay.py
+-rw-r--r--   0 embali     (501) staff       (20)     2940 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/telemetry.py
+-rw-r--r--   0 embali     (501) staff       (20)      297 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/tuning.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.581109 ouija-0.3.0/ouija.egg-info/
+-rw-r--r--   0 embali     (501) staff       (20)     2116 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)      521 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/SOURCES.txt
+-rw-r--r--   0 embali     (501) staff       (20)        1 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/dependency_links.txt
+-rw-r--r--   0 embali     (501) staff       (20)       36 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/requires.txt
+-rw-r--r--   0 embali     (501) staff       (20)        6 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/top_level.txt
+-rw-r--r--   0 embali     (501) staff       (20)       38 2023-08-07 23:04:28.592671 ouija-0.3.0/setup.cfg
+-rw-r--r--   0 embali     (501) staff       (20)      875 2023-08-07 22:55:23.000000 ouija-0.3.0/setup.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.590671 ouija-0.3.0/tests/
+-rw-r--r--   0 embali     (501) staff       (20)     2666 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_interface.py
+-rw-r--r--   0 embali     (501) staff       (20)     1569 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_link.py
+-rw-r--r--   0 embali     (501) staff       (20)    15840 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_ouija.py
+-rw-r--r--   0 embali     (501) staff       (20)      749 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_packet.py
+-rw-r--r--   0 embali     (501) staff       (20)      984 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_proxy.py
+-rw-r--r--   0 embali     (501) staff       (20)      767 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_rawparser.py
+-rw-r--r--   0 embali     (501) staff       (20)     2958 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_relay.py
+-rw-r--r--   0 embali     (501) staff       (20)     2856 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_telemetry.py
```

### Comparing `ouija-0.2.0/LICENSE` & `ouija-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ouija-0.2.0/PKG-INFO` & `ouija-0.3.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-Metadata-Version: 2.1
-Name: ouija
-Version: 0.2.0
-Summary: Python library for building and accessing UDP-relayed TCP proxies
-Home-page: https://github.com/neurophant/ouija/
-Author: Anton Smolin
-Author-email: smolin.anton@gmail.com
-License: MIT
-Keywords: async https tcp udp proxy relay
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
 Ouija
 =====
 
 Python library for building and accessing UDP-relayed TCP proxies
 
+|pypi|
+
+.. |pypi| image:: https://badge.fury.io/py/ouija.svg
+    :target: https://badge.fury.io/py/ouija
+    :alt: pypi version
+
 Features
 --------
 
+.. image:: https://raw.githubusercontent.com/neurophant/ouija/master/ouija.png
+    :alt: Sliding from center to edge - searching for maximum entropy difference
+    :width: 883
+    :height: 363
+
 Classes:
 
 * Tuning - Relay-Proxy settings
 * Interface - basic HTTPS proxy server
-* Relay - HTTPS proxy interface, which communicates with Proxy via encrypted UDP
+* Relay - HTTPS proxy relay, which communicates with Proxy via encrypted UDP
 * Link - Relay link within Proxy
 * Proxy - UDP server, which gets requests from Relay and sends back responses from target TCP servers
 
 Tuning:
 
 * fernet - Fernet instance with provided secret key - use Fernet.generate_key()
 * token - your secret token - UUID4 or anything else
@@ -63,8 +59,10 @@
 examples:
     * ouija-relay - simple HTTPS proxy server interface
     * ouija-proxy - UDP-relayed TCP proxy server
 
 Tests
 -----
 
-TBD
+.. code-block:: bash
+
+    pytest --cov-report html:htmlcov --cov=ouija tests/
```

### Comparing `ouija-0.2.0/ouija/interface.py` & `ouija-0.3.0/ouija/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import logging
 import os
 from typing import Dict
 
 from .tuning import Tuning
 from .relay import Relay
 from .telemetry import Telemetry
-from .utils import RawParser
+from .rawparser import RawParser
 
 
 logging.basicConfig(
     format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
     datefmt='%Y-%m-%d:%H:%M:%S',
     level=logging.ERROR,
 )
 logger = logging.getLogger(__name__)
 
 
 class Interface:
     telemetry: Telemetry
-    __tuning: Tuning
-    __proxy_host: str
-    __proxy_port: int
-    __index: int
-    __sessions: Dict[int, asyncio.Task]
+    tuning: Tuning
+    proxy_host: str
+    proxy_port: int
+    index: int
+    sessions: Dict[int, asyncio.Task]
 
     def __init__(self, *, telemetry: Telemetry, tuning: Tuning, proxy_host: str, proxy_port: int) -> None:
         self.telemetry = telemetry
         self.tuning = tuning
         self.proxy_host = proxy_host
         self.proxy_port = proxy_port
         self.index = 0
@@ -49,46 +49,45 @@
             proxy_host=self.proxy_host,
             proxy_port=self.proxy_port,
             remote_host=remote_host,
             remote_port=remote_port,
         )
         await relay.serve()
 
-    async def _session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+    async def handle_session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         data = await reader.readuntil(b'\r\n\r\n')
         request = RawParser(data=data)
-
         if request.error:
             logger.error('Parse error')
         elif request.method == 'CONNECT':
             await self.https_handler(
                 reader=reader,
                 writer=writer,
                 remote_host=request.host,
                 remote_port=request.port,
             )
         else:
             logger.error(f'{request.method} method is not supported')
 
     async def session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         try:
-            await asyncio.wait_for(self._session(reader=reader, writer=writer), self.tuning.serving_timeout)
+            await asyncio.wait_for(self.handle_session(reader=reader, writer=writer), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
             logger.error('Timeout')
 
     async def serve(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
-        self.sessions[self.index] = asyncio.create_task(self._session(reader=reader, writer=writer))
+        self.sessions[self.index] = asyncio.create_task(self.session(reader=reader, writer=writer))
         self.index += 1
 
-    async def cleanup(self) -> None:
+    async def cleanup(self) -> None:    # pragma: no cover
         while True:
             await asyncio.sleep(1)
             for index in sorted(self.sessions.keys()):
                 if self.sessions[index].done():
                     self.sessions.pop(index)
-            self.telemetry.links = len(self.sessions)
+            self.telemetry.link(links=len(self.sessions))
 
-    async def monitor(self) -> None:
+    async def monitor(self) -> None:    # pragma: no cover
         while True:
             await asyncio.sleep(1)
             os.system('clear')
             print(self.telemetry)
```

### Comparing `ouija-0.2.0/ouija/link.py` & `ouija-0.3.0/ouija/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .packet import Packet
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .ouija import Ouija
 
 from typing import TYPE_CHECKING
-if TYPE_CHECKING:
+if TYPE_CHECKING:   # pragma: no cover
     from proxy import Proxy
 
 
 logging.basicConfig(
     format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
     datefmt='%Y-%m-%d:%H:%M:%S',
     level=logging.ERROR,
@@ -55,11 +55,11 @@
         self.opened.set()
         asyncio.create_task(self.serve())
         self.proxy.links[self.addr] = self
         await self.send_ack_open()
         return True
 
     async def on_serve(self) -> bool:
-        return True
+        return True     # pragma: no cover
 
     async def on_close(self) -> None:
         self.proxy.links.pop(self.addr, None)
```

### Comparing `ouija-0.2.0/ouija/ouija.py` & `ouija-0.3.0/ouija/ouija.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import asyncio
 import logging
 import time
 from typing import Optional, Dict
 
 from .telemetry import Telemetry
 from .tuning import Tuning
-from .primitives import Sent, Received
-from .packet import Phase, Packet
+from .packet import Phase, Packet, Sent, Received
 
 
 logging.basicConfig(
     format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
     datefmt='%Y-%m-%d:%H:%M:%S',
     level=logging.ERROR,
 )
@@ -33,27 +32,27 @@
     write_closed: asyncio.Event
 
     async def sendto(self, *, data: bytes) -> None:
         raise NotImplementedError
 
     async def send(self, *, data: bytes) -> None:
         await self.sendto(data=data)
+        self.telemetry.send(data=data)
 
-        self.telemetry.packets_sent += 1
-        self.telemetry.bytes_sent += len(data)
-        if len(data) > self.telemetry.max_packet_size:
-            self.telemetry.max_packet_size = len(data)
+    async def send_packet(self, *, packet: Packet) -> bytes:
+        data = packet.binary(fernet=self.tuning.fernet)
+        await self.send(data=data)
+        return data
 
-    async def send_retry(self, *, data: bytes, event: asyncio.Event) -> bool:
+    async def send_retry(self, *, packet: Packet, event: asyncio.Event) -> bool:
         for _ in range(self.tuning.udp_retries):
-            await self.send(data=data)
+            await self.send_packet(packet=packet)
             try:
                 await asyncio.wait_for(event.wait(), self.tuning.udp_timeout)
             except asyncio.TimeoutError:
-                self.telemetry.resent += 1
                 continue
             else:
                 return True
         else:
             return False
 
     async def read(self) -> bytes:
@@ -65,177 +64,170 @@
             await self.writer.drain()
 
     async def recv(self, *, seq: int, data: bytes, drain: bool) -> None:
         if seq >= self.recv_seq:
             self.recv_buf[seq] = Received(data=data, drain=drain)
 
         for seq in sorted(self.recv_buf.keys()):
-            if seq < self.recv_seq:
-                self.recv_buf.pop(seq)
-            if seq == self.recv_seq:
-                recv = self.recv_buf.pop(seq)
-                await self.write(data=recv.data, drain=recv.drain)
-                self.recv_seq += 1
+            if seq != self.recv_seq:
+                continue
+
+            recv = self.recv_buf.pop(seq)
+            await self.write(data=recv.data, drain=recv.drain)
+            self.recv_seq += 1
 
         await self.send_ack_data(seq=seq)
 
         if len(self.recv_buf) >= self.tuning.udp_capacity:
             await self.close()
-            self.telemetry.recv_buf_overloads += 1
+            self.telemetry.recv_buf_overload()
 
     async def enqueue_send(self, *, data: bytes, drain: bool) -> None:
         data_packet = Packet(
             phase=Phase.DATA,
             ack=False,
             seq=self.sent_seq,
             data=data,
             drain=drain,
         )
-        data_ = await data_packet.binary(fernet=self.tuning.fernet)
-        self.sent_buf[self.sent_seq] = Sent(data=data_)
-        await self.send(data=data_)
+        self.sent_buf[self.sent_seq] = Sent(data=await self.send_packet(packet=data_packet))
         self.sent_seq += 1
 
         if len(self.sent_buf) >= self.tuning.udp_capacity:
             await self.close()
-            self.telemetry.sent_buf_overloads += 1
+            self.telemetry.send_buf_overload()
 
     async def dequeue_send(self, *, seq: int) -> None:
         self.sent_buf.pop(seq, None)
 
     async def send_open(self) -> bool:
         open_packet = Packet(
             phase=Phase.OPEN,
             ack=False,
             token=self.tuning.token,
             host=self.remote_host,
             port=self.remote_port,
         )
-        if not await self.send_retry(
-                data=await open_packet.binary(fernet=self.tuning.fernet),
-                event=self.opened,
-        ):
+        if not await self.send_retry(packet=open_packet, event=self.opened):
             return False
 
         return True
 
     async def send_ack_open(self) -> None:
         open_ack_packet = Packet(
             phase=Phase.OPEN,
             ack=True,
             token=self.tuning.token,
         )
-        await self.send(data=await open_ack_packet.binary(fernet=self.tuning.fernet))
+        await self.send_packet(packet=open_ack_packet)
 
     async def check_token(self, *, token: str) -> bool:
         if token == self.tuning.token:
             return True
 
         await self.close()
-        self.telemetry.token_errors += 1
+        self.telemetry.token_error()
         return False
 
     async def send_ack_data(self, *, seq: int) -> None:
         data_ack_packet = Packet(
             phase=Phase.DATA,
             ack=True,
             seq=seq,
         )
-        await self.send(data=await data_ack_packet.binary(fernet=self.tuning.fernet))
+        await self.send_packet(packet=data_ack_packet)
 
     async def send_close(self) -> None:
         close_packet = Packet(
             phase=Phase.CLOSE,
             ack=False,
         )
-        await self.send_retry(
-            data=await close_packet.binary(fernet=self.tuning.fernet),
-            event=self.read_closed,
-        )
+        await self.send_retry(packet=close_packet, event=self.read_closed)
 
     async def send_ack_close(self) -> None:
         close_ack_packet = Packet(
             phase=Phase.CLOSE,
             ack=True,
         )
-        await self.send(data=await close_ack_packet.binary(fernet=self.tuning.fernet))
+        await self.send_packet(packet=close_ack_packet)
 
     async def on_open(self, packet: Packet) -> bool:
         raise NotImplementedError
 
-    async def process_packet(self, *, packet: Packet) -> None:
+    async def process_packet(self, *, data: bytes) -> None:
+        self.telemetry.recv(data=data)
+        packet = Packet.packet(data=data, fernet=self.tuning.fernet)
+
         match packet.phase:
             case Phase.OPEN:
                 if not await self.check_token(token=packet.token):
                     return
 
                 if not await self.on_open(packet=packet):
                     return
 
-                self.telemetry.opened += 1
+                self.telemetry.open()
             case Phase.DATA:
                 if not self.opened.is_set() or self.write_closed.is_set():
                     return
 
                 if packet.ack:
                     await self.dequeue_send(seq=packet.seq)
                 else:
                     await self.recv(seq=packet.seq, data=packet.data, drain=packet.drain)
             case Phase.CLOSE:
                 if packet.ack:
                     self.read_closed.set()
                 else:
                     await self.send_ack_close()
                     self.write_closed.set()
-            case _:
-                self.telemetry.type_errors += 1
+            case _:     # pragma: no cover
+                self.telemetry.type_error()
 
-    async def process(self, *, packet: Packet) -> None:
+    async def process(self, *, data: bytes) -> None:
         try:
-            await self.process_packet(packet=packet)
+            await self.process_packet(data=data)
         except ConnectionError as e:
             logger.error(e)
-            self.telemetry.connection_errors += 1
+            self.telemetry.connection_error()
         except Exception as e:
             await self.close()
             logger.error(e)
-            self.telemetry.processing_errors += 1
+            self.telemetry.processing_error()
 
     async def resend_packets(self) -> None:
         while self.opened.is_set() or self.sent_buf:
             await asyncio.sleep(self.tuning.udp_timeout)
 
             for seq in sorted(self.sent_buf.keys()):
                 delta = int(time.time()) - self.sent_buf[seq].timestamp
 
                 if delta >= self.tuning.serving_timeout or self.sent_buf[seq].retries >= self.tuning.udp_retries:
                     await self.close()
-                    self.telemetry.unfinished += 1
-                    break
+                    return
 
                 if delta >= self.tuning.udp_timeout:
                     await self.send(data=self.sent_buf[seq].data)
                     self.sent_buf[seq].retries += 1
-                    self.telemetry.resent += 1
 
         await self.send_close()
 
         try:
             await asyncio.wait_for(self.write_closed.wait(), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
             pass
 
     async def resend(self) -> None:
         try:
             await asyncio.wait_for(self.resend_packets(), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
-            self.telemetry.timeout_errors += 1
+            self.telemetry.timeout_error()
         except Exception as e:
             logger.error(e)
-            self.telemetry.resending_errors += 1
+            self.telemetry.resending_error()
         finally:
             await self.close()
 
     async def on_serve(self) -> bool:
         raise NotImplementedError
 
     async def serve_stream(self) -> None:
@@ -259,28 +251,28 @@
                     drain=True if len(data) - idx <= self.tuning.udp_payload else False,
                 )
 
     async def serve(self) -> None:
         try:
             await asyncio.wait_for(self.serve_stream(), self.tuning.serving_timeout)
         except asyncio.TimeoutError:
-            self.telemetry.timeout_errors += 1
+            self.telemetry.timeout_error()
         except ConnectionError as e:
             logger.error(e)
-            self.telemetry.connection_errors += 1
+            self.telemetry.connection_error()
         except Exception as e:
             logger.error(e)
-            self.telemetry.serving_errors += 1
+            self.telemetry.serving_error()
 
     async def on_close(self) -> None:
         raise NotImplementedError
 
     async def close(self) -> None:
         if self.opened.is_set():
-            self.telemetry.closed += 1
+            self.telemetry.close()
 
         self.opened.clear()
         self.read_closed.set()
         self.write_closed.set()
 
         if isinstance(self.writer, asyncio.StreamWriter) and not self.writer.is_closing():
             self.writer.close()
```

### Comparing `ouija-0.2.0/ouija/proxy.py` & `ouija-0.3.0/ouija/proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import os
 from typing import Dict, Tuple
 import logging
 
-from .packet import Packet
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .link import Link
 
 
 logging.basicConfig(
     format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
@@ -31,44 +30,35 @@
         self.tuning = tuning
         self.proxy_host = proxy_host
         self.proxy_port = proxy_port
 
     def connection_made(self, transport) -> None:
         self.transport = transport
 
-    async def _datagram_received_async(self, *, data, addr) -> None:
-        self.telemetry.packets_received += 1
-        self.telemetry.bytes_received += len(data)
-        try:
-            packet = await Packet.packet(data=data, fernet=self.tuning.fernet)
-        except Exception as e:
-            logger.error(e)
-            self.telemetry.decoding_errors += 1
-            return
-
+    async def datagram_received_async(self, *, data, addr) -> None:
         link = self.links.get(addr, Link(telemetry=self.telemetry, proxy=self, addr=addr, tuning=self.tuning))
-        await link.process(packet=packet)
+        await link.process(data=data)
 
     def datagram_received(self, data, addr) -> None:
-        asyncio.create_task(self._datagram_received_async(data=data, addr=addr))
+        asyncio.create_task(self.datagram_received_async(data=data, addr=addr))
 
-    def error_received(self, exc) -> None:
+    def error_received(self, exc) -> None:  # pragma: no cover
         logger.error(exc)
 
     def connection_lost(self, exc) -> None:
         self.transport.close()
         logger.error(exc)
 
-    async def serve(self) -> None:
+    async def serve(self) -> None:  # pragma: no cover
         loop = asyncio.get_event_loop()
         await loop.create_datagram_endpoint(lambda: self, local_addr=(self.proxy_host, self.proxy_port))
 
-    async def cleanup(self) -> None:
+    async def cleanup(self) -> None:    # pragma: no cover
         while True:
             await asyncio.sleep(1)
-            self.telemetry.links = len(self.links)
+            self.telemetry.link(links=len(self.links))
 
-    async def monitor(self) -> None:
+    async def monitor(self) -> None:    # pragma: no cover
         while True:
             await asyncio.sleep(1)
             os.system('clear')
             print(self.telemetry)
```

### Comparing `ouija-0.2.0/ouija/relay.py` & `ouija-0.3.0/ouija/relay.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,30 +47,22 @@
         self.recv_buf = dict()
         self.recv_seq = 0
         self.write_closed = asyncio.Event()
 
     def connection_made(self, transport) -> None:
         self.transport = transport
 
-    async def _datagram_received_async(self, *, data, addr) -> None:
-        self.telemetry.packets_received += 1
-        self.telemetry.bytes_received += len(data)
-        try:
-            packet = await Packet.packet(data=data, fernet=self.tuning.fernet)
-        except Exception as e:
-            logger.error(e)
-            self.telemetry.decoding_errors += 1
-            return
-        await self.process(packet=packet)
+    async def datagram_received_async(self, *, data, addr) -> None:
+        await self.process(data=data)
 
     def datagram_received(self, data, addr) -> None:
-        asyncio.create_task(self._datagram_received_async(data=data, addr=addr))
+        asyncio.create_task(self.datagram_received_async(data=data, addr=addr))
 
     def error_received(self, exc) -> None:
-        logger.error(exc)
+        logger.error(exc)   # pragma: no cover
 
     def connection_lost(self, exc) -> None:
         asyncio.create_task(self.close())
 
     async def sendto(self, *, data: bytes) -> None:
         self.transport.sendto(data)
```

### Comparing `ouija-0.2.0/ouija/utils.py` & `ouija-0.3.0/ouija/rawparser.py`

 * *Files identical despite different names*

### Comparing `ouija-0.2.0/ouija.egg-info/PKG-INFO` & `ouija-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ouija
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for building and accessing UDP-relayed TCP proxies
 Home-page: https://github.com/neurophant/ouija/
 Author: Anton Smolin
 Author-email: smolin.anton@gmail.com
 License: MIT
 Keywords: async https tcp udp proxy relay
 Classifier: Development Status :: 3 - Alpha
@@ -14,22 +14,33 @@
 License-File: LICENSE
 
 Ouija
 =====
 
 Python library for building and accessing UDP-relayed TCP proxies
 
+|pypi|
+
+.. |pypi| image:: https://badge.fury.io/py/ouija.svg
+    :target: https://badge.fury.io/py/ouija
+    :alt: pypi version
+
 Features
 --------
 
+.. image:: https://raw.githubusercontent.com/neurophant/ouija/master/ouija.png
+    :alt: Sliding from center to edge - searching for maximum entropy difference
+    :width: 883
+    :height: 363
+
 Classes:
 
 * Tuning - Relay-Proxy settings
 * Interface - basic HTTPS proxy server
-* Relay - HTTPS proxy interface, which communicates with Proxy via encrypted UDP
+* Relay - HTTPS proxy relay, which communicates with Proxy via encrypted UDP
 * Link - Relay link within Proxy
 * Proxy - UDP server, which gets requests from Relay and sends back responses from target TCP servers
 
 Tuning:
 
 * fernet - Fernet instance with provided secret key - use Fernet.generate_key()
 * token - your secret token - UUID4 or anything else
@@ -63,8 +74,10 @@
 examples:
     * ouija-relay - simple HTTPS proxy server interface
     * ouija-proxy - UDP-relayed TCP proxy server
 
 Tests
 -----
 
-TBD
+.. code-block:: bash
+
+    pytest --cov-report html:htmlcov --cov=ouija tests/
```

### Comparing `ouija-0.2.0/setup.py` & `ouija-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ouija',
-    version='0.2.0',
+    version='0.3.0',
     description='Python library for building and accessing UDP-relayed TCP proxies',
     long_description=long_description,
     url='https://github.com/neurophant/ouija/',
     author='Anton Smolin',
     author_email='smolin.anton@gmail.com',
     license='MIT',
     classifiers=[
```


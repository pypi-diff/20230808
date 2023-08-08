# Comparing `tmp/ouija-0.3.0.tar.gz` & `tmp/ouija-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ouija-0.3.0.tar", last modified: Mon Aug  7 23:04:28 2023, max compression
+gzip compressed data, was "ouija-1.0.0.tar", last modified: Tue Aug  8 16:15:49 2023, max compression
```

## Comparing `ouija-0.3.0.tar` & `ouija-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.592454 ouija-0.3.0/
--rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-0.3.0/LICENSE
--rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-0.3.0/MANIFEST.in
--rw-r--r--   0 embali     (501) staff       (20)     2116 2023-08-07 23:04:28.591941 ouija-0.3.0/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)     1618 2023-08-07 22:55:23.000000 ouija-0.3.0/README.rst
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.576422 ouija-0.3.0/ouija/
--rw-r--r--   0 embali     (501) staff       (20)      380 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/__init__.py
--rw-r--r--   0 embali     (501) staff       (20)     3007 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/interface.py
--rw-r--r--   0 embali     (501) staff       (20)     1908 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/link.py
--rw-r--r--   0 embali     (501) staff       (20)     8869 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/ouija.py
--rw-r--r--   0 embali     (501) staff       (20)     1648 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/packet.py
--rw-r--r--   0 embali     (501) staff       (20)     2027 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/proxy.py
--rw-r--r--   0 embali     (501) staff       (20)     1127 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/rawparser.py
--rw-r--r--   0 embali     (501) staff       (20)     2583 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/relay.py
--rw-r--r--   0 embali     (501) staff       (20)     2940 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/telemetry.py
--rw-r--r--   0 embali     (501) staff       (20)      297 2023-08-07 22:55:23.000000 ouija-0.3.0/ouija/tuning.py
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.581109 ouija-0.3.0/ouija.egg-info/
--rw-r--r--   0 embali     (501) staff       (20)     2116 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/PKG-INFO
--rw-r--r--   0 embali     (501) staff       (20)      521 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/SOURCES.txt
--rw-r--r--   0 embali     (501) staff       (20)        1 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/dependency_links.txt
--rw-r--r--   0 embali     (501) staff       (20)       36 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/requires.txt
--rw-r--r--   0 embali     (501) staff       (20)        6 2023-08-07 23:04:28.000000 ouija-0.3.0/ouija.egg-info/top_level.txt
--rw-r--r--   0 embali     (501) staff       (20)       38 2023-08-07 23:04:28.592671 ouija-0.3.0/setup.cfg
--rw-r--r--   0 embali     (501) staff       (20)      875 2023-08-07 22:55:23.000000 ouija-0.3.0/setup.py
-drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-07 23:04:28.590671 ouija-0.3.0/tests/
--rw-r--r--   0 embali     (501) staff       (20)     2666 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_interface.py
--rw-r--r--   0 embali     (501) staff       (20)     1569 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_link.py
--rw-r--r--   0 embali     (501) staff       (20)    15840 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_ouija.py
--rw-r--r--   0 embali     (501) staff       (20)      749 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_packet.py
--rw-r--r--   0 embali     (501) staff       (20)      984 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_proxy.py
--rw-r--r--   0 embali     (501) staff       (20)      767 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_rawparser.py
--rw-r--r--   0 embali     (501) staff       (20)     2958 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_relay.py
--rw-r--r--   0 embali     (501) staff       (20)     2856 2023-08-07 22:55:23.000000 ouija-0.3.0/tests/test_telemetry.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-08 16:15:49.611278 ouija-1.0.0/
+-rw-r--r--   0 embali     (501) staff       (20)     1069 2023-07-30 00:34:05.000000 ouija-1.0.0/LICENSE
+-rw-r--r--   0 embali     (501) staff       (20)       35 2023-07-30 00:34:28.000000 ouija-1.0.0/MANIFEST.in
+-rw-r--r--   0 embali     (501) staff       (20)     4435 2023-08-08 16:15:49.610576 ouija-1.0.0/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)     3632 2023-08-08 16:13:05.000000 ouija-1.0.0/README.rst
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-08 16:15:49.594429 ouija-1.0.0/ouija/
+-rw-r--r--   0 embali     (501) staff       (20)      380 2023-08-07 22:55:23.000000 ouija-1.0.0/ouija/__init__.py
+-rw-r--r--   0 embali     (501) staff       (20)     2899 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/interface.py
+-rw-r--r--   0 embali     (501) staff       (20)     1755 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/link.py
+-rw-r--r--   0 embali     (501) staff       (20)       94 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/log.py
+-rw-r--r--   0 embali     (501) staff       (20)     9193 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/ouija.py
+-rw-r--r--   0 embali     (501) staff       (20)     1648 2023-08-07 22:55:23.000000 ouija-1.0.0/ouija/packet.py
+-rw-r--r--   0 embali     (501) staff       (20)     1846 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/proxy.py
+-rw-r--r--   0 embali     (501) staff       (20)     1127 2023-08-07 22:55:23.000000 ouija-1.0.0/ouija/rawparser.py
+-rw-r--r--   0 embali     (501) staff       (20)     2381 2023-08-08 16:13:05.000000 ouija-1.0.0/ouija/relay.py
+-rw-r--r--   0 embali     (501) staff       (20)     2940 2023-08-07 22:55:23.000000 ouija-1.0.0/ouija/telemetry.py
+-rw-r--r--   0 embali     (501) staff       (20)      297 2023-08-07 22:55:23.000000 ouija-1.0.0/ouija/tuning.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-08 16:15:49.600016 ouija-1.0.0/ouija.egg-info/
+-rw-r--r--   0 embali     (501) staff       (20)     4435 2023-08-08 16:15:49.000000 ouija-1.0.0/ouija.egg-info/PKG-INFO
+-rw-r--r--   0 embali     (501) staff       (20)      534 2023-08-08 16:15:49.000000 ouija-1.0.0/ouija.egg-info/SOURCES.txt
+-rw-r--r--   0 embali     (501) staff       (20)        1 2023-08-08 16:15:49.000000 ouija-1.0.0/ouija.egg-info/dependency_links.txt
+-rw-r--r--   0 embali     (501) staff       (20)       36 2023-08-08 16:15:49.000000 ouija-1.0.0/ouija.egg-info/requires.txt
+-rw-r--r--   0 embali     (501) staff       (20)        6 2023-08-08 16:15:49.000000 ouija-1.0.0/ouija.egg-info/top_level.txt
+-rw-r--r--   0 embali     (501) staff       (20)       38 2023-08-08 16:15:49.611440 ouija-1.0.0/setup.cfg
+-rw-r--r--   0 embali     (501) staff       (20)     1175 2023-08-08 16:13:05.000000 ouija-1.0.0/setup.py
+drwxr-xr-x   0 embali     (501) staff       (20)        0 2023-08-08 16:15:49.609534 ouija-1.0.0/tests/
+-rw-r--r--   0 embali     (501) staff       (20)     3059 2023-08-08 16:13:05.000000 ouija-1.0.0/tests/test_interface.py
+-rw-r--r--   0 embali     (501) staff       (20)     1929 2023-08-08 16:13:05.000000 ouija-1.0.0/tests/test_link.py
+-rw-r--r--   0 embali     (501) staff       (20)    16103 2023-08-08 16:13:05.000000 ouija-1.0.0/tests/test_ouija.py
+-rw-r--r--   0 embali     (501) staff       (20)      749 2023-08-07 22:55:23.000000 ouija-1.0.0/tests/test_packet.py
+-rw-r--r--   0 embali     (501) staff       (20)     1338 2023-08-08 16:13:05.000000 ouija-1.0.0/tests/test_proxy.py
+-rw-r--r--   0 embali     (501) staff       (20)      767 2023-08-07 22:55:23.000000 ouija-1.0.0/tests/test_rawparser.py
+-rw-r--r--   0 embali     (501) staff       (20)     2960 2023-08-08 16:13:05.000000 ouija-1.0.0/tests/test_relay.py
+-rw-r--r--   0 embali     (501) staff       (20)     2856 2023-08-07 22:55:23.000000 ouija-1.0.0/tests/test_telemetry.py
```

### Comparing `ouija-0.3.0/LICENSE` & `ouija-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/ouija/interface.py` & `ouija-1.0.0/ouija/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 import asyncio
-import logging
 import os
 from typing import Dict
 
 from .tuning import Tuning
 from .relay import Relay
 from .telemetry import Telemetry
 from .rawparser import RawParser
-
-
-logging.basicConfig(
-    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
-    datefmt='%Y-%m-%d:%H:%M:%S',
-    level=logging.ERROR,
-)
-logger = logging.getLogger(__name__)
+from .log import logger
 
 
 class Interface:
     telemetry: Telemetry
     tuning: Tuning
     proxy_host: str
     proxy_port: int
@@ -49,45 +41,51 @@
             proxy_host=self.proxy_host,
             proxy_port=self.proxy_port,
             remote_host=remote_host,
             remote_port=remote_port,
         )
         await relay.serve()
 
-    async def handle_session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+    async def session_wrapped(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         data = await reader.readuntil(b'\r\n\r\n')
         request = RawParser(data=data)
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
 
-    async def session(self, *, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
+    async def session(self, *, index: int, reader: asyncio.StreamReader, writer: asyncio.StreamWriter):
         try:
-            await asyncio.wait_for(self.handle_session(reader=reader, writer=writer), self.tuning.serving_timeout)
-        except asyncio.TimeoutError:
-            logger.error('Timeout')
+            await asyncio.wait_for(self.session_wrapped(reader=reader, writer=writer), self.tuning.serving_timeout)
+        except TimeoutError:
+            self.telemetry.timeout_error()
+        except Exception as e:
+            logger.exception(e)
+            self.telemetry.serving_error()
+        finally:
+            _ = self.sessions.pop(index, None)
 
     async def serve(self, reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
-        self.sessions[self.index] = asyncio.create_task(self.session(reader=reader, writer=writer))
+        """Relay TCP server entry point
+
+        :returns: None
+        """
+        self.sessions[self.index] = asyncio.create_task(self.session(index=self.index, reader=reader, writer=writer))
         self.index += 1
 
-    async def cleanup(self) -> None:    # pragma: no cover
-        while True:
-            await asyncio.sleep(1)
-            for index in sorted(self.sessions.keys()):
-                if self.sessions[index].done():
-                    self.sessions.pop(index)
-            self.telemetry.link(links=len(self.sessions))
+    async def debug(self) -> None:    # pragma: no cover
+        """Debug monitor with telemetry output
 
-    async def monitor(self) -> None:    # pragma: no cover
+        :returns: None
+        """
         while True:
             await asyncio.sleep(1)
+            self.telemetry.link(links=len(self.sessions))
             os.system('clear')
             print(self.telemetry)
```

### Comparing `ouija-0.3.0/ouija/link.py` & `ouija-1.0.0/ouija/link.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 import asyncio
 from typing import Tuple
-import logging
 
 from .packet import Packet
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .ouija import Ouija
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:   # pragma: no cover
     from proxy import Proxy
 
 
-logging.basicConfig(
-    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
-    datefmt='%Y-%m-%d:%H:%M:%S',
-    level=logging.ERROR,
-)
-logger = logging.getLogger(__name__)
-
-
 class Link(Ouija):
     proxy: 'Proxy'
     addr: Tuple[str, int]
 
     def __init__(self,  *, telemetry: Telemetry,  proxy: 'Proxy', addr: Tuple[str, int], tuning: Tuning) -> None:
         self.telemetry = telemetry
         self.proxy = proxy
@@ -37,18 +28,21 @@
         self.sent_buf = dict()
         self.sent_seq = 0
         self.read_closed = asyncio.Event()
         self.recv_buf = dict()
         self.recv_seq = 0
         self.write_closed = asyncio.Event()
 
-    async def sendto(self, *, data: bytes) -> None:
+    async def on_send(self, *, data: bytes) -> None:
         self.proxy.transport.sendto(data, self.addr)
 
     async def on_open(self, *, packet: Packet) -> bool:
+        if not packet.host or not packet.port:
+            return False
+
         if self.opened.is_set():
             await self.send_ack_open()
             return False
 
         self.remote_host = packet.host
         self.remote_port = packet.port
         self.reader, self.writer = await asyncio.open_connection(self.remote_host, self.remote_port)
```

### Comparing `ouija-0.3.0/ouija/ouija.py` & `ouija-1.0.0/ouija/ouija.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import asyncio
-import logging
 import time
 from typing import Optional, Dict
 
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .packet import Phase, Packet, Sent, Received
-
-
-logging.basicConfig(
-    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
-    datefmt='%Y-%m-%d:%H:%M:%S',
-    level=logging.ERROR,
-)
-logger = logging.getLogger(__name__)
+from .log import logger
 
 
 class Ouija:
     telemetry: Telemetry
     tuning: Tuning
     reader: Optional[asyncio.StreamReader]
     writer: Optional[asyncio.StreamWriter]
@@ -27,59 +19,63 @@
     sent_buf: Dict[int, Sent]
     sent_seq: int
     read_closed: asyncio.Event
     recv_buf: Dict[int, Received]
     recv_seq: int
     write_closed: asyncio.Event
 
-    async def sendto(self, *, data: bytes) -> None:
+    async def on_send(self, *, data: bytes) -> None:
+        """Hook - send binary data via UDP
+
+        :param data: binary data
+        :returns: None"""
         raise NotImplementedError
 
     async def send(self, *, data: bytes) -> None:
-        await self.sendto(data=data)
+        await self.on_send(data=data)
         self.telemetry.send(data=data)
 
     async def send_packet(self, *, packet: Packet) -> bytes:
         data = packet.binary(fernet=self.tuning.fernet)
         await self.send(data=data)
         return data
 
     async def send_retry(self, *, packet: Packet, event: asyncio.Event) -> bool:
         for _ in range(self.tuning.udp_retries):
             await self.send_packet(packet=packet)
             try:
                 await asyncio.wait_for(event.wait(), self.tuning.udp_timeout)
-            except asyncio.TimeoutError:
+            except TimeoutError:
                 continue
             else:
                 return True
         else:
             return False
 
     async def read(self) -> bytes:
         return await self.reader.read(self.tuning.tcp_buffer)
 
     async def write(self, *, data: bytes, drain: bool) -> None:
         self.writer.write(data)
         if drain:
             await self.writer.drain()
 
-    async def recv(self, *, seq: int, data: bytes, drain: bool) -> None:
-        if seq >= self.recv_seq:
-            self.recv_buf[seq] = Received(data=data, drain=drain)
+    async def recv(self, *, packet: Packet) -> None:
+        if packet.seq >= self.recv_seq:
+            self.recv_buf[packet.seq] = Received(data=packet.data, drain=packet.drain)
 
         for seq in sorted(self.recv_buf.keys()):
             if seq != self.recv_seq:
                 continue
 
             recv = self.recv_buf.pop(seq)
             await self.write(data=recv.data, drain=recv.drain)
             self.recv_seq += 1
 
-        await self.send_ack_data(seq=seq)
+        await self.send_ack_data(seq=packet.seq)
 
         if len(self.recv_buf) >= self.tuning.udp_capacity:
             await self.close()
             self.telemetry.recv_buf_overload()
 
     async def enqueue_send(self, *, data: bytes, drain: bool) -> None:
         data_packet = Packet(
@@ -147,17 +143,21 @@
         close_ack_packet = Packet(
             phase=Phase.CLOSE,
             ack=True,
         )
         await self.send_packet(packet=close_ack_packet)
 
     async def on_open(self, packet: Packet) -> bool:
+        """Hook - process phase open packet
+
+        :param packet: Packet
+        :returns: True on opened link, False on fail"""
         raise NotImplementedError
 
-    async def process_packet(self, *, data: bytes) -> None:
+    async def process_wrapped(self, *, data: bytes) -> None:
         self.telemetry.recv(data=data)
         packet = Packet.packet(data=data, fernet=self.tuning.fernet)
 
         match packet.phase:
             case Phase.OPEN:
                 if not await self.check_token(token=packet.token):
                     return
@@ -169,36 +169,40 @@
             case Phase.DATA:
                 if not self.opened.is_set() or self.write_closed.is_set():
                     return
 
                 if packet.ack:
                     await self.dequeue_send(seq=packet.seq)
                 else:
-                    await self.recv(seq=packet.seq, data=packet.data, drain=packet.drain)
+                    await self.recv(packet=packet)
             case Phase.CLOSE:
                 if packet.ack:
                     self.read_closed.set()
                 else:
                     await self.send_ack_close()
                     self.write_closed.set()
             case _:     # pragma: no cover
                 self.telemetry.type_error()
 
     async def process(self, *, data: bytes) -> None:
+        """Decode and process packet
+
+        :param data: binary packet
+        :returns: None"""
         try:
-            await self.process_packet(data=data)
+            await self.process_wrapped(data=data)
         except ConnectionError as e:
             logger.error(e)
             self.telemetry.connection_error()
         except Exception as e:
             await self.close()
-            logger.error(e)
+            logger.exception(e)
             self.telemetry.processing_error()
 
-    async def resend_packets(self) -> None:
+    async def resend_wrapped(self) -> None:
         while self.opened.is_set() or self.sent_buf:
             await asyncio.sleep(self.tuning.udp_timeout)
 
             for seq in sorted(self.sent_buf.keys()):
                 delta = int(time.time()) - self.sent_buf[seq].timestamp
 
                 if delta >= self.tuning.serving_timeout or self.sent_buf[seq].retries >= self.tuning.udp_retries:
@@ -209,32 +213,35 @@
                     await self.send(data=self.sent_buf[seq].data)
                     self.sent_buf[seq].retries += 1
 
         await self.send_close()
 
         try:
             await asyncio.wait_for(self.write_closed.wait(), self.tuning.serving_timeout)
-        except asyncio.TimeoutError:
+        except TimeoutError:
             pass
 
     async def resend(self) -> None:
         try:
-            await asyncio.wait_for(self.resend_packets(), self.tuning.serving_timeout)
-        except asyncio.TimeoutError:
+            await asyncio.wait_for(self.resend_wrapped(), self.tuning.serving_timeout)
+        except TimeoutError:
             self.telemetry.timeout_error()
         except Exception as e:
-            logger.error(e)
+            logger.exception(e)
             self.telemetry.resending_error()
         finally:
             await self.close()
 
     async def on_serve(self) -> bool:
+        """Hook - executed before serving
+
+        :returns: True - start serving, False - return"""
         raise NotImplementedError
 
-    async def serve_stream(self) -> None:
+    async def serve_wrapped(self) -> None:
         if not await self.on_serve():
             return
 
         asyncio.create_task(self.resend())
 
         while self.opened.is_set():
             try:
@@ -248,26 +255,32 @@
             for idx in range(0, len(data), self.tuning.udp_payload):
                 await self.enqueue_send(
                     data=data[idx:idx + self.tuning.udp_payload],
                     drain=True if len(data) - idx <= self.tuning.udp_payload else False,
                 )
 
     async def serve(self) -> None:
+        """Serve TCP stream with timeout
+
+        :returns: None"""
         try:
-            await asyncio.wait_for(self.serve_stream(), self.tuning.serving_timeout)
-        except asyncio.TimeoutError:
+            await asyncio.wait_for(self.serve_wrapped(), self.tuning.serving_timeout)
+        except TimeoutError:
             self.telemetry.timeout_error()
         except ConnectionError as e:
             logger.error(e)
             self.telemetry.connection_error()
         except Exception as e:
-            logger.error(e)
+            logger.exception(e)
             self.telemetry.serving_error()
 
     async def on_close(self) -> None:
+        """Hook - executed on close
+
+        :returns: None"""
         raise NotImplementedError
 
     async def close(self) -> None:
         if self.opened.is_set():
             self.telemetry.close()
 
         self.opened.clear()
```

### Comparing `ouija-0.3.0/ouija/packet.py` & `ouija-1.0.0/ouija/packet.py`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/ouija/rawparser.py` & `ouija-1.0.0/ouija/rawparser.py`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/ouija/relay.py` & `ouija-1.0.0/ouija/relay.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import asyncio
-import logging
 
 from .telemetry import Telemetry
 from .tuning import Tuning
 from .ouija import Ouija
 from .packet import Packet
-
-
-logging.basicConfig(
-    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
-    datefmt='%Y-%m-%d:%H:%M:%S',
-    level=logging.ERROR,
-)
-logger = logging.getLogger(__name__)
+from .log import logger
 
 
 class Relay(Ouija, asyncio.DatagramProtocol):
     transport: asyncio.DatagramTransport
     proxy_host: str
     proxy_port: int
 
@@ -59,15 +51,15 @@
 
     def error_received(self, exc) -> None:
         logger.error(exc)   # pragma: no cover
 
     def connection_lost(self, exc) -> None:
         asyncio.create_task(self.close())
 
-    async def sendto(self, *, data: bytes) -> None:
+    async def on_send(self, *, data: bytes) -> None:
         self.transport.sendto(data)
 
     async def on_open(self, *, packet: Packet) -> bool:
         if not packet.ack or self.opened.is_set():
             return False
 
         await self.write(data=b'HTTP/1.1 200 Connection Established\r\n\r\n', drain=True)
```

### Comparing `ouija-0.3.0/ouija/telemetry.py` & `ouija-1.0.0/ouija/telemetry.py`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/ouija.egg-info/SOURCES.txt` & `ouija-1.0.0/ouija.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 ouija/__init__.py
 ouija/interface.py
 ouija/link.py
+ouija/log.py
 ouija/ouija.py
 ouija/packet.py
 ouija/proxy.py
 ouija/rawparser.py
 ouija/relay.py
 ouija/telemetry.py
 ouija/tuning.py
```

### Comparing `ouija-0.3.0/setup.py` & `ouija-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,24 +6,29 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ouija',
-    version='0.3.0',
+    version='1.0.0',
     description='Python library for building and accessing UDP-relayed TCP proxies',
     long_description=long_description,
     url='https://github.com/neurophant/ouija/',
     author='Anton Smolin',
     author_email='smolin.anton@gmail.com',
     license='MIT',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
+        'Framework :: AsyncIO',
         'Intended Audience :: Developers',
+        'Intended Audience :: Information Technology',
+        'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11',
+        'Topic :: Internet :: Proxy Servers',
+        'Topic :: Software Development :: Libraries',
     ],
-    keywords='async https tcp udp proxy relay',
+    keywords='asyncio https tcp udp proxy tunnel relay network encrypted security censorship',
     packages=['ouija'],
     install_requires=['cryptography>=41.0.2', 'pbjson>=1.18.0'],
 )
```

### Comparing `ouija-0.3.0/tests/test_interface.py` & `ouija-1.0.0/tests/test_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,56 +17,65 @@
         remote_host='example.com',
         remote_port=443,
     )
     relay_test.serve.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_interface_handle_session(interface_test):
+async def test_interface_session_wrapped(interface_test):
     reader = AsyncMock()
     reader.readuntil = AsyncMock(return_value=b'CONNECT https://example.com:443 HTTP/1.1')
     interface_test.https_handler = AsyncMock()
-    await interface_test.handle_session(reader=reader, writer=AsyncMock())
+    await interface_test.session_wrapped(reader=reader, writer=AsyncMock())
     interface_test.https_handler.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_interface_handle_session_request_error(interface_test, mocker: MockerFixture):
+async def test_interface_session_wrapped_request_error(interface_test, mocker: MockerFixture):
     reader = AsyncMock()
     reader.readuntil = AsyncMock(return_value=b'CONNECT https://example.com:443 HTTP/1.1')
     interface_test.https_handler = AsyncMock()
     mocked_rawparser = mocker.patch('ouija.interface.RawParser')
     mocked_rawparser.return_value = RawParser(data=b'')
-    await interface_test.handle_session(reader=reader, writer=AsyncMock())
+    await interface_test.session_wrapped(reader=reader, writer=AsyncMock())
     interface_test.https_handler.assert_not_awaited()
 
 
 @pytest.mark.asyncio
-async def test_interface_handle_session_method_error(interface_test):
+async def test_interface_session_wrapped_method_error(interface_test):
     reader = AsyncMock()
     reader.readuntil = AsyncMock(return_value=b'GET example.com HTTP/1.1')
     interface_test.https_handler = AsyncMock()
-    await interface_test.handle_session(reader=reader, writer=AsyncMock())
+    await interface_test.session_wrapped(reader=reader, writer=AsyncMock())
     interface_test.https_handler.assert_not_awaited()
 
 
 @pytest.mark.asyncio
 async def test_interface_session(interface_test):
-    interface_test.handle_session = AsyncMock()
-    await interface_test.session(reader=AsyncMock(), writer=AsyncMock())
-    interface_test.handle_session.assert_awaited()
+    interface_test.session_wrapped = AsyncMock()
+    await interface_test.session(index=0, reader=AsyncMock(), writer=AsyncMock())
+    interface_test.session_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=TimeoutError)
 async def test_interface_session_timeouterror(interface_test):
-    interface_test.handle_session = AsyncMock()
-    interface_test.handle_session.side_effect = TimeoutError()
-    await interface_test.session(reader=AsyncMock(), writer=AsyncMock())
-    interface_test.handle_session.assert_awaited()
+    interface_test.session_wrapped = AsyncMock()
+    interface_test.session_wrapped.side_effect = TimeoutError()
+    await interface_test.session(index=0, reader=AsyncMock(), writer=AsyncMock())
+    interface_test.session_wrapped.assert_awaited()
+
+
+@pytest.mark.asyncio
+@pytest.mark.xfail(raises=Exception)
+async def test_interface_session_exception(interface_test):
+    interface_test.session_wrapped = AsyncMock()
+    interface_test.session_wrapped.side_effect = Exception()
+    await interface_test.session(index=0, reader=AsyncMock(), writer=AsyncMock())
+    interface_test.session_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_interface_serve(interface_test):
     interface_test.session = AsyncMock()
     await interface_test.serve(reader=AsyncMock(), writer=AsyncMock())
     interface_test.session.assert_called()
```

### Comparing `ouija-0.3.0/tests/test_link.py` & `ouija-1.0.0/tests/test_link.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pytest
 from pytest_mock import MockerFixture
 
 from ouija import Packet, Phase
 
 
 @pytest.mark.asyncio
-async def test_link_sendto(link_test, data_test):
-    await link_test.sendto(data=data_test)
+async def test_link_on_send(link_test, data_test):
+    await link_test.on_send(data=data_test)
     link_test.proxy.transport.sendto.assert_called()
 
 
 @pytest.mark.asyncio
 async def test_link_on_open(link_test, token_test, mocker: MockerFixture):
     async def open_connection(*args, **kwargs):
         return AsyncMock(), AsyncMock()
@@ -31,14 +31,27 @@
     assert await link_test.on_open(packet=packet)
     assert link_test.opened.is_set()
     link_test.serve.assert_called()
     link_test.send_ack_open.assert_awaited()
 
 
 @pytest.mark.asyncio
+async def test_link_on_open_empty_remote(link_test, token_test):
+    link_test.opened.set()
+    link_test.send_ack_open = AsyncMock()
+    packet = Packet(
+        phase=Phase.OPEN,
+        ack=False,
+        token=token_test,
+    )
+    assert not await link_test.on_open(packet=packet)
+    link_test.send_ack_open.assert_not_awaited()
+
+
+@pytest.mark.asyncio
 async def test_link_on_open_opened(link_test, token_test):
     link_test.opened.set()
     link_test.send_ack_open = AsyncMock()
     packet = Packet(
         phase=Phase.OPEN,
         ack=False,
         token=token_test,
```

### Comparing `ouija-0.3.0/tests/test_ouija.py` & `ouija-1.0.0/tests/test_ouija.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import pytest
 
 from ouija import Packet, Phase
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=NotImplementedError)
-async def test_sendto(ouija_test, data_test):
-    await ouija_test.sendto(data=data_test)
+async def test_on_send(ouija_test, data_test):
+    await ouija_test.on_send(data=data_test)
 
 
 @pytest.mark.asyncio
 async def test_send(ouija_test, data_test):
-    ouija_test.sendto = AsyncMock()
+    ouija_test.on_send = AsyncMock()
     await ouija_test.send(data=data_test)
-    ouija_test.sendto.assert_awaited_with(data=data_test)
+    ouija_test.on_send.assert_awaited_with(data=data_test)
 
 
 @pytest.mark.asyncio
 async def test_send_packet(ouija_test, data_test):
     ouija_test.send = AsyncMock()
     packet = Packet(phase=Phase.DATA, ack=False, seq=0, data=data_test, drain=True)
     await ouija_test.send_packet(packet=packet)
@@ -70,29 +70,46 @@
     ouija_test.writer.drain.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_recv(ouija_test, data_test):
     ouija_test.write = AsyncMock()
     ouija_test.send_ack_data = AsyncMock()
-    await ouija_test.recv(seq=1, data=data_test, drain=False)
-    await ouija_test.recv(seq=2, data=data_test, drain=False)
-    await ouija_test.recv(seq=0, data=data_test, drain=False)
+    packet = Packet(
+        phase=Phase.DATA,
+        ack=False,
+        seq=1,
+        data=data_test,
+        drain=False,
+    )
+    await ouija_test.recv(packet=packet)
+    packet.seq = 2
+    await ouija_test.recv(packet=packet)
+    packet.seq = 0
+    await ouija_test.recv(packet=packet)
     ouija_test.write.assert_awaited()
     ouija_test.send_ack_data.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_recv_overload(ouija_test, data_test):
     ouija_test.write = AsyncMock()
     ouija_test.send_ack_data = AsyncMock()
     ouija_test.close = AsyncMock()
     ouija_test.tuning.udp_capacity = 1
-    await ouija_test.recv(seq=1, data=data_test, drain=False)
-    await ouija_test.recv(seq=2, data=data_test, drain=False)
+    packet = Packet(
+        phase=Phase.DATA,
+        ack=False,
+        seq=1,
+        data=data_test,
+        drain=False,
+    )
+    await ouija_test.recv(packet=packet)
+    packet.seq = 2
+    await ouija_test.recv(packet=packet)
     ouija_test.close.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_enqueue_send(ouija_test, data_test):
     ouija_test.send_packet = AsyncMock()
     await ouija_test.enqueue_send(data=data_test, drain=True)
@@ -182,322 +199,322 @@
 async def test_send_ack_close(ouija_test):
     ouija_test.send_packet = AsyncMock()
     await ouija_test.send_ack_close()
     ouija_test.send_packet.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_open(ouija_test, token_test):
+async def test_process_wrapped_open(ouija_test, token_test):
     ouija_test.check_token = AsyncMock(return_value=True)
     ouija_test.on_open = AsyncMock(return_value=True)
     packet = Packet(
         phase=Phase.OPEN,
         ack=False,
         token=token_test,
         host='example.com',
         port=443,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.check_token.assert_awaited()
     ouija_test.on_open.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_open_check_token_false(ouija_test, token_test):
+async def test_process_wrapped_open_check_token_false(ouija_test, token_test):
     ouija_test.check_token = AsyncMock(return_value=False)
     packet = Packet(
         phase=Phase.OPEN,
         ack=False,
         token=token_test,
         host='example.com',
         port=443,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.check_token.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_open_on_open_false(ouija_test, token_test):
+async def test_process_wrapped_open_on_open_false(ouija_test, token_test):
     ouija_test.on_open = AsyncMock(return_value=False)
     packet = Packet(
         phase=Phase.OPEN,
         ack=False,
         token=token_test,
         host='example.com',
         port=443,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.on_open.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_data_ack(ouija_test):
+async def test_process_wrapped_data_ack(ouija_test):
     ouija_test.opened.set()
     ouija_test.dequeue_send = AsyncMock()
     packet = Packet(
         phase=Phase.DATA,
         ack=True,
         seq=0,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.dequeue_send.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_data(ouija_test, data_test):
+async def test_process_wrapped_data(ouija_test, data_test):
     ouija_test.opened.set()
     ouija_test.recv = AsyncMock()
     packet = Packet(
         phase=Phase.DATA,
         ack=False,
         seq=0,
         data=data_test,
         drain=False,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.recv.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_data_not_opened(ouija_test, data_test):
+async def test_process_wrapped_data_not_opened(ouija_test, data_test):
     ouija_test.dequeue_send = AsyncMock()
     ouija_test.recv = AsyncMock()
     packet = Packet(
         phase=Phase.DATA,
         ack=False,
         seq=0,
         data=data_test,
         drain=False,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.dequeue_send.assert_not_awaited()
     ouija_test.recv.assert_not_awaited()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_close_ack(ouija_test):
+async def test_process_wrapped_close_ack(ouija_test):
     packet = Packet(
         phase=Phase.CLOSE,
         ack=True,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     assert ouija_test.read_closed.is_set()
 
 
 @pytest.mark.asyncio
-async def test_process_packet_close(ouija_test):
+async def test_process_wrapped_close(ouija_test):
     ouija_test.send_ack_close = AsyncMock()
     packet = Packet(
         phase=Phase.CLOSE,
         ack=False,
     )
-    await ouija_test.process_packet(data=packet.binary(fernet=ouija_test.tuning.fernet))
+    await ouija_test.process_wrapped(data=packet.binary(fernet=ouija_test.tuning.fernet))
     ouija_test.send_ack_close.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_process(ouija_test):
-    ouija_test.process_packet = AsyncMock()
+    ouija_test.process_wrapped = AsyncMock()
     packet = Packet(
         phase=Phase.CLOSE,
         ack=False,
     )
     await ouija_test.process(data=packet.binary(fernet=ouija_test.tuning.fernet))
-    ouija_test.process_packet.assert_awaited()
+    ouija_test.process_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=ConnectionError)
 async def test_process_connectionerror(ouija_test):
-    ouija_test.process_packet = AsyncMock()
-    ouija_test.process_packet.side_effect = ConnectionError()
+    ouija_test.process_wrapped = AsyncMock()
+    ouija_test.process_wrapped.side_effect = ConnectionError()
     packet = Packet(
         phase=Phase.CLOSE,
         ack=False,
     )
     await ouija_test.process(data=packet.binary(fernet=ouija_test.tuning.fernet))
-    ouija_test.process_packet.assert_awaited()
+    ouija_test.process_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=Exception)
 async def test_process_exception(ouija_test):
-    ouija_test.process_packet = AsyncMock()
-    ouija_test.process_packet.side_effect = Exception()
+    ouija_test.process_wrapped = AsyncMock()
+    ouija_test.process_wrapped.side_effect = Exception()
     ouija_test.close = AsyncMock()
     packet = Packet(
         phase=Phase.CLOSE,
         ack=False,
     )
     await ouija_test.process(data=packet.binary(fernet=ouija_test.tuning.fernet))
-    ouija_test.process_packet.assert_awaited()
+    ouija_test.process_wrapped.assert_awaited()
     ouija_test.close.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_resend_packets(ouija_test, data_test):
+async def test_resend_wrapped(ouija_test, data_test):
     ouija_test.close = AsyncMock()
     ouija_test.send = AsyncMock()
     ouija_test.send_close = AsyncMock()
     await ouija_test.enqueue_send(data=data_test, drain=True)
-    await ouija_test.resend_packets()
+    await ouija_test.resend_wrapped()
     ouija_test.close.assert_awaited()
     ouija_test.send.assert_awaited()
     ouija_test.send_close.assert_not_awaited()
 
 
 @pytest.mark.asyncio
-async def test_resend_packets_empty(ouija_test):
+async def test_resend_wrapped_empty(ouija_test):
     ouija_test.send_close = AsyncMock()
-    await ouija_test.resend_packets()
+    await ouija_test.resend_wrapped()
     ouija_test.send_close.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_resend(ouija_test):
-    ouija_test.resend_packets = AsyncMock()
+    ouija_test.resend_wrapped = AsyncMock()
     ouija_test.close = AsyncMock()
     await ouija_test.resend()
-    ouija_test.resend_packets.assert_awaited()
+    ouija_test.resend_wrapped.assert_awaited()
     ouija_test.close.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=TimeoutError)
 async def test_resend_timeouterror(ouija_test):
-    ouija_test.resend_packets = AsyncMock()
-    ouija_test.resend_packets.side_effect = TimeoutError()
+    ouija_test.resend_wrapped = AsyncMock()
+    ouija_test.resend_wrapped.side_effect = TimeoutError()
     ouija_test.close = AsyncMock()
     await ouija_test.resend()
-    ouija_test.resend_packets.assert_awaited()
+    ouija_test.resend_wrapped.assert_awaited()
     ouija_test.close.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=Exception)
 async def test_resend_exception(ouija_test):
-    ouija_test.resend_packets = AsyncMock()
-    ouija_test.resend_packets.side_effect = Exception()
+    ouija_test.resend_wrapped = AsyncMock()
+    ouija_test.resend_wrapped.side_effect = Exception()
     await ouija_test.resend()
-    ouija_test.resend_packets.assert_awaited()
+    ouija_test.resend_wrapped.assert_awaited()
     ouija_test.close.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=NotImplementedError)
 async def test_on_serve(ouija_test):
     await ouija_test.on_serve()
 
 
 @pytest.mark.asyncio
-async def test_serve_stream(ouija_test, data_test):
+async def test_serve_wrapped(ouija_test, data_test):
     async def resetter():
         await asyncio.sleep(3)
         ouija_test.opened.clear()
     ouija_test.on_serve = AsyncMock(return_value=True)
     ouija_test.resend = AsyncMock()
     ouija_test.read = AsyncMock(return_value=data_test)
     ouija_test.enqueue_send = AsyncMock()
     ouija_test.opened.set()
     asyncio.create_task(resetter())
-    await ouija_test.serve_stream()
+    await ouija_test.serve_wrapped()
     ouija_test.on_serve.assert_awaited()
     ouija_test.resend.assert_awaited()
     ouija_test.read.assert_awaited()
     ouija_test.enqueue_send.assert_awaited()
 
 
 @pytest.mark.asyncio
-async def test_serve_stream_on_serve_false(ouija_test, data_test):
+async def test_serve_wrapped_on_serve_false(ouija_test, data_test):
     async def resetter():
         await asyncio.sleep(3)
         ouija_test.opened.clear()
     ouija_test.on_serve = AsyncMock(return_value=False)
     ouija_test.resend = AsyncMock()
     ouija_test.read = AsyncMock(return_value=data_test)
     ouija_test.enqueue_send = AsyncMock()
     ouija_test.opened.set()
     asyncio.create_task(resetter())
-    await ouija_test.serve_stream()
+    await ouija_test.serve_wrapped()
     ouija_test.on_serve.assert_awaited()
     ouija_test.resend.assert_not_awaited()
     ouija_test.read.assert_not_awaited()
     ouija_test.enqueue_send.assert_not_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=TimeoutError)
-async def test_serve_stream_timeouterror(ouija_test, data_test):
+async def test_serve_wrapped_timeouterror(ouija_test, data_test):
     async def resetter():
         await asyncio.sleep(3)
         ouija_test.opened.clear()
     ouija_test.on_serve = AsyncMock(return_value=True)
     ouija_test.resend = AsyncMock()
     ouija_test.read = AsyncMock(return_value=data_test)
     ouija_test.read.side_effect = TimeoutError()
     ouija_test.enqueue_send = AsyncMock()
     ouija_test.opened.set()
     asyncio.create_task(resetter())
-    await ouija_test.serve_stream()
+    await ouija_test.serve_wrapped()
     ouija_test.on_serve.assert_awaited()
     ouija_test.resend.assert_awaited()
     ouija_test.read.assert_awaited()
     ouija_test.enqueue_send.assert_not_awaited()
 
 
 @pytest.mark.asyncio
-async def test_serve_stream_empty(ouija_test, data_test):
+async def test_serve_wrapped_empty(ouija_test, data_test):
     async def resetter():
         await asyncio.sleep(3)
         ouija_test.opened.clear()
     ouija_test.on_serve = AsyncMock(return_value=True)
     ouija_test.resend = AsyncMock()
     ouija_test.read = AsyncMock(return_value=b'')
     ouija_test.enqueue_send = AsyncMock()
     ouija_test.opened.set()
     asyncio.create_task(resetter())
-    await ouija_test.serve_stream()
+    await ouija_test.serve_wrapped()
     ouija_test.on_serve.assert_awaited()
     ouija_test.resend.assert_awaited()
     ouija_test.read.assert_awaited()
     ouija_test.enqueue_send.assert_not_awaited()
 
 
 @pytest.mark.asyncio
 async def test_serve(ouija_test):
-    ouija_test.serve_stream = AsyncMock()
+    ouija_test.serve_wrapped = AsyncMock()
     await ouija_test.serve()
-    ouija_test.serve_stream.assert_awaited()
+    ouija_test.serve_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=TimeoutError)
 async def test_serve_timeouterror(ouija_test):
-    ouija_test.serve_stream = AsyncMock()
-    ouija_test.serve_stream.side_effect = TimeoutError()
+    ouija_test.serve_wrapped = AsyncMock()
+    ouija_test.serve_wrapped.side_effect = TimeoutError()
     await ouija_test.serve()
-    ouija_test.serve_stream.assert_awaited()
+    ouija_test.serve_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=ConnectionError)
 async def test_serve_connectionerror(ouija_test):
-    ouija_test.serve_stream = AsyncMock()
-    ouija_test.serve_stream.side_effect = ConnectionError()
+    ouija_test.serve_wrapped = AsyncMock()
+    ouija_test.serve_wrapped.side_effect = ConnectionError()
     await ouija_test.serve()
-    ouija_test.serve_stream.assert_awaited()
+    ouija_test.serve_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 @pytest.mark.xfail(raises=Exception)
 async def test_serve_exception(ouija_test):
-    ouija_test.serve_stream = AsyncMock()
-    ouija_test.serve_stream.side_effect = Exception()
+    ouija_test.serve_wrapped = AsyncMock()
+    ouija_test.serve_wrapped.side_effect = Exception()
     await ouija_test.serve()
-    ouija_test.serve_stream.assert_awaited()
+    ouija_test.serve_wrapped.assert_awaited()
 
 
 @pytest.mark.asyncio
 async def test_close(ouija_test):
     ouija_test.opened.set()
     ouija_test.writer = AsyncMock(spec=asyncio.StreamWriter)
     ouija_test.writer.is_closing = lambda: False
```

### Comparing `ouija-0.3.0/tests/test_packet.py` & `ouija-1.0.0/tests/test_packet.py`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/tests/test_proxy.py` & `ouija-1.0.0/tests/test_proxy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest.mock import Mock, AsyncMock
 
 import pytest
+from pytest_mock import MockerFixture
 
 
 def test_proxy_connection_made(proxy_test):
     mock = Mock()
     proxy_test.connection_made(mock)
     assert proxy_test.transport == mock
 
@@ -25,7 +26,16 @@
 
 
 @pytest.mark.asyncio
 async def test_proxy_connection_lost(proxy_test):
     proxy_test.transport = AsyncMock()
     proxy_test.connection_lost(Exception())
     proxy_test.transport.close.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_proxy_serve(proxy_test, mocker: MockerFixture):
+    mocked_asyncio = mocker.patch('ouija.proxy.asyncio')
+    mocked_loop = AsyncMock()
+    mocked_asyncio.get_event_loop = lambda: mocked_loop
+    await proxy_test.serve()
+    mocked_loop.create_datagram_endpoint.assert_awaited()
```

### Comparing `ouija-0.3.0/tests/test_rawparser.py` & `ouija-1.0.0/tests/test_rawparser.py`

 * *Files identical despite different names*

### Comparing `ouija-0.3.0/tests/test_relay.py` & `ouija-1.0.0/tests/test_relay.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 async def test_relay_connection_lost(relay_test):
     relay_test.close = AsyncMock()
     relay_test.connection_lost(Exception())
     relay_test.close.assert_called()
 
 
 @pytest.mark.asyncio
-async def test_relay_sendto(relay_test, data_test):
+async def test_relay_on_send(relay_test, data_test):
     relay_test.transport = Mock()
-    await relay_test.sendto(data=data_test)
+    await relay_test.on_send(data=data_test)
     relay_test.transport.sendto.assert_called()
 
 
 @pytest.mark.asyncio
 async def test_relay_on_open(relay_test, token_test):
     relay_test.write = AsyncMock()
     packet = Packet(
```

### Comparing `ouija-0.3.0/tests/test_telemetry.py` & `ouija-1.0.0/tests/test_telemetry.py`

 * *Files identical despite different names*


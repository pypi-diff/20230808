# Comparing `tmp/pyagentx3-0.1.3.tar.gz` & `tmp/pyagentx3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyagentx3-0.1.3.tar", last modified: Fri Apr  8 10:06:58 2022, max compression
+gzip compressed data, was "pyagentx3-0.1.4.tar", last modified: Tue Aug  8 19:31:21 2023, max compression
```

## Comparing `pyagentx3-0.1.3.tar` & `pyagentx3-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/
--rw-rw-r--   0 prinz     (1000) prinz     (1000)     1273 2022-04-08 10:04:53.000000 pyagentx3-0.1.3/setup.py
--rw-r--r--   0 prinz     (1000) prinz     (1000)     6281 2022-04-08 08:08:05.000000 pyagentx3-0.1.3/README.md
-drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3/
--rw-rw-r--   0 prinz     (1000) prinz     (1000)     1063 2022-04-08 07:27:44.000000 pyagentx3-0.1.3/pyagentx3/tools.py
--rw-rw-r--   0 prinz     (1000) prinz     (1000)     4068 2022-04-08 07:27:44.000000 pyagentx3-0.1.3/pyagentx3/__init__.py
--rw-rw-r--   0 prinz     (1000) prinz     (1000)    13116 2022-04-08 08:22:01.000000 pyagentx3-0.1.3/pyagentx3/pdu.py
--rw-rw-r--   0 prinz     (1000) prinz     (1000)    10590 2022-04-08 09:51:16.000000 pyagentx3-0.1.3/pyagentx3/network.py
--rw-rw-r--   0 prinz     (1000) prinz     (1000)     2800 2022-04-08 09:32:22.000000 pyagentx3-0.1.3/pyagentx3/agent.py
--rw-r--r--   0 prinz     (1000) prinz     (1000)     4987 2021-03-01 19:42:59.000000 pyagentx3-0.1.3/pyagentx3/updater.py
--rw-r--r--   0 prinz     (1000) prinz     (1000)     1797 2020-08-11 11:03:28.000000 pyagentx3-0.1.3/pyagentx3/sethandler.py
-drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3.egg-info/
--rw-r--r--   0 prinz     (1000) prinz     (1000)      293 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3.egg-info/SOURCES.txt
--rw-r--r--   0 prinz     (1000) prinz     (1000)        1 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3.egg-info/dependency_links.txt
--rw-r--r--   0 prinz     (1000) prinz     (1000)     1251 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3.egg-info/PKG-INFO
--rw-r--r--   0 prinz     (1000) prinz     (1000)       10 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/pyagentx3.egg-info/top_level.txt
--rw-rw-r--   0 prinz     (1000) prinz     (1000)     1251 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/PKG-INFO
--rw-rw-r--   0 prinz     (1000) prinz     (1000)       38 2022-04-08 10:06:58.000000 pyagentx3-0.1.3/setup.cfg
+drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2023-08-08 19:31:21.707409 pyagentx3-0.1.4/
+-rw-r--r--   0 prinz     (1000) prinz     (1000)     1392 2020-08-10 10:34:45.000000 pyagentx3-0.1.4/LICENSE.txt
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)     1145 2023-08-08 19:31:21.707409 pyagentx3-0.1.4/PKG-INFO
+-rw-r--r--   0 prinz     (1000) prinz     (1000)     6281 2022-04-08 08:08:05.000000 pyagentx3-0.1.4/README.md
+drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2023-08-08 19:31:21.707409 pyagentx3-0.1.4/pyagentx3/
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)     5748 2023-06-16 12:58:17.000000 pyagentx3-0.1.4/pyagentx3/__init__.py
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)     2800 2022-04-08 09:32:22.000000 pyagentx3-0.1.4/pyagentx3/agent.py
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)    12059 2023-06-16 13:38:03.000000 pyagentx3-0.1.4/pyagentx3/network.py
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)    13555 2023-06-16 13:38:20.000000 pyagentx3-0.1.4/pyagentx3/pdu.py
+-rw-r--r--   0 prinz     (1000) prinz     (1000)     1797 2020-08-11 11:03:28.000000 pyagentx3-0.1.4/pyagentx3/sethandler.py
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)     1063 2022-04-08 07:27:44.000000 pyagentx3-0.1.4/pyagentx3/tools.py
+-rw-r--r--   0 prinz     (1000) prinz     (1000)     4987 2021-03-01 19:42:59.000000 pyagentx3-0.1.4/pyagentx3/updater.py
+drwxrwxr-x   0 prinz     (1000) prinz     (1000)        0 2023-08-08 19:31:21.707409 pyagentx3-0.1.4/pyagentx3.egg-info/
+-rw-r--r--   0 prinz     (1000) prinz     (1000)     1145 2023-08-08 19:31:21.000000 pyagentx3-0.1.4/pyagentx3.egg-info/PKG-INFO
+-rw-r--r--   0 prinz     (1000) prinz     (1000)      305 2023-08-08 19:31:21.000000 pyagentx3-0.1.4/pyagentx3.egg-info/SOURCES.txt
+-rw-r--r--   0 prinz     (1000) prinz     (1000)        1 2023-08-08 19:31:21.000000 pyagentx3-0.1.4/pyagentx3.egg-info/dependency_links.txt
+-rw-r--r--   0 prinz     (1000) prinz     (1000)       10 2023-08-08 19:31:21.000000 pyagentx3-0.1.4/pyagentx3.egg-info/top_level.txt
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)       38 2023-08-08 19:31:21.707409 pyagentx3-0.1.4/setup.cfg
+-rw-rw-r--   0 prinz     (1000) prinz     (1000)     1276 2023-08-08 19:30:04.000000 pyagentx3-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyagentx3-0.1.3/setup.py` & `pyagentx3-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 
 setup(
     name = "pyagentx3",
-    version = "0.1.3",
+    version = "0.1.4",
     author = "Richard Prinz",
     author_email = "richard.prinz@min.at",
-    description = ("AgentX package to extend SNMP with pure Python3"),
+    description = ("AgentX package to extend SNMP with pure Python3.10"),
     license = "BSD",
     keywords = "snmp network agentx ",
     url = "https://github.com/rprinz08/pyagentx3",
     packages=['pyagentx3'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
```

### Comparing `pyagentx3-0.1.3/README.md` & `pyagentx3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyagentx3-0.1.3/pyagentx3/tools.py` & `pyagentx3-0.1.4/pyagentx3/tools.py`

 * *Files identical despite different names*

### Comparing `pyagentx3-0.1.3/pyagentx3/pdu.py` & `pyagentx3-0.1.4/pyagentx3/pdu.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             buf += struct.pack('!L', oid[i])
         return buf
 
     def encode_octet(self, octet):
         data_len = 0
         data = octet
 
-        if not isinstance(octet, collections.Sized):
+        if not isinstance(octet, collections.abc.Sized):
             if isinstance(octet, IPv4Address) or isinstance(octet, IPv6Address):
                 data = octet.packed
             else:
                 data = str(octet)
 
         if isinstance(data, str):
             data = data.encode('latin1')
@@ -123,15 +123,15 @@
             # No data
             pass
         else:
             logger.error('Unknown Type: %s', pdu_type)
         return buf
 
     def encode_header(self, pdu_type, payload_length=0, flags=0):
-        flags = flags | 0x10  # Bit 5 = all ints in NETWORK_BYTE_ORDER
+        flags = flags | pyagentx3.AX_PDU_FLAG_BYTE_ORDER # Bit 5 = all ints in NETWORK_BYTE_ORDER
         buf = struct.pack('BBBB', 1, pdu_type, flags, 0)
         buf += struct.pack('!L', self.session_id) # sessionID
         buf += struct.pack('!L', self.transaction_id) # transactionID
         buf += struct.pack('!L', self.packet_id) # packetID
         buf += struct.pack('!L', payload_length)
         return buf
 
@@ -294,51 +294,64 @@
             except Exception:
                 logger.exception('Unable to decode value of type (%d %s) for OID (%s)',
                     vtype, pyagentx3.TYPE_NAME.get(vtype, 'UNKNOWN'), oid)
                 ok = False
 
         return {'type':vtype, 'name':oid, 'data':data}, ok
 
-    def decode_header(self):
+    @staticmethod
+    def decode_header(buf):
         try:
-            t = struct.unpack('!BBBBLLLL', self.decode_buf[:20])
-            self.decode_buf = self.decode_buf[20:]
+            t = struct.unpack('!BBBBLLLL', buf[:pyagentx3.AX_PDU_HDR_LEN])
             ret = {
                 'version': t[0],
                 'pdu_type':t[1],
-                'pdu_type_name':  pyagentx3.PDU_TYPE_NAME[t[1]],
+                'pdu_type_name': pyagentx3.PDU_TYPE_NAME[t[1]],
                 'flags':t[2],
                 'reserved':t[3],
                 'session_id':t[4],
                 'transaction_id':t[5],
                 'packet_id':t[6],
                 'payload_length':t[7],
             }
+            return ret
+        except Exception:
+            return None
+
+    def _decode_header(self):
+        try:
+            ret = self.__class__.decode_header(self.decode_buf)
+            self.decode_buf = self.decode_buf[pyagentx3.AX_PDU_HDR_LEN:]
+            if not isinstance(ret, dict):
+                raise Exception("Invalid PDU header")
+
             self.state = ret
             self.type = ret['pdu_type']
             self.session_id = ret['session_id']
             self.packet_id = ret['packet_id']
             self.transaction_id = ret['transaction_id']
             self.decode_buf = self.decode_buf[:ret['payload_length']]
-            if ret['flags'] & 0x08:  # content present
+            if ret['flags'] & pyagentx3.AX_PDU_FLAG_CONTEXT:  # content present
                 context = self.decode_octet()
                 logger.debug('Context: %s', context)
             return ret
         except Exception:
             logger.exception('Invalid packing: %d', len(self.decode_buf))
             logger.debug('%s', pprint.pformat(self.decode_buf))
 
     def decode(self, buf):
         self.set_decode_buf(buf)
 
         logger.debug('Decode AgentX PDU:')
         for i in hexdump(self.decode_buf, sep='-'):
             logger.debug(i)
 
-        ret = self.decode_header()
+        ret = self._decode_header()
+        if not isinstance(ret, dict):
+            return
         if ret['pdu_type'] == pyagentx3.AGENTX_RESPONSE_PDU:
             # Decode Response Header
             t = struct.unpack('!LHH', self.decode_buf[:8])
             self.decode_buf = self.decode_buf[8:]
             self.response = {
                 'sysUpTime': t[0],
                 'error':t[1],
@@ -371,8 +384,7 @@
                                  pyagentx3.AGENTX_CLEANUPSET_PDU]:
             pass
 
         else:
             pdu_type_str = pyagentx3.PDU_TYPE_NAME.get(ret['pdu_type'],
                 'Unknown:'+ str(ret['pdu_type']))
             logger.error('Unsupported PDU type: %s', pdu_type_str)
-
```

### Comparing `pyagentx3-0.1.3/pyagentx3/network.py` & `pyagentx3-0.1.4/pyagentx3/network.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 logger.addHandler(NullHandler())
 # --------------------------------------------
 
 import socket
 import time
 import threading
 from queue import Empty
+import struct
 import pyagentx3
 from pyagentx3.pdu import PDU
 
 
 class Network(threading.Thread):
 
     def __init__(self, queue, oid_list, sethandlers, agent_id, socket_path):
         threading.Thread.__init__(self)
         self.stop = threading.Event()
         self._agent_id = agent_id
         self._socket_path = socket_path
         self._queue = queue
         self._oid_list = oid_list
         self._sethandlers = sethandlers
+        self._recv_buf = bytes()
 
         self.session_id = 0
         self.transaction_id = 0
         self.debug = 1
         # Data Related Variables
         self.data = {}
         self.data_idx = []
@@ -68,23 +70,54 @@
         if self.debug or force:
             logger.log(log_level, "---- Sent PDU:")
             pdu.dump()
         buf = pdu.encode()
         self.socket.send(buf)
 
     def recv_pdu(self):
-        buf = self.socket.recv(1024)
-        if not buf:
+        # Try to read next n bytes from socket until at least a full
+        # PDU header is available.
+        if len(self._recv_buf) < pyagentx3.AX_PDU_HDR_LEN:
+            self._recv_buf += self.socket.recv(4096)
+            if len(self._recv_buf) < pyagentx3.AX_PDU_HDR_LEN:
+                return None
+
+        # Try to decode a PDU header from beginning of buffer.
+        hdr = PDU.decode_header(self._recv_buf[:pyagentx3.AX_PDU_HDR_LEN])
+        # If its not possible to decode a PDU header from buffer, remove
+        # invalid PDU header from buffer.
+        if not isinstance(hdr, dict):
+            self._recv_buf = self._recv_buf[pyagentx3.AX_PDU_HDR_LEN:]
             return None
-        pdu = PDU()
+        payload_len = hdr["payload_length"]
+
+        # Ensure that full PDU is in buffer.
+        # Note: Max PDU payload length could be ~4GB,
+        # this could be problematic ...
+        next_pdu_len = pyagentx3.AX_PDU_HDR_LEN + payload_len
+        if len(self._recv_buf) < next_pdu_len:
+            self._recv_buf += self.socket.recv(next_pdu_len)
+            if len(self._recv_buf) < next_pdu_len:
+                return None
+
         if self.debug:
             logger.debug("---- Received PDU:")
-        pdu.decode(buf)
+
+        # Payload length valid, so decode complete PDU.
+        pdu = PDU()
+        pdu.decode(self._recv_buf[:next_pdu_len])
+        self._recv_buf = self._recv_buf[next_pdu_len:]
+
         if self.debug:
             pdu.dump()
+            logger.debug("---- Remaining buffer length ({})".format(
+                len(self._recv_buf)))
+            logger.debug("---- Buffer length ({}), PDU length ({})".format(
+                len(self._recv_buf), next_pdu_len))
+
         return pdu
 
     # =========================================
 
     def _get_updates(self):
         while True:
             try:
```

### Comparing `pyagentx3-0.1.3/pyagentx3/agent.py` & `pyagentx3-0.1.4/pyagentx3/agent.py`

 * *Files identical despite different names*

### Comparing `pyagentx3-0.1.3/pyagentx3/updater.py` & `pyagentx3-0.1.4/pyagentx3/updater.py`

 * *Files identical despite different names*

### Comparing `pyagentx3-0.1.3/pyagentx3/sethandler.py` & `pyagentx3-0.1.4/pyagentx3/sethandler.py`

 * *Files identical despite different names*

### Comparing `pyagentx3-0.1.3/pyagentx3.egg-info/PKG-INFO` & `pyagentx3-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyagentx3
-Version: 0.1.3
-Summary: AgentX package to extend SNMP with pure Python3
+Version: 0.1.4
+Summary: AgentX package to extend SNMP with pure Python3.10
 Home-page: https://github.com/rprinz08/pyagentx3
 Author: Richard Prinz
 Author-email: richard.prinz@min.at
 License: BSD
-Description: PyAgentX3
-        --------------------
-        pyagentx3 is a pure Python3 implementation of AgentX protocol (RFC 2741), it
-        will allow you to extend an SNMP agent (e.g. snmpd) by writing AgentX subagents,
-        without modifying the original SNMP agent.
-        
-        The agent can support the following commands:
-        - snmpget
-        - snmpwalk
-        - snmptable
-        - snmpset
-        
-        It also allows sending notifications/traps.
-        
 Keywords: snmp network agentx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
+License-File: LICENSE.txt
+
+PyAgentX3
+--------------------
+pyagentx3 is a pure Python3 implementation of AgentX protocol (RFC 2741), it
+will allow you to extend an SNMP agent (e.g. snmpd) by writing AgentX subagents,
+without modifying the original SNMP agent.
+
+The agent can support the following commands:
+- snmpget
+- snmpwalk
+- snmptable
+- snmpset
+
+It also allows sending notifications/traps.
```

### Comparing `pyagentx3-0.1.3/PKG-INFO` & `pyagentx3-0.1.4/pyagentx3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyagentx3
-Version: 0.1.3
-Summary: AgentX package to extend SNMP with pure Python3
+Version: 0.1.4
+Summary: AgentX package to extend SNMP with pure Python3.10
 Home-page: https://github.com/rprinz08/pyagentx3
 Author: Richard Prinz
 Author-email: richard.prinz@min.at
 License: BSD
-Description: PyAgentX3
-        --------------------
-        pyagentx3 is a pure Python3 implementation of AgentX protocol (RFC 2741), it
-        will allow you to extend an SNMP agent (e.g. snmpd) by writing AgentX subagents,
-        without modifying the original SNMP agent.
-        
-        The agent can support the following commands:
-        - snmpget
-        - snmpwalk
-        - snmptable
-        - snmpset
-        
-        It also allows sending notifications/traps.
-        
 Keywords: snmp network agentx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
+License-File: LICENSE.txt
+
+PyAgentX3
+--------------------
+pyagentx3 is a pure Python3 implementation of AgentX protocol (RFC 2741), it
+will allow you to extend an SNMP agent (e.g. snmpd) by writing AgentX subagents,
+without modifying the original SNMP agent.
+
+The agent can support the following commands:
+- snmpget
+- snmpwalk
+- snmptable
+- snmpset
+
+It also allows sending notifications/traps.
```


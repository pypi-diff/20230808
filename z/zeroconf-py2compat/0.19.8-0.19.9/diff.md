# Comparing `tmp/zeroconf-py2compat-0.19.8.tar.gz` & `tmp/zeroconf-py2compat-0.19.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zeroconf-py2compat-0.19.8.tar", last modified: Mon Jun 29 05:08:50 2020, max compression
+gzip compressed data, was "dist/zeroconf-py2compat-0.19.9.tar", last modified: Wed Jul 15 17:00:19 2020, max compression
```

## Comparing `zeroconf-py2compat-0.19.8.tar` & `zeroconf-py2compat-0.19.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jamalex   (1000) jamalex   (1000)        0 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/
--rw-r--r--   0 jamalex   (1000) jamalex   (1000)    14003 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/PKG-INFO
--rw-r--r--   0 jamalex   (1000) jamalex   (1000)     9680 2020-06-29 05:06:56.000000 zeroconf-py2compat-0.19.8/README.rst
--rw-r--r--   0 jamalex   (1000) jamalex   (1000)    32777 2020-05-22 22:28:41.000000 zeroconf-py2compat-0.19.8/enum_compat.py
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)      173 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/setup.cfg
--rwxr-xr-x   0 jamalex   (1000) jamalex   (1000)     2117 2020-06-29 05:05:55.000000 zeroconf-py2compat-0.19.8/setup.py
--rw-r--r--   0 jamalex   (1000) jamalex   (1000)    75615 2020-06-29 05:05:26.000000 zeroconf-py2compat-0.19.8/zeroconf.py
-drwxr-xr-x   0 jamalex   (1000) jamalex   (1000)        0 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)    14003 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/PKG-INFO
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)      306 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/SOURCES.txt
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)        1 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/dependency_links.txt
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)        1 2019-06-17 23:45:25.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/not-zip-safe
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)       10 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/requires.txt
--rw-rw-r--   0 jamalex   (1000) jamalex   (1000)       21 2020-06-29 05:08:50.000000 zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/top_level.txt
+drwxr-xr-x   0 jamalex   (1000) jamalex   (1000)        0 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/
+-rw-r--r--   0 jamalex   (1000) jamalex   (1000)    14155 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/PKG-INFO
+-rw-r--r--   0 jamalex   (1000) jamalex   (1000)     9783 2020-07-15 17:00:06.000000 zeroconf-py2compat-0.19.9/README.rst
+-rw-r--r--   0 jamalex   (1000) jamalex   (1000)    32777 2020-05-22 22:28:41.000000 zeroconf-py2compat-0.19.9/enum_compat.py
+-rw-r--r--   0 jamalex   (1000) jamalex   (1000)      173 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/setup.cfg
+-rwxr-xr-x   0 jamalex   (1000) jamalex   (1000)     2134 2020-07-15 17:00:06.000000 zeroconf-py2compat-0.19.9/setup.py
+-rw-r--r--   0 jamalex   (1000) jamalex   (1000)    75654 2020-07-15 17:00:06.000000 zeroconf-py2compat-0.19.9/zeroconf.py
+drwxr-xr-x   0 jamalex   (1000) jamalex   (1000)        0 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)    14155 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/PKG-INFO
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)      306 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/SOURCES.txt
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)        1 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/dependency_links.txt
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)        1 2019-06-17 23:45:25.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/not-zip-safe
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)       10 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/requires.txt
+-rw-rw-r--   0 jamalex   (1000) jamalex   (1000)       21 2020-07-15 17:00:19.000000 zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/top_level.txt
```

### Comparing `zeroconf-py2compat-0.19.8/PKG-INFO` & `zeroconf-py2compat-0.19.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.1
 Name: zeroconf-py2compat
-Version: 0.19.8
+Version: 0.19.9
 Summary: Pure Python Multicast DNS Service Discovery Library (Bonjour/Avahi compatible)
 Home-page: https://github.com/learningequality/python-zeroconf
-Author: Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre
+Author: Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre, Richard Tibbles
 Author-email: UNKNOWN
 License: LGPL
 Description: python-zeroconf-py2compat
         =========================
             
         This is a fork of pyzeroconf, Multicast DNS Service Discovery for Python,
         originally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),
@@ -105,14 +105,18 @@
             print('\n'.join(ZeroconfServiceTypes.find()))
         
         See examples directory for more.
         
         Changelog
         =========
         
+        0.19.9
+        ------
+        Turn _GLOBAL_DONE into a threading Event to allow for better interruptability at close.
+        
         0.19.8
         ------
         Handle exceptions in interface enumeration and just return an empty list.
         
         0.19.7
         ------
         Reverted from ifaddr back to ifcfg.
```

### Comparing `zeroconf-py2compat-0.19.8/README.rst` & `zeroconf-py2compat-0.19.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,18 @@
     print('\n'.join(ZeroconfServiceTypes.find()))
 
 See examples directory for more.
 
 Changelog
 =========
 
+0.19.9
+------
+Turn _GLOBAL_DONE into a threading Event to allow for better interruptability at close.
+
 0.19.8
 ------
 Handle exceptions in interface enumeration and just return an empty list.
 
 0.19.7
 ------
 Reverted from ifaddr back to ifcfg.
```

### Comparing `zeroconf-py2compat-0.19.8/enum_compat.py` & `zeroconf-py2compat-0.19.9/enum_compat.py`

 * *Files identical despite different names*

### Comparing `zeroconf-py2compat-0.19.8/setup.py` & `zeroconf-py2compat-0.19.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="zeroconf-py2compat",
     version=version,
     description="Pure Python Multicast DNS Service Discovery Library "
     "(Bonjour/Avahi compatible)",
     long_description=readme,
-    author="Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre",
+    author="Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre, Richard Tibbles",
     url="https://github.com/learningequality/python-zeroconf",
     py_modules=["zeroconf", "enum_compat"],
     platforms=["unix", "linux", "osx"],
     license="LGPL",
     zip_safe=False,
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `zeroconf-py2compat-0.19.8/zeroconf.py` & `zeroconf-py2compat-0.19.9/zeroconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from six import binary_type, indexbytes, int2byte, iteritems, text_type
 from six.moves import xrange
 
 import enum_compat as enum
 
 __author__ = "Paul Scott-Murphy, William McBrine"
 __maintainer__ = "Jamie Alexandre <jamie@learningequality.org>"
-__version__ = "0.19.8"
+__version__ = "0.19.9"
 __license__ = "LGPL"
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
@@ -1730,17 +1730,18 @@
                     else:
                         interfaces.append({"inet": "", "inet6": address})
         except Exception as e:
             return []
 
         return interfaces
 
+
 else:
 
-     def get_network_interfaces():
+    def get_network_interfaces():
         try:
             return ifcfg.interfaces().values()
         except:  # ifcfg throws an Exception if the ip/ifconfig commands are not found
             return []
 
 
 def get_all_addresses():
@@ -1806,15 +1807,15 @@
     def __init__(self, interfaces=InterfaceChoice.All):
         """Creates an instance of the Zeroconf class, establishing
         multicast communications, listening and reaping threads.
 
         :type interfaces: :class:`InterfaceChoice` or sequence of ip addresses
         """
         # hook for threads
-        self._GLOBAL_DONE = False
+        self._GLOBAL_DONE = threading.Event()
 
         self._listen_socket = new_socket()
         interfaces = normalize_interface_choice(interfaces)
 
         self._respond_sockets = []
 
         for i in interfaces:
@@ -1863,15 +1864,15 @@
         self.engine.add_reader(self.listener, self._listen_socket)
         self.reaper = Reaper(self)
 
         self.debug = None
 
     @property
     def done(self):
-        return self._GLOBAL_DONE
+        return self._GLOBAL_DONE.wait(0.1)
 
     def wait(self, timeout):
         """Calling thread waits for a given number of milliseconds or
         until notified."""
         with self.condition:
             self.condition.wait(timeout / 1000.0)
 
@@ -2272,15 +2273,15 @@
         if len(packet) > _MAX_MSG_ABSOLUTE:
             self.log_warning_once(
                 "Dropping %r over-sized packet (%d bytes) %r", out, len(packet), packet
             )
             return
         log.debug("Sending %r (%d bytes) as %r...", out, len(packet), packet)
         for s in self._respond_sockets:
-            if self._GLOBAL_DONE:
+            if self._GLOBAL_DONE.is_set():
                 return
             try:
                 outgoing_ip = s.getsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_IF, 4)
                 socket_packet = packet.replace(
                     USE_IP_OF_OUTGOING_INTERFACE, outgoing_ip
                 )
                 bytes_sent = s.sendto(socket_packet, 0, (addr, port))
@@ -2293,19 +2294,19 @@
                         "!!! sent %d out of %d bytes to %r"
                         % (bytes_sent, len(socket_packet), s)
                     )
 
     def close(self):
         """Ends the background threads, and prevent this instance from
         servicing further queries."""
-        if not self._GLOBAL_DONE:
+        if not self._GLOBAL_DONE.is_set():
             # remove service listeners
             self.remove_all_service_listeners()
             self.unregister_all_services()
-            self._GLOBAL_DONE = True
+            self._GLOBAL_DONE.set()
 
             # shutdown recv socket and thread
             self.engine.del_reader(self._listen_socket)
             self._listen_socket.close()
             self.engine.join()
 
             # shutdown the rest
```

### Comparing `zeroconf-py2compat-0.19.8/zeroconf_py2compat.egg-info/PKG-INFO` & `zeroconf-py2compat-0.19.9/zeroconf_py2compat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 1.1
 Name: zeroconf-py2compat
-Version: 0.19.8
+Version: 0.19.9
 Summary: Pure Python Multicast DNS Service Discovery Library (Bonjour/Avahi compatible)
 Home-page: https://github.com/learningequality/python-zeroconf
-Author: Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre
+Author: Paul Scott-Murphy, William McBrine, Jakub Stasiak, Jamie Alexandre, Richard Tibbles
 Author-email: UNKNOWN
 License: LGPL
 Description: python-zeroconf-py2compat
         =========================
             
         This is a fork of pyzeroconf, Multicast DNS Service Discovery for Python,
         originally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),
@@ -105,14 +105,18 @@
             print('\n'.join(ZeroconfServiceTypes.find()))
         
         See examples directory for more.
         
         Changelog
         =========
         
+        0.19.9
+        ------
+        Turn _GLOBAL_DONE into a threading Event to allow for better interruptability at close.
+        
         0.19.8
         ------
         Handle exceptions in interface enumeration and just return an empty list.
         
         0.19.7
         ------
         Reverted from ifaddr back to ifcfg.
```


# Comparing `tmp/AIOAladdinConnect-0.1.8.tar.gz` & `tmp/AIOAladdinConnect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIOAladdinConnect-0.1.8.tar", last modified: Wed Jun  1 17:48:20 2022, max compression
+gzip compressed data, was "AIOAladdinConnect-0.1.9.tar", last modified: Wed Jun  1 20:18:56 2022, max compression
```

## Comparing `AIOAladdinConnect-0.1.8.tar` & `AIOAladdinConnect-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 17:48:20.822739 AIOAladdinConnect-0.1.8/
-drwxrwxrwx   0        0        0        0 2022-06-01 17:48:20.785944 AIOAladdinConnect-0.1.8/AIOAladdinConnect/
--rw-rw-rw-   0        0        0     8544 2022-06-01 17:41:06.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect/__init__.py
--rw-rw-rw-   0        0        0     3321 2022-06-01 16:56:49.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect/eventsocket.py
--rw-rw-rw-   0        0        0     5376 2022-06-01 17:29:06.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect/session_manager.py
-drwxrwxrwx   0        0        0        0 2022-06-01 17:48:20.818224 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/
--rw-rw-rw-   0        0        0     2637 2022-06-01 17:48:19.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2022-06-01 17:48:20.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-01 17:48:20.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-06-01 17:48:20.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-06-01 17:48:20.000000 AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2637 2022-06-01 17:48:20.824570 AIOAladdinConnect-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1982 2022-06-01 13:55:13.000000 AIOAladdinConnect-0.1.8/README.md
--rw-rw-rw-   0        0        0       86 2022-06-01 17:48:20.827746 AIOAladdinConnect-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      984 2022-06-01 17:47:49.000000 AIOAladdinConnect-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:18:56.214111 AIOAladdinConnect-0.1.9/
+drwxrwxrwx   0        0        0        0 2022-06-01 20:18:56.170574 AIOAladdinConnect-0.1.9/AIOAladdinConnect/
+-rw-rw-rw-   0        0        0     8616 2022-06-01 20:17:52.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect/__init__.py
+-rw-rw-rw-   0        0        0     3321 2022-06-01 16:56:49.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect/eventsocket.py
+-rw-rw-rw-   0        0        0     5376 2022-06-01 17:53:57.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect/session_manager.py
+drwxrwxrwx   0        0        0        0 2022-06-01 20:18:56.206111 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/
+-rw-rw-rw-   0        0        0     2637 2022-06-01 20:18:54.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2022-06-01 20:18:55.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-01 20:18:54.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-06-01 20:18:55.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2022-06-01 20:18:55.000000 AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2637 2022-06-01 20:18:56.215109 AIOAladdinConnect-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1982 2022-06-01 13:55:13.000000 AIOAladdinConnect-0.1.9/README.md
+-rw-rw-rw-   0        0        0       86 2022-06-01 20:18:56.219107 AIOAladdinConnect-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      984 2022-06-01 20:18:26.000000 AIOAladdinConnect-0.1.9/setup.py
```

### Comparing `AIOAladdinConnect-0.1.8/AIOAladdinConnect/__init__.py` & `AIOAladdinConnect-0.1.9/AIOAladdinConnect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,14 @@
     }
 
     CONTROLLER_STATUS = {
         0: 'Offline',
         1: STATUS_CONNECTED
     }
 
-    
-
     def __init__(self, email:str, password:str,attr_changed:Callable):
         self._session = SessionManager(email, password)
         self._eventsocket = None
         self._doors = {'device_id':0}
         self._attr_changed = attr_changed
     
     def register_callback(self,update_callback:Callable):
@@ -196,24 +194,29 @@
             if door["device_id"] == device_id and door["door_number"] == door_number:
                 return door["rssi"]
 
     async def _call_back(self,msg):
         """Call back from AIO HTTP web socket with door status information"""
         # Opening and Closing only are sent if the WEB API called the open/close event
         # pressing the local button only results in a state change of open or close.
-        self._LOGGER.debug(f"Got the callback {json.loads(msg)}")
+        _LOGGER.debug(f"Got the callback {json.loads(msg)}")
         json_msg = json.loads(msg)
         for door in self._doors:
             # There are multiple messages from the websocket for the same value - filter this off
             if json_msg['door'] == door['door_number'] and self.DOOR_STATUS[json_msg['door_status']] != door['status']:
                 door.update({'status': self.DOOR_STATUS[json_msg["door_status"]]})
-                self._LOGGER.debug(f"Status Updated {self.DOOR_STATUS[json_msg['door_status']]}")
+                _LOGGER.debug(f"Status Updated {self.DOOR_STATUS[json_msg['door_status']]}")
                 if self._attr_changed:
                     await self._attr_changed()
             else:
-                self._LOGGER.debug(f"Status NOT updated {self.DOOR_STATUS[json_msg['door_status']]}")
+                _LOGGER.debug(f"Status NOT updated {self.DOOR_STATUS[json_msg['door_status']]}")
 
     def auth_token(self):
         return self._session.auth_token()
 
     def set_auth_token(self,auth_token):
         self._session.set_auth_token(auth_token)
+        if self._eventsocket:
+            self._eventsocket.set_auth_token(auth_token)
+
+
+
```

### Comparing `AIOAladdinConnect-0.1.8/AIOAladdinConnect/eventsocket.py` & `AIOAladdinConnect-0.1.9/AIOAladdinConnect/eventsocket.py`

 * *Files identical despite different names*

### Comparing `AIOAladdinConnect-0.1.8/AIOAladdinConnect/session_manager.py` & `AIOAladdinConnect-0.1.9/AIOAladdinConnect/session_manager.py`

 * *Files identical despite different names*

### Comparing `AIOAladdinConnect-0.1.8/AIOAladdinConnect.egg-info/PKG-INFO` & `AIOAladdinConnect-0.1.9/AIOAladdinConnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AIOAladdinConnect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Async API for controlling Genie garage doors connected to Aladdin Connect devices
 Home-page: http://github.com/mkmer/AIOAladdinConnect
-Download-URL: https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.9.tar.gz
 Author: Mike Kasper
 Author-email: m_kasper@sbcglobal.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIOAladdinConnect-0.1.8/PKG-INFO` & `AIOAladdinConnect-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: AIOAladdinConnect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Async API for controlling Genie garage doors connected to Aladdin Connect devices
 Home-page: http://github.com/mkmer/AIOAladdinConnect
-Download-URL: https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.8.tar.gz
+Download-URL: https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.9.tar.gz
 Author: Mike Kasper
 Author-email: m_kasper@sbcglobal.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIOAladdinConnect-0.1.8/README.md` & `AIOAladdinConnect-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `AIOAladdinConnect-0.1.8/setup.py` & `AIOAladdinConnect-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='AIOAladdinConnect',
-    version='0.1.8',
+    version='0.1.9',
     author='Mike Kasper',
     author_email='m_kasper@sbcglobal.net',
     url='http://github.com/mkmer/AIOAladdinConnect',
-    download_url='https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.8.tar.gz',
+    download_url='https://github.com/mkmer/AIOAladdinConnect/archive/refs/tags/0.1.9.tar.gz',
     packages=['AIOAladdinConnect'],
     scripts=[],
     description='Python Async API for controlling Genie garage doors connected to Aladdin Connect devices',
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```


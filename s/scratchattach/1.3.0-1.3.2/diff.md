# Comparing `tmp/scratchattach-1.3.0.tar.gz` & `tmp/scratchattach-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.3.0.tar", last modified: Mon Jul 31 12:16:01 2023, max compression
+gzip compressed data, was "scratchattach-1.3.2.tar", last modified: Mon Aug  7 23:20:21 2023, max compression
```

## Comparing `scratchattach-1.3.0.tar` & `scratchattach-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:16:01.001222 scratchattach-1.3.0/
--rw-rw-rw-   0        0        0    22121 2023-07-31 12:16:01.000222 scratchattach-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 12:16:00.984507 scratchattach-1.3.0/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    15465 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18518 2023-07-31 12:07:52.000000 scratchattach-1.3.0/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25440 2023-07-31 12:15:07.000000 scratchattach-1.3.0/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:16:00.999222 scratchattach-1.3.0/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22121 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:16:01.001222 scratchattach-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-07-31 12:15:22.000000 scratchattach-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:20:21.237343 scratchattach-1.3.2/
+-rw-rw-rw-   0        0        0    22121 2023-08-07 23:20:21.237343 scratchattach-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 23:20:21.223323 scratchattach-1.3.2/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    15474 2023-08-07 23:19:49.000000 scratchattach-1.3.2/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18436 2023-07-31 14:27:54.000000 scratchattach-1.3.2/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-07-30 15:45:18.000000 scratchattach-1.3.2/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25440 2023-07-31 12:15:07.000000 scratchattach-1.3.2/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-08-07 23:20:21.236332 scratchattach-1.3.2/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22121 2023-08-07 23:20:21.000000 scratchattach-1.3.2/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-08-07 23:20:21.000000 scratchattach-1.3.2/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 23:20:21.000000 scratchattach-1.3.2/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-08-07 23:20:21.000000 scratchattach-1.3.2/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 23:20:21.000000 scratchattach-1.3.2/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 23:20:21.237343 scratchattach-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-08-07 23:20:06.000000 scratchattach-1.3.2/setup.py
```

### Comparing `scratchattach-1.3.0/PKG-INFO` & `scratchattach-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.3.0
+Version: 1.3.2
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.3.0/README.md` & `scratchattach-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_cloud.py` & `scratchattach-1.3.2/scratchattach/_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             try:
                 self.websocket = websocket.WebSocket()
                 self.websocket.connect(
                     "wss://clouddata.scratch.mit.edu",
                     cookie="scratchsessionsid=" + self._session_id + ";",
                     origin="https://scratch.mit.edu",
                     enable_multithread=True,
-                    timeout=timeout
+                    timeout=self._ws_timeout
                 )
             except Exception:
                 raise(_exceptions.ConnectionError)
         self._connect_timestamp = time.time()
 
     def set_var(self, variable, value):
         variable = variable.replace("☁ ", "")
```

### Comparing `scratchattach-1.3.0/scratchattach/_cloud_requests.py` & `scratchattach-1.3.2/scratchattach/_cloud_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,16 +376,15 @@
                         self.request_parts[request_id].append(raw_request[1:])
                         continue
 
                     if request_id in self.responded_request_ids:
                         continue
                     else:
                         self.responded_request_ids.insert(0, request_id)
-                        self.responded_request_ids = self.responded_request_ids[:
-                                                                                15]
+                        self.responded_request_ids = self.responded_request_ids[:15]
                 except Exception:
                     self.last_timestamp = event.timestamp
                     continue
 
                 self.last_requester = event.user
                 self.last_timestamp = event.timestamp
```

### Comparing `scratchattach-1.3.0/scratchattach/_encoder.py` & `scratchattach-1.3.2/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_exceptions.py` & `scratchattach-1.3.2/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_forum.py` & `scratchattach-1.3.2/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_project.py` & `scratchattach-1.3.2/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_session.py` & `scratchattach-1.3.2/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_studio.py` & `scratchattach-1.3.2/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach/_user.py` & `scratchattach-1.3.2/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.3.0/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.3.2/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.3.0
+Version: 1.3.2
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.3.0/setup.py` & `scratchattach-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.3.0'
+VERSION = '1.3.2'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```


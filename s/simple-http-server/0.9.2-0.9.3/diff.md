# Comparing `tmp/simple_http_server-0.9.2.tar.gz` & `tmp/simple_http_server-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple_http_server-0.9.2.tar", last modified: Mon Mar  8 07:28:15 2021, max compression
+gzip compressed data, was "dist/simple_http_server-0.9.3.tar", last modified: Tue Mar  9 07:15:57 2021, max compression
```

## Comparing `simple_http_server-0.9.2.tar` & `simple_http_server-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-08 07:28:15.718195 simple_http_server-0.9.2/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    19540 2021-03-08 07:28:15.718195 simple_http_server-0.9.2/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    15150 2021-02-25 10:49:49.000000 simple_http_server-0.9.2/README.md
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2021-03-08 07:28:15.718195 simple_http_server-0.9.2/setup.cfg
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      821 2021-01-04 08:23:06.000000 simple_http_server-0.9.2/setup.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-08 07:28:15.710195 simple_http_server-0.9.2/simple_http_server/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    20615 2021-03-08 07:24:10.000000 simple_http_server-0.9.2/simple_http_server/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      126 2021-02-24 08:46:39.000000 simple_http_server-0.9.2/simple_http_server/__utils.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     5287 2021-02-22 10:44:08.000000 simple_http_server-0.9.2/simple_http_server/_http_session_local_impl.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    15034 2021-02-24 08:48:19.000000 simple_http_server-0.9.2/simple_http_server/base_http_request_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    27887 2021-02-24 09:37:21.000000 simple_http_server-0.9.2/simple_http_server/http_request_handler.py
--rwxrwxr-x   0 keijack   (1000) keijack   (1000)    11925 2021-03-08 07:02:49.000000 simple_http_server-0.9.2/simple_http_server/http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3242 2021-02-22 10:44:08.000000 simple_http_server-0.9.2/simple_http_server/logger.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     5205 2021-02-24 08:43:15.000000 simple_http_server-0.9.2/simple_http_server/server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    12646 2021-03-08 07:24:45.000000 simple_http_server-0.9.2/simple_http_server/websocket_request_handler.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-08 07:28:15.718195 simple_http_server-0.9.2/simple_http_server.egg-info/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    19540 2021-03-08 07:28:15.000000 simple_http_server-0.9.2/simple_http_server.egg-info/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      525 2021-03-08 07:28:15.000000 simple_http_server-0.9.2/simple_http_server.egg-info/SOURCES.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2021-03-08 07:28:15.000000 simple_http_server-0.9.2/simple_http_server.egg-info/dependency_links.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       19 2021-03-08 07:28:15.000000 simple_http_server-0.9.2/simple_http_server.egg-info/top_level.txt
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-09 07:15:57.079421 simple_http_server-0.9.3/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    19854 2021-03-09 07:15:57.079421 simple_http_server-0.9.3/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    15392 2021-03-09 07:15:07.000000 simple_http_server-0.9.3/README.md
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2021-03-09 07:15:57.079421 simple_http_server-0.9.3/setup.cfg
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      821 2021-01-04 08:23:06.000000 simple_http_server-0.9.3/setup.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-09 07:15:57.079421 simple_http_server-0.9.3/simple_http_server/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    20615 2021-03-09 07:10:25.000000 simple_http_server-0.9.3/simple_http_server/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      126 2021-02-24 08:46:39.000000 simple_http_server-0.9.3/simple_http_server/__utils.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     5287 2021-02-22 10:44:08.000000 simple_http_server-0.9.3/simple_http_server/_http_session_local_impl.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    15034 2021-02-24 08:48:19.000000 simple_http_server-0.9.3/simple_http_server/base_http_request_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    27887 2021-02-24 09:37:21.000000 simple_http_server-0.9.3/simple_http_server/http_request_handler.py
+-rwxrwxr-x   0 keijack   (1000) keijack   (1000)    12134 2021-03-09 03:13:48.000000 simple_http_server-0.9.3/simple_http_server/http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3242 2021-02-22 10:44:08.000000 simple_http_server-0.9.3/simple_http_server/logger.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     5350 2021-03-09 06:09:24.000000 simple_http_server-0.9.3/simple_http_server/server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    12646 2021-03-08 07:24:45.000000 simple_http_server-0.9.3/simple_http_server/websocket_request_handler.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2021-03-09 07:15:57.079421 simple_http_server-0.9.3/simple_http_server.egg-info/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    19854 2021-03-09 07:15:56.000000 simple_http_server-0.9.3/simple_http_server.egg-info/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      525 2021-03-09 07:15:56.000000 simple_http_server-0.9.3/simple_http_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2021-03-09 07:15:56.000000 simple_http_server-0.9.3/simple_http_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       19 2021-03-09 07:15:56.000000 simple_http_server-0.9.3/simple_http_server.egg-info/top_level.txt
```

### Comparing `simple_http_server-0.9.2/PKG-INFO` & `simple_http_server-0.9.3/simple_http_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple_http_server
-Version: 0.9.2
+Name: simple-http-server
+Version: 0.9.3
 Summary: This is a simple http server, use MVC like design.
 Home-page: https://github.com/keijack/python-simple-http-server
 Author: Keijack
 Author-email: keijack.wu@gmail.com
 License: UNKNOWN
 Description: # python-simple-http-server
         
@@ -28,20 +28,28 @@
         * Session support, and even, you can apply your own session implementation.
         * Spring MVC like request mapping.
         * SSL support.
         * Websocket support (from 0.9.0).
         * Easy to use.
         * Free style controller writing.
         
+        ## Dependencies
+        
+        There are no other dependencies needed to run this project. However, if you want to run the unitests in the `tests` folder, you need to install `websocket` via pip:
+        
+        ```shell
+        python3 -m pip install websocket
+        ```
+        
         ## How to use
         
         ### Install
         
         ```shell
-        pip install simple_http_server
+        python3 -m pip install simple_http_server
         ```
         
         ### Write Controllers
         
         ```python
         
         from simple_http_server import request_map
@@ -477,14 +485,15 @@
         
         ```python
         logger.set_level("DEBUG")
         ```
         
         This logger will first save all the log record to a global queue, and then output them in a background thread, so it is very suitable for getting several logger with a same handler, especialy the `TimedRotatingFileHandler` which may slice the log files not quite well in a mutiple thread environment. 
         
+        
         ## Thanks
         
         The code that process websocket comes from the following project: https://github.com/Pithikos/python-websocket-server
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `simple_http_server-0.9.2/README.md` & `simple_http_server-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,28 @@
 * Session support, and even, you can apply your own session implementation.
 * Spring MVC like request mapping.
 * SSL support.
 * Websocket support (from 0.9.0).
 * Easy to use.
 * Free style controller writing.
 
+## Dependencies
+
+There are no other dependencies needed to run this project. However, if you want to run the unitests in the `tests` folder, you need to install `websocket` via pip:
+
+```shell
+python3 -m pip install websocket
+```
+
 ## How to use
 
 ### Install
 
 ```shell
-pip install simple_http_server
+python3 -m pip install simple_http_server
 ```
 
 ### Write Controllers
 
 ```python
 
 from simple_http_server import request_map
@@ -469,10 +477,11 @@
 
 ```python
 logger.set_level("DEBUG")
 ```
 
 This logger will first save all the log record to a global queue, and then output them in a background thread, so it is very suitable for getting several logger with a same handler, especialy the `TimedRotatingFileHandler` which may slice the log files not quite well in a mutiple thread environment. 
 
+
 ## Thanks
 
 The code that process websocket comes from the following project: https://github.com/Pithikos/python-websocket-server
```

### Comparing `simple_http_server-0.9.2/setup.py` & `simple_http_server-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server/__init__.py` & `simple_http_server-0.9.3/simple_http_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import http.cookies
 import inspect
 import time
 from typing import Any, Dict, List, Tuple, Type, Union, Callable
 from simple_http_server.logger import get_logger
 
 name = "simple_http_server"
-version = "0.9.2"
+version = "0.9.3"
 
 _logger = get_logger("simple_http_server.__init__")
 
 
 class Session:
 
     def __init__(self):
```

### Comparing `simple_http_server-0.9.2/simple_http_server/_http_session_local_impl.py` & `simple_http_server-0.9.3/simple_http_server/_http_session_local_impl.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server/base_http_request_handler.py` & `simple_http_server-0.9.3/simple_http_server/base_http_request_handler.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server/http_request_handler.py` & `simple_http_server-0.9.3/simple_http_server/http_request_handler.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server/http_server.py` & `simple_http_server-0.9.3/simple_http_server/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,15 @@
                  ssl_check_hostname: bool = False,
                  keyfile: str = "",
                  certfile: str = "",
                  keypass: str = "",
                  ssl_context: _ssl.SSLContext = None,
                  resources: Dict[str, str] = {}):
         self.host = host
+        self.__ready = False
 
         self.ssl = ssl
         self.server = HTTPServer(self.host, res_conf=resources)
 
         if ssl:
             if ssl_context:
                 ssl_ctx = ssl_context
@@ -295,23 +296,32 @@
                 ssl_ctx.check_hostname = ssl_check_hostname
                 ssl_ctx.load_cert_chain(certfile=certfile, keyfile=keyfile, password=keypass)
             self.server.socket = ssl_ctx.wrap_socket(
                 self.server.socket,
                 server_side=True
             )
 
+    @property
+    def ready(self):
+        return self.__ready
+
     def resources(self, res={}):
         self.server.res_conf = res
 
     def start(self):
         if self.ssl:
             ssl_hint = " with SSL on"
         else:
             ssl_hint = ""
         _logger.info(f"Dispatcher Http Server starts. Listen to port [{self.host[1]}]{ssl_hint}.")
-        self.server.serve_forever()
+        try:
+            self.__ready = True
+            self.server.serve_forever()
+        except:
+            self.__ready = False
+            raise
 
     def shutdown(self):
         # server must shutdown in a separate thread, or it will be deadlocking...WTF!
         t = threading.Thread(target=self.server.shutdown)
         t.daemon = True
         t.start()
```

### Comparing `simple_http_server-0.9.2/simple_http_server/logger.py` & `simple_http_server-0.9.3/simple_http_server/logger.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server/server.py` & `simple_http_server-0.9.3/simple_http_server/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from simple_http_server import request_map
 from simple_http_server import StaticFile
 from simple_http_server.logger import get_logger
 
 
 __logger = get_logger("simple_http_server.server")
 __lock = threading.Lock()
-__server = None
+_server = None
 
 
 def _is_match(string="", regx=r""):
     if not regx:
         return True
     pattern = re.compile(regx)
     match = pattern.match(string)
@@ -82,22 +82,25 @@
     return modules
 
 
 def _import_module(mname):
     try:
         importlib.import_module(mname)
     except:
-        __logger.warn(f"Import moudle [{mname}] error!")
+        __logger.warning(f"Import moudle [{mname}] error!")
 
 
-def scan(base_dir: str = "", regx: str = r"") -> None:
-    ft = inspect.currentframe()
-    fts = inspect.getouterframes(ft)
-    entrance = fts[-1]
-    work_dir = os.path.dirname(inspect.getabsfile(entrance[0]))
+def scan(base_dir: str = "", regx: str = r"", project_dir: str = "") -> None:
+    if project_dir:
+        work_dir = project_dir
+    else:
+        ft = inspect.currentframe()
+        fts = inspect.getouterframes(ft)
+        entrance = fts[-1]
+        work_dir = os.path.dirname(inspect.getabsfile(entrance[0]))
     modules = _load_all_modules(work_dir, base_dir, regx)
 
     for mname in modules:
         __logger.info(f"Import controllers from module: {mname}")
         _import_module(mname)
 
 
@@ -108,52 +111,56 @@
           ssl_check_hostname: bool = False,
           keyfile: str = "",
           certfile: str = "",
           keypass: str = "",
           ssl_context: _ssl.SSLContext = None,
           resources: Dict[str, str] = {}) -> None:
     with __lock:
-        global __server
-        if __server is not None:
-            __server.shutdown()
-        __server = http_server.SimpleDispatcherHttpServer(host=(host, port),
-                                                          ssl=ssl,
-                                                          ssl_protocol=ssl_protocol,
-                                                          ssl_check_hostname=ssl_check_hostname,
-                                                          keyfile=keyfile,
-                                                          certfile=certfile,
-                                                          keypass=keypass,
-                                                          ssl_context=ssl_context,
-                                                          resources=resources)
+        global _server
+        if _server is not None:
+            _server.shutdown()
+        _server = http_server.SimpleDispatcherHttpServer(host=(host, port),
+                                                         ssl=ssl,
+                                                         ssl_protocol=ssl_protocol,
+                                                         ssl_check_hostname=ssl_check_hostname,
+                                                         keyfile=keyfile,
+                                                         certfile=certfile,
+                                                         keypass=keypass,
+                                                         ssl_context=ssl_context,
+                                                         resources=resources)
 
     filters = _get_filters()
     # filter configuration
     for ft in filters:
-        __server.map_filter(ft["url_pattern"], ft["func"])
+        _server.map_filter(ft["url_pattern"], ft["func"])
 
     request_mappings = _get_request_mappings()
     # request mapping
     for ctr in request_mappings:
-        __server.map_request(ctr)
+        _server.map_request(ctr)
 
     ws_handlers = _get_websocket_handlers()
 
     for endpoint, clz in ws_handlers.items():
-        __server.map_websocket_handler(endpoint, clz)
+        _server.map_websocket_handler(endpoint, clz)
 
     # start the server
-    __server.start()
+    _server.start()
+
+
+def is_ready() -> bool:
+    return _server and _server.ready
 
 
 def stop() -> None:
     with __lock:
-        global __server
-        if __server is not None:
+        global _server
+        if _server is not None:
             __logger.info("shutting down server...")
-            __server.shutdown()
-            __server = None
+            _server.shutdown()
+            _server = None
 
 
 @request_map("/favicon.ico")
 def _favicon():
     root = os.path.dirname(os.path.abspath(__file__))
     return StaticFile(f"{root}/favicon.ico", "image/x-icon")
```

### Comparing `simple_http_server-0.9.2/simple_http_server/websocket_request_handler.py` & `simple_http_server-0.9.3/simple_http_server/websocket_request_handler.py`

 * *Files identical despite different names*

### Comparing `simple_http_server-0.9.2/simple_http_server.egg-info/PKG-INFO` & `simple_http_server-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple-http-server
-Version: 0.9.2
+Name: simple_http_server
+Version: 0.9.3
 Summary: This is a simple http server, use MVC like design.
 Home-page: https://github.com/keijack/python-simple-http-server
 Author: Keijack
 Author-email: keijack.wu@gmail.com
 License: UNKNOWN
 Description: # python-simple-http-server
         
@@ -28,20 +28,28 @@
         * Session support, and even, you can apply your own session implementation.
         * Spring MVC like request mapping.
         * SSL support.
         * Websocket support (from 0.9.0).
         * Easy to use.
         * Free style controller writing.
         
+        ## Dependencies
+        
+        There are no other dependencies needed to run this project. However, if you want to run the unitests in the `tests` folder, you need to install `websocket` via pip:
+        
+        ```shell
+        python3 -m pip install websocket
+        ```
+        
         ## How to use
         
         ### Install
         
         ```shell
-        pip install simple_http_server
+        python3 -m pip install simple_http_server
         ```
         
         ### Write Controllers
         
         ```python
         
         from simple_http_server import request_map
@@ -477,14 +485,15 @@
         
         ```python
         logger.set_level("DEBUG")
         ```
         
         This logger will first save all the log record to a global queue, and then output them in a background thread, so it is very suitable for getting several logger with a same handler, especialy the `TimedRotatingFileHandler` which may slice the log files not quite well in a mutiple thread environment. 
         
+        
         ## Thanks
         
         The code that process websocket comes from the following project: https://github.com/Pithikos/python-websocket-server
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `simple_http_server-0.9.2/simple_http_server.egg-info/SOURCES.txt` & `simple_http_server-0.9.3/simple_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*


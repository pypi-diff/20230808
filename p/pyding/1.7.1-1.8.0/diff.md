# Comparing `tmp/pyding-1.7.1.tar.gz` & `tmp/pyding-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyding-1.7.1.tar", last modified: Wed Jun 14 18:05:56 2023, max compression
+gzip compressed data, was "pyding-1.8.0.tar", last modified: Tue Aug  8 20:24:19 2023, max compression
```

## Comparing `pyding-1.7.1.tar` & `pyding-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 18:05:39.000000 pyding-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 18:05:56.412751 pyding-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-14 18:05:39.000000 pyding-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/pyding/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/event_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-14 18:05:39.000000 pyding-1.7.1/pyding/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 18:05:56.412751 pyding-1.7.1/pyding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 18:05:56.000000 pyding-1.7.1/pyding.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 18:05:56.412751 pyding-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-14 18:05:39.000000 pyding-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:24:19.768101 pyding-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 20:24:08.000000 pyding-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-08 20:24:19.768101 pyding-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-08-08 20:24:08.000000 pyding-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:24:19.768101 pyding-1.8.0/pyding/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-08 20:24:08.000000 pyding-1.8.0/pyding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-08-08 20:24:08.000000 pyding-1.8.0/pyding/event_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 20:24:08.000000 pyding-1.8.0/pyding/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-08 20:24:08.000000 pyding-1.8.0/pyding/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:24:19.768101 pyding-1.8.0/pyding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-08 20:24:19.000000 pyding-1.8.0/pyding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-08 20:24:19.000000 pyding-1.8.0/pyding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:24:19.000000 pyding-1.8.0/pyding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 20:24:19.000000 pyding-1.8.0/pyding.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:24:19.768101 pyding-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-08 20:24:08.000000 pyding-1.8.0/setup.py
```

### Comparing `pyding-1.7.1/LICENSE` & `pyding-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyding-1.7.1/PKG-INFO` & `pyding-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyding
-Version: 1.7.1
+Version: 1.8.0
 Summary: Simpĺe but effective event framework
 Home-page: https://github.com/jaobernardi/pyding
 Author: João Lucas Bernardi
 Author-email: joao_bernardi@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -92,14 +92,35 @@
 thread.start()
 
 # Wait for the event to be called
 event_inputs = pyding.wait_for("random_event")
 # event_inputs = {'event': EventCall object, ... any other keyargs here ... }
 ```
 
+<h3 align="center"> Queues </h3>
+
+<p align="center"> Queues are populated from events, useful for multiple entry points approaches with <code>pyding.queue</code></p>
+
+```python
+import pyding
+from threading import Thread
+
+def listener(event):
+    queue = pyding.queue("foo")
+    while True:
+        event = queue.get()
+        # do stuff here...
+
+# Start the listener
+Thread(target=listener, daemon=True).start()
+
+# Call the event
+event = pyding.call("check", cancellable=True)
+```
+
 <h3 align="center"> Cancellable events </h3>
 
 <p align="center"> You can also make events that can be cancelled, using the <code>cancellable</code> keyword for <code>pyding.call</code></p>
 
 > ⚠️ - Cancelling an event which cannot be cancelled will raise `pyding.exceptions.UncancellableEvent`
 
 ```python
@@ -115,14 +136,16 @@
 # Call the event
 event = pyding.call("check", cancellable=True)
 
 event.cancelled
 # will return True
 ```
 
+
+
 <h3 align="center"> Hierarchy </h3>
 
 <p align="center"> Event handlers can have an priority attached to them. If the event is cancelled, it will not execute the next handlers. This behavior can be changed by the <code>blocking</code> keyword for <code>pyding.call</code></p>
 
 ```python
 import pyding
```

### Comparing `pyding-1.7.1/README.md` & `pyding-1.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,35 @@
 thread.start()
 
 # Wait for the event to be called
 event_inputs = pyding.wait_for("random_event")
 # event_inputs = {'event': EventCall object, ... any other keyargs here ... }
 ```
 
+<h3 align="center"> Queues </h3>
+
+<p align="center"> Queues are populated from events, useful for multiple entry points approaches with <code>pyding.queue</code></p>
+
+```python
+import pyding
+from threading import Thread
+
+def listener(event):
+    queue = pyding.queue("foo")
+    while True:
+        event = queue.get()
+        # do stuff here...
+
+# Start the listener
+Thread(target=listener, daemon=True).start()
+
+# Call the event
+event = pyding.call("check", cancellable=True)
+```
+
 <h3 align="center"> Cancellable events </h3>
 
 <p align="center"> You can also make events that can be cancelled, using the <code>cancellable</code> keyword for <code>pyding.call</code></p>
 
 > ⚠️ - Cancelling an event which cannot be cancelled will raise `pyding.exceptions.UncancellableEvent`
 
 ```python
@@ -95,14 +116,16 @@
 # Call the event
 event = pyding.call("check", cancellable=True)
 
 event.cancelled
 # will return True
 ```
 
+
+
 <h3 align="center"> Hierarchy </h3>
 
 <p align="center"> Event handlers can have an priority attached to them. If the event is cancelled, it will not execute the next handlers. This behavior can be changed by the <code>blocking</code> keyword for <code>pyding.call</code></p>
 
 ```python
 import pyding
```

### Comparing `pyding-1.7.1/pyding/event_space.py` & `pyding-1.8.0/pyding/event_space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from .structures import EventHandler, EventCall, WaitingHandler
+from .structures import EventHandler, EventCall, WaitingHandler, QueuedHandler
 
 class EventSpace:
     """
         Manages and holds the event listener/handlers.
     """
     def __init__(self, event_handler_class: EventHandler = None):
         self.event_handler_class = event_handler_class or EventHandler
@@ -43,14 +43,18 @@
                 for handler in handlers:
                     if handler.origin_module == module:
                         handlers.remove(handler)
 
     def unregister_handler(self, handler):
         self.events[handler.event][handler.priority].remove(handler)
 
+    def queue(self, event_name: str, priority: int=0, register_ra: bool=True, function: bool=None, requirement_exceptions: bool=False, is_async: bool=None, **kwargs):
+        handler = QueuedHandler(event_name, priority, self, is_async=is_async, requirement_exceptions=requirement_exceptions, execution_requirements=kwargs)
+        handler.register()
+        return handler.get_queue()
 
     def wait_for(self, event_name: str, priority: int=0, register_ra: bool=True, function: bool=None, requirement_exceptions: bool=False, is_async: bool=None, **kwargs):
         handler = WaitingHandler(event_name, priority, self, is_async=is_async, requirement_exceptions=requirement_exceptions, execution_requirements=kwargs)
         handler.register()
         return handler.wait()
 
     # Define the "on" method
```

### Comparing `pyding-1.7.1/pyding/structures.py` & `pyding-1.8.0/pyding/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #structures.py
 import asyncio
 import inspect
+import queue
+from threading import Thread
 from .exceptions import UncancellableEvent, UnfulfilledRequirement
 
 
 # Wrapper for event handlers
 class EventHandler:
     def __init__(self, function, event: str, priority: int, event_space, additional_kwargs: dict = {}, execution_requirements: dict = {}, requirement_exceptions: bool = False, is_async: bool = None):
         self.function = function
@@ -58,14 +60,25 @@
     
     def wait(self):
         while not self.output:
             continue
         self.unregister()
         return self.output
 
+class QueuedHandler(EventHandler):
+    def __init__(self, *args, **kwargs):
+        self.output = None
+        self.queue = queue.Queue()
+        super().__init__(self.handler, *args, **kwargs)
+    
+    def handler(self, *args, **kwargs):
+        Thread(target=self.queue.put, args=(kwargs,), daemon=True, name='Include event to queue').start()
+    
+    def get_queue(self):
+        return self.queue
 
 
 # Add support for event calls inside objects
 class EventSupport:
     def __init__(self):
         self.register_events()
 
@@ -73,16 +86,14 @@
         for method in self.__dir__():
             method = self.__getattribute__(method)
             if isinstance(method, EventHandler):
                 if method.registered:
                     method.unregister()
                 method.register({"self": self})
 
-
-
 # Define the EventCall class
 class EventCall:
     def __init__(self, event_name, cancellable=False):
         self.__name = event_name
         self.__cancelled = False
         self.__stopped = False
         self.__response = None
```

### Comparing `pyding-1.7.1/pyding.egg-info/PKG-INFO` & `pyding-1.8.0/pyding.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyding
-Version: 1.7.1
+Version: 1.8.0
 Summary: Simpĺe but effective event framework
 Home-page: https://github.com/jaobernardi/pyding
 Author: João Lucas Bernardi
 Author-email: joao_bernardi@outlook.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -92,14 +92,35 @@
 thread.start()
 
 # Wait for the event to be called
 event_inputs = pyding.wait_for("random_event")
 # event_inputs = {'event': EventCall object, ... any other keyargs here ... }
 ```
 
+<h3 align="center"> Queues </h3>
+
+<p align="center"> Queues are populated from events, useful for multiple entry points approaches with <code>pyding.queue</code></p>
+
+```python
+import pyding
+from threading import Thread
+
+def listener(event):
+    queue = pyding.queue("foo")
+    while True:
+        event = queue.get()
+        # do stuff here...
+
+# Start the listener
+Thread(target=listener, daemon=True).start()
+
+# Call the event
+event = pyding.call("check", cancellable=True)
+```
+
 <h3 align="center"> Cancellable events </h3>
 
 <p align="center"> You can also make events that can be cancelled, using the <code>cancellable</code> keyword for <code>pyding.call</code></p>
 
 > ⚠️ - Cancelling an event which cannot be cancelled will raise `pyding.exceptions.UncancellableEvent`
 
 ```python
@@ -115,14 +136,16 @@
 # Call the event
 event = pyding.call("check", cancellable=True)
 
 event.cancelled
 # will return True
 ```
 
+
+
 <h3 align="center"> Hierarchy </h3>
 
 <p align="center"> Event handlers can have an priority attached to them. If the event is cancelled, it will not execute the next handlers. This behavior can be changed by the <code>blocking</code> keyword for <code>pyding.call</code></p>
 
 ```python
 import pyding
```

### Comparing `pyding-1.7.1/setup.py` & `pyding-1.8.0/setup.py`

 * *Files identical despite different names*


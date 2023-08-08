# Comparing `tmp/python-send-logs-to-0.2.1b0.tar.gz` & `tmp/python-send-logs-to-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-send-logs-to-0.2.1b0.tar", last modified: Wed Apr 26 13:47:00 2023, max compression
+gzip compressed data, was "python-send-logs-to-0.3.1.tar", last modified: Tue Aug  8 13:33:03 2023, max compression
```

## Comparing `python-send-logs-to-0.2.1b0.tar` & `python-send-logs-to-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.2.1b0/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3331 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2557 2023-04-26 13:31:01.000000 python-send-logs-to-0.2.1b0/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/log_to/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       27 2023-04-26 13:32:14.000000 python-send-logs-to-0.2.1b0/log_to/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5706 2023-04-18 10:47:06.000000 python-send-logs-to-0.2.1b0/log_to/redis.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3331 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      275 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        7 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.2.1b0/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.3.1/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3329 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2557 2023-08-08 13:10:52.000000 python-send-logs-to-0.3.1/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/log_to/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-08 13:32:36.000000 python-send-logs-to-0.3.1/log_to/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     8012 2023-08-08 13:30:58.000000 python-send-logs-to-0.3.1/log_to/redis.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3329 2023-08-08 13:33:03.000000 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      316 2023-08-08 13:33:03.000000 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-08 13:33:03.000000 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-08-08 13:33:03.000000 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       13 2023-08-08 13:33:03.000000 python-send-logs-to-0.3.1/python_send_logs_to.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.3.1/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-08 13:33:03.362167 python-send-logs-to-0.3.1/tests/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        0 2023-05-15 18:04:14.000000 python-send-logs-to-0.3.1/tests/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1482 2023-08-08 13:31:46.000000 python-send-logs-to-0.3.1/tests/test_handlers.py
```

### Comparing `python-send-logs-to-0.2.1b0/LICENSE` & `python-send-logs-to-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.2.1b0/PKG-INFO` & `python-send-logs-to-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-send-logs-to
-Version: 0.2.1b0
+Version: 0.3.1
 Summary: A Python logging handler that sends logs to Redis; later to be a collection of logging handlers.
 Home-page: https://github.com/armandtvz/python-send-logs-to
 Author: Armandt van Zyl
 Author-email: armandtvz@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `python-send-logs-to-0.2.1b0/README.md` & `python-send-logs-to-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.2.1b0/log_to/redis.py` & `python-send-logs-to-0.3.1/log_to/redis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 import logging
+from logging.handlers import MemoryHandler, BufferingHandler
 from datetime import datetime, timezone, timedelta
 
 from redis import StrictRedis
 
 
 
 
-class RedisLogHandler(logging.Handler):
-    """
-    A logging handler that sends logs to Redis. Uses the Redis list type.
-    Other Redis types may be considered in future.
-
-    An example of a log stored in Redis at a key named
-    "logging:app:2023-01-01+0000":
-
-    .. code-block::
-
-        [2023-01-01 21:12:54,774] app | ERROR | <detail>
-        [2023-01-01 17:12:52,774] app | ERROR | <detail>
-        [2023-01-01 11:12:50,774] app | ERROR | <detail>
-    """
+class RedisLogMixin:
 
     def __init__(
         self,
-        key,
+        key=None,
+        redis_namespace=None,
+        namespace_separator=':',
         host='localhost',
         port=6379,
         password='',
         db=0,
         charset='utf-8',
+        socket_connect_timeout=10,
         cap=100_000,
         attach_date_to_key=True,
         expire_after=timedelta(days=61),
     ):
         """
         :param key:           The Redis key to log to.
         :param host:          Redis instance host. Default is ``localhost``
@@ -55,21 +46,30 @@
                               If the Redis key for a log already exists and has
                               no expire time; the expiry will be set. If the
                               expiry has already been set; the expire time
                               will not be changed. Redis 7 is required for this
                               because the ``NX`` option is used. If Redis 7 or
                               higher is not used no expiry will be set.
         """
-        logging.Handler.__init__(self)
         self.key = key
+        self.namespace_separator = namespace_separator
+        if isinstance(redis_namespace, str):
+            if redis_namespace.endswith(self.namespace_separator):
+                redis_namespace = redis_namespace[:-1]
+
+        if not self.key and not redis_namespace:
+            redis_namespace = 'logging'
+
+        self.redis_namespace = redis_namespace
         self.host = host
         self.port = port
         self.password = password
         self.db = db
         self.charset = charset
+        self.socket_connect_timeout = socket_connect_timeout
         self.cap = cap
         self.attach_date_to_key = attach_date_to_key
         self.redis = self.get_connection()
         self.expire_after = expire_after
         self.formatter = logging.Formatter(
             fmt='[{asctime}] {name} | {levelname} | {message}',
             style='{',
@@ -98,24 +98,33 @@
         redis = StrictRedis(
             host=self.host,
             port=self.port,
             password=self.password,
             db=self.db,
             encoding=self.charset,
             decode_responses=True,
+            socket_connect_timeout=self.socket_connect_timeout,
         )
         return redis
 
 
-    def get_key(self):
+    def get_key(self, record):
         key = self.key
+        if not key:
+            key = record.name
+
+        if self.redis_namespace:
+            # For example: "namespace:mykey"
+            key = f'{self.redis_namespace}{self.namespace_separator}{key}'
+
         if self.attach_date_to_key:
+            # For example: "namespace:mykey:2023-08-08+0000"
             now = datetime.now(tz=timezone.utc)
             today = now.strftime('%Y-%m-%d%z')
-            key = f'{key}:{today}'
+            key = f'{key}{self.namespace_separator}{today}'
         return key
 
 
     @property
     def redis_version(self):
         """
         Returns the major version of the Redis instance
@@ -132,32 +141,107 @@
             # cannot be cast to an integer;
             # rather play it safe and set
             # the version to 0
             version = 0
         return version
 
 
-    def emit(self, record):
+    def _emit(self, record, **kwargs):
+        pipe = kwargs.get('pipe', None)
+        trim_list = True
+        if not pipe:
+            pipe = self.redis.pipeline()
+        else:
+            trim_list = False
+
+        key = self.get_key(record)
+        record = self.format(record)
+        pipe.lpush(key, record)
+        if self.cap and trim_list:
+            pipe.ltrim(key, 0, self.cap)
+
+        if (
+            self.redis_version >= 7
+            and self.expire_after
+            and trim_list
+        ):
+            pipe.expire(key, self.expire_after, nx=True)
+        # If expire_after set and Redis version lower than 7
+        # redis.exceptions.ResponseError will be thrown when
+        # calling pipe.execute(). Therefore, it's important
+        # to check the Redis version before running execute()
+        if trim_list:
+            pipe.execute()
+
+
+
+
+class RedisLogHandler(RedisLogMixin, logging.Handler):
+    """
+    A logging handler that sends logs to Redis. Uses the Redis list type.
+    Other Redis types may be considered in future.
+
+    An example of a log stored in Redis at a key named
+    "logging:app:2023-01-01+0000":
+
+    .. code-block::
+
+        [2023-01-01 21:12:54,774] app | ERROR | <detail>
+        [2023-01-01 17:12:52,774] app | ERROR | <detail>
+        [2023-01-01 11:12:50,774] app | ERROR | <detail>
+    """
+
+    def __init__(self, *args, **kwargs):
+        logging.Handler.__init__(self)
+        super().__init__(*args, **kwargs)
+
+
+    def emit(self, record, **kwargs):
         """
         Insert the log record at the head of a Redis list by doing an ``LPUSH``.
         """
         try:
-            key = self.get_key()
-            record = self.format(record)
+            self._emit(record, **kwargs)
+        except Exception:
+            self.handleError(record)
+
+
+
+
+class RedisBufferedLogHandler(RedisLogMixin, BufferingHandler):
+
+    def __init__(
+        self,
+        capacity,
+        *args,
+        **kwargs,
+    ):
+        self.flushLevel = None
+        try:
+            self.flushLevel = kwargs.pop('flushLevel')
+        except KeyError:
+            self.flushLevel = logging.ERROR
+        BufferingHandler.__init__(self, capacity)
+        super().__init__(*args, **kwargs)
+
+
+    def shouldFlush(self, record):
+        """
+        Check for buffer full or a record at the flushLevel or higher.
+        """
+        return (len(self.buffer) >= self.capacity) or \
+                (record.levelno >= self.flushLevel)
+
+
+    def flush(self):
+        try:
+            if not self.buffer:
+                return
             pipe = self.redis.pipeline()
-            pipe.lpush(key, record)
-            if self.cap:
-                pipe.ltrim(key, 0, self.cap)
-
-            if (
-                self.redis_version >= 7
-                and self.expire_after
-            ):
-                pipe.expire(key, self.expire_after, nx=True)
-            # If expire_after set and Redis version lower than 7
-            # redis.exceptions.ResponseError will be thrown when
-            # calling pipe.execute(). Therefore, it's important
-            # to check the Redis version before running execute()
+
+            for record in self.buffer:
+                self._emit(record, pipe=pipe)
             pipe.execute()
+            self.buffer.clear()
 
         except Exception:
             self.handleError(record)
```

### Comparing `python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/PKG-INFO` & `python-send-logs-to-0.3.1/python_send_logs_to.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-send-logs-to
-Version: 0.2.1b0
+Version: 0.3.1
 Summary: A Python logging handler that sends logs to Redis; later to be a collection of logging handlers.
 Home-page: https://github.com/armandtvz/python-send-logs-to
 Author: Armandt van Zyl
 Author-email: armandtvz@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `python-send-logs-to-0.2.1b0/setup.py` & `python-send-logs-to-0.3.1/setup.py`

 * *Files identical despite different names*


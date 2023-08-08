# Comparing `tmp/usepy_plugin_redis-0.1.0.tar.gz` & `tmp/usepy_plugin_redis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy_plugin_redis-0.1.0.tar", max compression
+gzip compressed data, was "usepy_plugin_redis-0.1.1.tar", max compression
```

## Comparing `usepy_plugin_redis-0.1.0.tar` & `usepy_plugin_redis-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       20 2023-08-08 07:40:12.070907 usepy_plugin_redis-0.1.0/README.md
--rw-r--r--   0        0        0      497 2023-08-08 07:40:12.070907 usepy_plugin_redis-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3834 2023-08-08 07:40:12.070907 usepy_plugin_redis-0.1.0/src/usepy_plugin_redis/__init__.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 usepy_plugin_redis-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-08-08 14:31:21.370830 usepy_plugin_redis-0.1.1/README.md
+-rw-r--r--   0        0        0      497 2023-08-08 14:31:21.370830 usepy_plugin_redis-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4215 2023-08-08 14:31:21.374830 usepy_plugin_redis-0.1.1/src/usepy_plugin_redis/__init__.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 usepy_plugin_redis-0.1.1/PKG-INFO
```

### Comparing `usepy_plugin_redis-0.1.0/src/usepy_plugin_redis/__init__.py` & `usepy_plugin_redis-0.1.1/src/usepy_plugin_redis/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import threading
 
 import redis
 import time
 from threading import local
 
 MAX_SEND_ATTEMPTS = 6  # 最大发送重试次数
 MAX_CONNECTION_ATTEMPTS = float('inf')  # 最大连接重试次数
@@ -61,16 +62,27 @@
             try:
                 _connection.close()
             except Exception as exc:
                 logger.exception(f"RedisStore connection close error<{exc}>")
             del self.state.connection
 
 
-class RedisStreamMixin:
-    connection: redis.Redis
+class RedisStreamStore(RedisStore):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__shutdown = False
+        self.__shutdown_event = threading.Event()
+
+    def __del__(self):
+        self.shutdown()
+
+    def shutdown(self):
+        self.__shutdown = True
+        self.__shutdown_event.set()
 
     def _create_group(self, stream, group):
         try:
             self.connection.xgroup_create(stream, group, id='0', mkstream=True)
         except redis.exceptions.ResponseError as e:
             if "already exists" not in str(e):
                 raise e
@@ -86,16 +98,20 @@
                 del self.connection
                 attempts += 1
                 if attempts > MAX_SEND_ATTEMPTS:
                     raise exc
 
     def start_consuming(self, stream, group, consumer, callback, prefetch=1, **kwargs):
         """开始消费"""
+        self.__shutdown = False
+        self.__shutdown_event.clear()
         self._create_group(stream, group)
-        while True:
+        while not self.__shutdown:
+            if self.__shutdown:
+                break
             try:
                 messages = self.connection.xreadgroup(group, consumer, {stream: '>'}, count=prefetch, **kwargs)
                 for message in messages:
                     _, msg = message
                     callback(msg)
             except redis.ConnectionError:
                 logger.warning("RedisStore consume connection error, reconnecting...")
@@ -103,13 +119,9 @@
                 time.sleep(1)
             except Exception as e:
                 logger.exception(f"RedisStore consume error<{e}>, reconnecting...")
                 del self.connection
                 time.sleep(1)
 
 
-class RedisStreamStore(RedisStore, RedisStreamMixin):
-    pass
-
-
 useRedis = RedisStore
 useRedisStreamStore = RedisStreamStore
```


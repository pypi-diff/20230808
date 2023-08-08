# Comparing `tmp/agora_redis_client-1.1.40-py2.py3-none-any.whl.zip` & `tmp/agora_redis_client-1.1.41-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2642 bytes, number of entries: 7
+Zip file size: 2667 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       31 b- defN 23-Jun-14 11:28 agora_redis_client/__init__.py
--rw-r--r--  2.0 fat     1325 b- defN 23-Jun-14 11:28 agora_redis_client/redis_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Aug-08 16:54 agora_redis_client/version.py
--rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.40.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.40.dist-info/WHEEL
--rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.40.dist-info/METADATA
--rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.40.dist-info/RECORD
-7 files, 3035 bytes uncompressed, 1562 bytes compressed:  48.5%
+-rw-r--r--  2.0 fat     1451 b- defN 23-Aug-08 17:42 agora_redis_client/redis_client.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Aug-08 17:47 agora_redis_client/version.py
+-rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.41.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.41.dist-info/WHEEL
+-rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.41.dist-info/METADATA
+-rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.41.dist-info/RECORD
+7 files, 3161 bytes uncompressed, 1587 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: agora_redis_client/redis_client.py
 Comment: 
 
 Filename: agora_redis_client/version.py
 Comment: 
 
-Filename: agora_redis_client-1.1.40.dist-info/LICENSE
+Filename: agora_redis_client-1.1.41.dist-info/LICENSE
 Comment: 
 
-Filename: agora_redis_client-1.1.40.dist-info/WHEEL
+Filename: agora_redis_client-1.1.41.dist-info/WHEEL
 Comment: 
 
-Filename: agora_redis_client-1.1.40.dist-info/METADATA
+Filename: agora_redis_client-1.1.41.dist-info/METADATA
 Comment: 
 
-Filename: agora_redis_client-1.1.40.dist-info/RECORD
+Filename: agora_redis_client-1.1.41.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_redis_client/redis_client.py

```diff
@@ -9,30 +9,33 @@
     """
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls, *args, **kwargs)
         return cls._instance
 
     def __init__(self): 
-        self.configure()
-        super().__init__(host=self.server, port=self.port, decode_responses=True, socket_keepalive=True)        
+        logger.info("redis_client connecting")
+        self.configure()                
+        super().__init__(host=self.server, port=self.port, decode_responses=True, socket_keepalive=True)                
+        if self.ping():
+            logger.info("redis_client connected")
 
     def configure(self):
         self.server = config["AEA2:RedisClient:Server"]
         if self.server == "":
             self.server = "localhost"
 
         self.port = config["AEA2:RedisClient:Port"]
         if self.port == "":
-            self.port = "6379"
-
-        logger.info("AEA2:RedisClient:")
+            self.port = "6379"            
         logger.info(f"--- Server: {self.server}")
         logger.info(f"--- Port: {self.port}")        
       
+
+      
     def is_connected(self):
         try:             
             if self.ping():                
                 return True
         except Exception as e:
             logger.error(
                 f"Failed to connect to {self.server}:{self.port} :{str(e)}")
```

## agora_redis_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.40'
+__version__ = '1.1.41'
```

## Comparing `agora_redis_client-1.1.40.dist-info/METADATA` & `agora_redis_client-1.1.41.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: agora_redis_client
-Version: 1.1.40
+Version: 1.1.41
 Summary: Redis Client for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.40
-Requires-Dist: agora_config == 1.1.40
+Requires-Dist: agora_logging == 1.1.41
+Requires-Dist: agora_config == 1.1.41
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_redisclient
 
 This package is the Redis Client for the Agora Edge Apps SDK (Python) developed by SLB.
```


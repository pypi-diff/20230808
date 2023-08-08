# Comparing `tmp/shareddata-3.0.3.tar.gz` & `tmp/shareddata-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-3.0.3.tar", last modified: Fri Aug  4 08:02:06 2023, max compression
+gzip compressed data, was "shareddata-3.1.0.tar", last modified: Tue Aug  8 20:56:09 2023, max compression
```

## Comparing `shareddata-3.0.3.tar` & `shareddata-3.1.0.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-04 08:02:06.292769 shareddata-3.0.3/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-3.0.3/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-04 08:02:06.292769 shareddata-3.0.3/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-3.0.3/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-3.0.3/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-04 08:02:06.292769 shareddata-3.0.3/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-04 08:02:06.288769 shareddata-3.0.3/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-04 08:02:06.292769 shareddata-3.0.3/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14303 2023-08-04 07:58:10.000000 shareddata-3.0.3/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 11:10:47.000000 shareddata-3.0.3/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1282 2023-08-04 07:58:18.000000 shareddata-3.0.3/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-03 11:10:47.000000 shareddata-3.0.3/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8295 2023-08-03 12:53:26.000000 shareddata-3.0.3/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7485 2023-08-03 11:10:47.000000 shareddata-3.0.3/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9378 2023-08-04 00:31:28.000000 shareddata-3.0.3/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30809 2023-08-04 07:33:48.000000 shareddata-3.0.3/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-02 13:49:16.000000 shareddata-3.0.3/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 11:10:47.000000 shareddata-3.0.3/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-3.0.3/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-3.0.3/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-3.0.3/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-04 08:02:06.292769 shareddata-3.0.3/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-04 08:02:06.000000 shareddata-3.0.3/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      748 2023-08-04 08:02:06.000000 shareddata-3.0.3/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-04 08:02:06.000000 shareddata-3.0.3/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-04 08:02:06.000000 shareddata-3.0.3/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-04 08:02:06.000000 shareddata-3.0.3/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 20:56:09.136958 shareddata-3.1.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-3.1.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-08 20:56:09.136958 shareddata-3.1.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-3.1.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-3.1.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-08 20:56:09.136958 shareddata-3.1.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 20:56:09.132958 shareddata-3.1.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 20:56:09.136958 shareddata-3.1.0/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14236 2023-08-08 19:27:22.000000 shareddata-3.1.0/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-3.1.0/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10577 2023-08-03 11:10:47.000000 shareddata-3.1.0/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1722 2023-08-08 18:16:28.000000 shareddata-3.1.0/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-3.1.0/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-3.1.0/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-03 11:10:47.000000 shareddata-3.1.0/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8293 2023-08-07 18:30:48.000000 shareddata-3.1.0/src/SharedData/RealTime.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 20:56:09.136958 shareddata-3.1.0/src/SharedData/Routines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1340 2023-08-08 20:52:14.000000 shareddata-3.1.0/src/SharedData/Routines/Orchestrator.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1406 2023-08-08 20:43:38.000000 shareddata-3.1.0/src/SharedData/Routines/ReadLogs.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-08-08 18:08:08.000000 shareddata-3.1.0/src/SharedData/Routines/Scheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      663 2023-08-08 18:31:08.000000 shareddata-3.1.0/src/SharedData/Routines/SendCommand.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      909 2023-08-08 20:53:25.000000 shareddata-3.1.0/src/SharedData/Routines/Server.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8798 2023-08-08 20:39:38.000000 shareddata-3.1.0/src/SharedData/Routines/Worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10872 2023-08-08 20:19:21.000000 shareddata-3.1.0/src/SharedData/Routines/WorkerLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 18:45:04.000000 shareddata-3.1.0/src/SharedData/Routines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7070 2023-08-08 20:31:21.000000 shareddata-3.1.0/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9451 2023-08-07 14:54:31.000000 shareddata-3.1.0/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30765 2023-08-07 17:12:00.000000 shareddata-3.1.0/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8711 2023-08-07 17:22:37.000000 shareddata-3.1.0/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18088 2023-08-07 17:12:49.000000 shareddata-3.1.0/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13186 2023-08-03 11:10:47.000000 shareddata-3.1.0/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-3.1.0/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-3.1.0/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-3.1.0/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-08 20:56:09.136958 shareddata-3.1.0/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-08 20:56:09.000000 shareddata-3.1.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1001 2023-08-08 20:56:09.000000 shareddata-3.1.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-08 20:56:09.000000 shareddata-3.1.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-08 20:56:09.000000 shareddata-3.1.0/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-08 20:56:09.000000 shareddata-3.1.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-3.0.3/LICENSE` & `shareddata-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/PKG-INFO` & `shareddata-3.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 3.0.3
+Version: 3.1.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-3.0.3/README.md` & `shareddata-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/setup.cfg` & `shareddata-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 3.0.3
+version = 3.1.0
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-3.0.3/src/SharedData/AWSKinesis.py` & `shareddata-3.1.0/src/SharedData/AWSKinesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,16 +274,15 @@
 class KinesisStreamConsumer():
     def __init__(self,stream_name):
         self.stream_name = stream_name
         self.stream_buffer = []
         self.last_sequence_number = None
         self.get_stream()
 
-    def get_stream(self):
-        print('Initializing stream...')
+    def get_stream(self):        
         session = boto3.Session()
         if 'KINESIS_ENDPOINT_URL' in os.environ:
             self.client = session.client('kinesis',endpoint_url=os.environ['KINESIS_ENDPOINT_URL'])
         else:
             self.client = session.client('kinesis')
         
         try:
@@ -316,16 +315,15 @@
                         ShardId=shardid,
                         ShardIteratorType='AFTER_SEQUENCE_NUMBER',
                         StartingSequenceNumber=self.last_sequence_number
                         )
                 self.stream['Shards'][i]['ShardIterator'] = shard_iterator['ShardIterator']
                 
         if self.stream['StreamStatus'] != 'ACTIVE':
-            raise Exception('Stream status %s' % (self.stream['StreamStatus']))
-        print('Initializing stream DONE!')
+            raise Exception('Stream status %s' % (self.stream['StreamStatus']))        
                 
     def consume(self):
         success=False
 
         for i in range(len(self.stream['Shards'])):
             try:
                 response = self.client.get_records(\
```

### Comparing `shareddata-3.0.3/src/SharedData/AWSS3.py` & `shareddata-3.1.0/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/DataFrame.py` & `shareddata-3.1.0/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/Defaults.py` & `shareddata-3.1.0/src/SharedData/Defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,9 +34,24 @@
 
 if not 'LOG_LEVEL' in os.environ:    
     os.environ['LOG_LEVEL']='INFO'
 
 if not 'SAVE_LOCAL' in os.environ:    
     os.environ['SAVE_LOCAL']='True'
 
+if not 'GIT_PROTOCOL' in os.environ:
+    os.environ['GIT_PROTOCOL'] = 'https'
+
+if not 'GIT_SERVER' in os.environ:
+    os.environ['GIT_SERVER']='github.com'
+
+if not 'SOURCE_FOLDER' in os.environ:
+    os.environ['SOURCE_FOLDER'] = os.environ['USERPROFILE']+'/src/'
+
+if not 'SLEEP_TIME' in os.environ:
+    os.environ['SLEEP_TIME'] = '2'
+
+if not 'WORKERPOOL_STREAM' in os.environ:
+    os.environ['WORKERPOOL_STREAM'] = 'shareddata-workerpool'
+
 
 loaded=True
```

### Comparing `shareddata-3.0.3/src/SharedData/Logger.py` & `shareddata-3.1.0/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/LoggerConsumerProcess.py` & `shareddata-3.1.0/src/SharedData/Routines/ReadLogs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import time
 import numpy as np
 
 
 from SharedData.SharedData import SharedData
-shdata = SharedData(__file__,user='worker')
+shdata = SharedData('SharedData/Routines/ReadLogs',user='worker')
 from SharedData.Logger import Logger
 from SharedData.AWSKinesis import KinesisLogStreamConsumer
 
 SLEEP_TIME = 2
 
 def run():
-    Logger.log.info('Starting SharedDataLogsConsumer process')
     consumer = KinesisLogStreamConsumer(user='worker')
-
+    lastheartbeat = time.time()
     try:
         consumer.readLogs()
         if consumer.connect():
-            Logger.log.info('SharedDataLogsConsumer process STARTED!')
+            Logger.log.info('Logger reader process STARTED!')
     except:
         pass
 
     while True:
         success = False
         try:
-            success = consumer.consume()
+            success = consumer.consume()            
+            if (success) & (time.time()-lastheartbeat>=15):
+                lastheartbeat = time.time()
+                Logger.log.debug('#heartbeat#')                
         except:
             pass
 
         if not success:
-            Logger.log.info('SharedDataLogsConsumer process error! Restarting...')
+            Logger.log.info('Logger reader process error! Restarting...')
             try:
                 consumer.readLogs()
                 success = consumer.connect()
             except:
                 pass
             if success:
-                Logger.log.info('SharedDataLogsConsumer process RESTARTED!')
+                Logger.log.info('Logger reader process RESTARTED!')
             else:
-                Logger.log.info('SharedDataLogsConsumer failed RESTARTING!')
+                Logger.log.info('Logger reader failed RESTARTING!')
                 time.sleep(SLEEP_TIME*5)
         else:
             time.sleep(SLEEP_TIME + SLEEP_TIME*np.random.rand() - SLEEP_TIME/2)
 
 if __name__ == "__main__":
     run()
```

### Comparing `shareddata-3.0.3/src/SharedData/Metadata.py` & `shareddata-3.1.0/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/MultiProc.py` & `shareddata-3.1.0/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/RealTime.py` & `shareddata-3.1.0/src/SharedData/RealTime.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,29 +10,27 @@
     clients = {}
     # Create a lock to protect access to the clients Dict
     lock = threading.Lock()    
     server = None
     shdata = None
     accept_clients = None
 
-
     @staticmethod
     def runserver(shdata,host,port):
 
         RealTime.shdata = shdata
 
         RealTime.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         # This line allows the address to be reused
         RealTime.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         # Create the server and start accepting clients in a new thread
         RealTime.accept_clients = threading.Thread(target=RealTime.accept_clients_thread, args=(host, port))
         RealTime.accept_clients.start()
                 
-
     @staticmethod
     def accept_clients_thread(host, port):    
         RealTime.server.bind((host, port))
         RealTime.server.listen()
 
         Logger.log.info(f'Serving on {host}:{port}')
```

### Comparing `shareddata-3.0.3/src/SharedData/SharedData.py` & `shareddata-3.1.0/src/SharedData/SharedData.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,29 +40,28 @@
             'Relationships' : ['date','symbol1','symbol2'],
             'Portfolios' : ['date','portfolio'],
             'Signals' : ['date','portfolio','symbol'],
             'Risk' : ['date','portfolio','symbol'],
             'Positions' : ['date','portfolio','symbol'],
             'Orders' : ['date','portfolio','symbol','clordid'],
             'Trades' : ['date','portfolio','symbol','tradeid']
-        }
+        }        
         
         Logger.connect(self.source,self.user)
 
         if (os.name == 'posix'):
             remove_shm_from_resource_tracker()        
     
         if not self.islogged:
             self.islogged = True
             try:
-                Logger.log.debug('%s@%s CONNECTED!\nSharedData version %s, user %s' %
-                    (os.environ['USERNAME'], os.environ['COMPUTERNAME'],version('SharedData'), self.user))
+                Logger.log.debug('User:%s,SharedData:%s CONNECTED!' %
+                    (self.user, version('SharedData')))
             except:
-                Logger.log.debug('%s:%s CONNECTED!\nSharedData user %s!' %
-                    (os.environ['USERNAME'], os.environ['COMPUTERNAME'],self.user))
+                Logger.log.debug('User:%s CONNECTED!' % (self.user))
             
     ###############################################
     ############# DATA CONTAINERS #################
     ###############################################
 
     ############# TABLE #################
     def table(self,database,period,source,tablename,\
@@ -184,14 +183,8 @@
         shm_names = shm_names.sort_index()
         return shm_names
     
     @staticmethod
     def freeall():
         shm_names = SharedData.list()
         for shm_name in shm_names.index:
-            SharedData.free(shm_name)
-    
-    ###############################################
-    ############# REAL TIME MANAGEMENT ############
-    ###############################################
-    def subscribe(database,source,period):
-        SharedDataRealTime.subscribe(database,source,period)
+            SharedData.free(shm_name)
```

### Comparing `shareddata-3.0.3/src/SharedData/SharedNumpy.py` & `shareddata-3.1.0/src/SharedData/SharedNumpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         obj.table = None
         return obj
 
     def subscribe(self,host,port):
         self.table.subscribe(host, port)
 
     def preallocate(self):
+        # TODO: add a progress bar if memory to be preallocated too high
         arr = super().__getitem__(slice(0, self.size))
         arr['mtime'][:] = np.datetime64('NaT')
     ############################## KEYLESS OPERATIONS ########################################
 
     def insert(self, new_records):
         self.table.acquire()
```

### Comparing `shareddata-3.0.3/src/SharedData/Table.py` & `shareddata-3.1.0/src/SharedData/Table.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from SharedData.SharedNumpy import SharedNumpy
 from SharedData.RealTime import RealTime
 
 if os.name == 'posix':
     from SharedData.Utils  import cpp
 
 class Table:
+    #TODO: create a on disk mode
 
     def __init__(self, shareddata, database, period, source, tablename,\
           records=None,names=None,formats=None,size=None,overwrite=False,user='master'):
         self.shareddata = shareddata
         self.user = user
         self.database = database
         self.period = period        
@@ -132,16 +133,15 @@
                 
     def ismalloc(self):
         path, shm_name = self.get_path()
         [self.shm, ismalloc] = self.shareddata.malloc(shm_name)
         return ismalloc
 
     def create(self, names, formats, size):        
-        path, shm_name = self.get_path()
-        #TODO: WRITE FILE WITH POINTER TO SHARED DATA TO KEEP TRACK OF OPENED MEMORY
+        path, shm_name = self.get_path()        
         check_pkey = True
         npkeys = len(self.keys.pkeycolumns)
         for k in range(npkeys):
             check_pkey = (check_pkey) & (names[k]==self.keys.pkeycolumns[k])
         if not check_pkey:
             raise Exception('First columns must be %s!' % (self.keys.pkeycolumns))
         else:
```

### Comparing `shareddata-3.0.3/src/SharedData/TableIndex.py` & `shareddata-3.1.0/src/SharedData/TableIndex.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import SharedData.TableIndexJit as TableIndexJit
 from SharedData.TableIndexJit import *
 
 
 class TableIndex:
 
+    # TODO: create a symbol index
+    
     def __init__(self,table):
         self.table = table
         self.shareddata = self.table.shareddata
         
         self.initialized = False
 
         # primary key hash table
```

### Comparing `shareddata-3.0.3/src/SharedData/TableIndexJit.py` & `shareddata-3.1.0/src/SharedData/TableIndexJit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from numba import njit
+# TODO: change upsert to allow duplicated keep last
+
 ###################### DATE_SYMBOL ########################
 @njit(cache=True)
 def create_pkey_date_symbol_jit(records,count,pkey,dateiniidx,dateendidx,dateunit,start):
 	n = pkey.size-1
 	for i in range(start,count):
 		intdt = np.int32(np.int64(records['date'][i])/dateunit)
 		if dateiniidx[intdt]==-1:
```

### Comparing `shareddata-3.0.3/src/SharedData/TimeSeries.py` & `shareddata-3.1.0/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/TimeseriesContainer.py` & `shareddata-3.1.0/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/SharedData/Utils.py` & `shareddata-3.1.0/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-3.0.3/src/shareddata.egg-info/PKG-INFO` & `shareddata-3.1.0/src/shareddata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 3.0.3
+Version: 3.1.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-3.0.3/src/shareddata.egg-info/SOURCES.txt` & `shareddata-3.1.0/src/shareddata.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,32 @@
 pyproject.toml
 setup.cfg
 src/SharedData/AWSKinesis.py
 src/SharedData/AWSS3.py
 src/SharedData/DataFrame.py
 src/SharedData/Defaults.py
 src/SharedData/Logger.py
-src/SharedData/LoggerConsumerProcess.py
 src/SharedData/Metadata.py
 src/SharedData/MultiProc.py
 src/SharedData/RealTime.py
 src/SharedData/SharedData.py
 src/SharedData/SharedNumpy.py
 src/SharedData/Table.py
 src/SharedData/TableIndex.py
 src/SharedData/TableIndexJit.py
 src/SharedData/TimeSeries.py
 src/SharedData/TimeseriesContainer.py
 src/SharedData/Utils.py
 src/SharedData/__init__.py
+src/SharedData/Routines/Orchestrator.py
+src/SharedData/Routines/ReadLogs.py
+src/SharedData/Routines/Scheduler.py
+src/SharedData/Routines/SendCommand.py
+src/SharedData/Routines/Server.py
+src/SharedData/Routines/Worker.py
+src/SharedData/Routines/WorkerLib.py
+src/SharedData/Routines/__init__.py
 src/shareddata.egg-info/PKG-INFO
 src/shareddata.egg-info/SOURCES.txt
 src/shareddata.egg-info/dependency_links.txt
 src/shareddata.egg-info/requires.txt
 src/shareddata.egg-info/top_level.txt
```


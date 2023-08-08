# Comparing `tmp/seven2one-4.3.0.tar.gz` & `tmp/seven2one-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-4.3.0.tar", last modified: Mon Aug  7 11:33:04 2023, max compression
+gzip compressed data, was "seven2one-4.3.1.tar", last modified: Tue Aug  8 14:33:23 2023, max compression
```

## Comparing `seven2one-4.3.0.tar` & `seven2one-4.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-08-07 11:26:59.000000 seven2one-4.3.0/LICENSE
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:26:59.000000 seven2one-4.3.0/MANIFEST.in
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-07 11:33:04.803949 seven2one-4.3.0/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2726 2023-08-07 11:26:59.000000 seven2one-4.3.0/README.md
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-08-07 11:33:04.803949 seven2one-4.3.0/setup.cfg
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-08-07 11:26:59.000000 seven2one-4.3.0/setup.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.799949 seven2one-4.3.0/seven2one/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-08-07 11:32:59.000000 seven2one-4.3.0/seven2one/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/authorization.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    11073 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/automation.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    64496 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/core.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/email.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/fileImportService.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/fileimport.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/seven2one/logging_loki/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/const.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/emitter.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/logging_loki/handlers.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/programming.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/schedule.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.803949 seven2one-4.3.0/seven2one/utils/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-08-07 11:32:59.000000 seven2one-4.3.0/seven2one/utils/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_autprog.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_init.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_log.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_meta.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_time.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-08-07 11:26:59.000000 seven2one-4.3.0/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-07 11:33:04.799949 seven2one-4.3.0/seven2one.egg-info/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/requires.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-08-07 11:33:04.000000 seven2one-4.3.0/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:33:23.394714 seven2one-4.3.1/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-08-08 14:22:50.000000 seven2one-4.3.1/LICENSE
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:22:50.000000 seven2one-4.3.1/MANIFEST.in
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-08 14:33:23.394714 seven2one-4.3.1/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2726 2023-08-08 14:22:50.000000 seven2one-4.3.1/README.md
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-08-08 14:33:23.394714 seven2one-4.3.1/setup.cfg
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1388 2023-08-08 14:22:50.000000 seven2one-4.3.1/setup.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:33:23.386714 seven2one-4.3.1/seven2one/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-08-08 14:33:12.000000 seven2one-4.3.1/seven2one/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/authorization.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    12213 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/automation.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    64496 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/core.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/email.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/fileImportService.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/fileimport.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:33:23.390714 seven2one-4.3.1/seven2one/logging_loki/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/logging_loki/const.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/programming.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10052 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/schedule.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61479 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:33:23.394714 seven2one-4.3.1/seven2one/utils/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-08-08 14:33:12.000000 seven2one-4.3.1/seven2one/utils/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35567 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_init.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_log.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_meta.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_time.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6567 2023-08-08 14:22:50.000000 seven2one-4.3.1/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-08-08 14:33:23.390714 seven2one-4.3.1/seven2one.egg-info/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3179 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       97 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/requires.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-08-08 14:33:23.000000 seven2one-4.3.1/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-4.3.0/LICENSE` & `seven2one-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/PKG-INFO` & `seven2one-4.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.3.0
+Version: 4.3.1
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.3.0/README.md` & `seven2one-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/setup.py` & `seven2one-4.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/authorization.py` & `seven2one-4.3.1/seven2one/authorization.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/automation.py` & `seven2one-4.3.1/seven2one/automation.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     def getVersion(self):
         """
         Returns name and version of the responsible micro service
         """
 
         return Utils._getServiceVersion(self, 'automation')
 
+    def _resolve_where(self, where: str):
+        # todo: remove function and use Utils. Therefore remove the 'topLevel' thing! Is it coming from dynO?
+        resolvedFilter = ''
+        if where != None:
+            resolvedFilter = Utils._resolveWhere(self, where)["topLevel"]
+
+        return resolvedFilter
+
     def workflows(self) -> pd.DataFrame:
         """Returns a DataFrame of all Workflows"""
 
         graphQLString = f'''query workflows {{
             workflows {{
                 id
                 name
@@ -41,17 +49,36 @@
         if result == None:
             return
 
         df = pd.json_normalize(result['workflows'])
         return df
 
     def workflowInstances(self, workflowId: str = None, fromTimepoint: str = None, toTimepoint: str = None,
-                          fields: list = None, where: str = None, showTasks=False, skip=0, take=50) -> pd.DataFrame:
-        """Shows Instances of a workflow. If workflowId=None, all Instances of all 
-        workflows will be returned."""
+                          fields: list = None, where: str = None, showTasks=False, skip=0, maxResults=50) -> pd.DataFrame:
+        """Shows Instances of a workflow. If workflowId=None, all Instances of all workflows will be returned.
+
+        Parameters:
+        -----------
+        workflowId : str
+            The id of the workflow.
+        fromTimepoint : str
+            Filter on instances started after this timepoint (format: "%Y-%m-%dT%H:%M:%S.%fZ").
+        toTimepoint : str
+            Filter on instances ended before this timepoint (format: "%Y-%m-%dT%H:%M:%S.%fZ").
+        fields : list
+            A list of all properties to be queried. If None, all properties will be queried.
+        where : str
+            Filter based on query string. Examples: 'state eq COMPLETED', 
+        showTasks : bool
+            If True, the tasks of the workflow instances will be shown.
+        skip : int
+            Offset pagination: skip the first n instances.
+        maxResults : int
+            Offset pagination: take up to the first n instances.
+        """
 
         meta = ['id', 'name', 'businessKey',
                 'version', 'startTime', 'endTime', 'state']
         key = 'workflowInstances'
 
         if workflowId != None:
             _workflowId = f'workflowId: "{workflowId}"'
@@ -87,15 +114,15 @@
                     name
                     value
                     time
                 }}'''
 
         resolvedFilter = ''
         if where != None:
-            resolvedFilter = Utils._resolveWhereString(where)
+            resolvedFilter = self._resolve_where(where)
 
         if showTasks != False:
             _tasks = f'''tasks {{
                             id
                             topic
                             workerId
                             timestamp
@@ -103,15 +130,15 @@
                             retries
                             errorMessage
                         }}'''
         else:
             _tasks = ''
 
         graphQLString = f'''query Instances {{
-            {key}(skip: {skip} take: {take} {_workflowId} {_fromTimepoint} {_toTimepoint} {resolvedFilter}) {{
+            {key}(skip: {skip} take: {maxResults} {_workflowId} {_fromTimepoint} {_toTimepoint} {resolvedFilter}) {{
             items {{
                 {_fields}
                 {_tasks}
                 }}
             }}
         }}
         '''
```

### Comparing `seven2one-4.3.0/seven2one/core.py` & `seven2one-4.3.1/seven2one/core.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/email.py` & `seven2one-4.3.1/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/fileImportService.py` & `seven2one-4.3.1/seven2one/fileImportService.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/fileimport.py` & `seven2one-4.3.1/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/logging_loki/const.py` & `seven2one-4.3.1/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/logging_loki/emitter.py` & `seven2one-4.3.1/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/logging_loki/handlers.py` & `seven2one-4.3.1/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/programming.py` & `seven2one-4.3.1/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/schedule.py` & `seven2one-4.3.1/seven2one/schedule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from uuid import uuid4
 import pandas as pd
 from datetime import datetime, timedelta
 from loguru import logger
 
 from .utils.ut import Utils
 
+
 class Schedule():
-    def __init__(self, accessToken:str, endpoint:str, client:object) -> None:
-              
+    def __init__(self, accessToken: str, endpoint: str, client: object) -> None:
+
         self.raiseException = client.raiseException
         self.defaults = client.defaults
         self.accessToken = accessToken
         self.endpoint = endpoint
         self.proxies = client.proxies
 
     def getVersion(self):
         """
         Returns name and version of the responsible micro service
         """
 
         return Utils._getServiceVersion(self, 'schedule')
 
+    def _resolve_where(self, where: str):
+        # todo: remove function and use Utils. Therefore remove the 'topLevel' thing! Is it coming from dynO?
+        resolvedFilter = ''
+        if where != None:
+            resolvedFilter = f'({Utils._resolveWhere(self, where)["topLevel"]})'
+
+        return resolvedFilter
+
     def schedules(
-        self, 
-        fields:list=None, 
-        where:str=None) -> pd.DataFrame:
+            self,
+            fields: list = None,
+            where: str = None) -> pd.DataFrame:
         """
         Returns schedules in a DataFrame
 
         Parameters:
         -----------
         fields: list | str = None
             A list of all properties to be queried. If None, all properties will be queried.
@@ -45,73 +54,75 @@
         """
 
         key = 'schedules'
 
         if fields != None:
             if type(fields) != list:
                 fields = [fields]
-            _fields = Utils._queryFields(fields, recursive=True)   
+            _fields = Utils._queryFields(fields, recursive=True)
         else:
-            _fields =f'''scheduleId
+            _fields = f'''scheduleId
                 name
                 description
                 workflowId
                 businessKey
                 cron
                 timeZone
                 isActive
                 nextFireTime
                 variables {{
                     key
                     value
-                }}''' 
+                }}'''
 
         resolvedFilter = ''
-        if where != None: 
-            resolvedFilter = f'({Utils._resolveWhereString(where)})'
+        if where != None:
+            resolvedFilter = self._resolve_where(where)
 
         graphQLString = f'''query schedules {{
             {key}{resolvedFilter}  {{
                 {_fields}
             }}
         }}
         '''
 
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         df = pd.json_normalize(result[key])
         return df
 
-    def createSchedule(self, name:str, workflowId:str, businessKey:str, cron:str, 
-        isActive:bool=True, description:str=None, variables:dict=None, timeZone:str=None) -> str:
+    def createSchedule(self, name: str, workflowId: str, businessKey: str, cron: str,
+                       isActive: bool = True, description: str = None, variables: dict = None, timeZone: str = None) -> str:
         """Creates a schedule and returns the schedule Id"""
 
         correlationId = str(uuid4())
-        with logger.contextualize(correlation_id = correlationId):
+        with logger.contextualize(correlation_id=correlationId):
 
             if isActive == True:
                 isActive = 'true'
             else:
                 isActive = 'false'
 
             if description != None:
                 description = description
-            else: 
+            else:
                 description = ''
 
             if timeZone == None:
                 timeZone = ''
 
             if variables != None:
                 _variables = 'variables: [\n'
-                for k,v in variables.items():
+                for k, v in variables.items():
                     _variables += f'{{key: "{k}", value: "{v}"}}\n'
                 _variables += ']'
-            else: _variables = ''
+            else:
+                _variables = ''
 
             graphQLString = f'''mutation createSchedule {{
                 createSchedule(input:{{
                     name: "{name}"
                     workflowId: "{workflowId}"
                     businessKey: "{businessKey}"
                     cron: "{cron}"
@@ -128,30 +139,31 @@
                         message
                     }}
                 }}
             }}'''
 
             result = Utils._executeGraphQL(self, graphQLString, correlationId)
             logger.debug(graphQLString)
-            if result == None: return
+            if result == None:
+                return
 
             key = 'createSchedule'
             if result[key]['errors']:
                 Utils._listGraphQlErrors(result, key)
             else:
                 scheduleId = result[key]['schedule']['scheduleId']
                 logger.info(f"New schedule {scheduleId} created.")
 
             return scheduleId
 
-    def updateSchedule(self, scheduleId, name:str=None, workflowId:str=None, businessKey:str=None, 
-        cron:str=None, isActive:bool=None, description:str=None, variables:dict=None, timeZone:str=None) -> None:
+    def updateSchedule(self, scheduleId, name: str = None, workflowId: str = None, businessKey: str = None,
+                       cron: str = None, isActive: bool = None, description: str = None, variables: dict = None, timeZone: str = None) -> None:
         """
         Updates a schedule. Only arguments that ar not None will overwrite respective fields.
-        
+
         Parameters:
         -----------
         scheduleId : str
             The Id of the schedule that is to be updated.
         name : str
             The name of the schedule.
         workflowId : str
@@ -173,33 +185,40 @@
         --------
         >>> vars = {
                 'var1': 99,
                 'var2': "AnyString"
             }
         >>> client.Scheduler.updateSchedule('112880211090997248', name='test_schedule',
                 isActive=True, variables=vars)
-        
+
         """
 
         correlationId = str(uuid4())
-        with logger.contextualize(correlation_id = correlationId):
+        with logger.contextualize(correlation_id=correlationId):
 
             updateScheduleArgs = ''
 
-            if name != None: updateScheduleArgs += f'name: "{name}"\n'
-            if workflowId != None: updateScheduleArgs += f'workflowId: "{workflowId}"\n'
-            if businessKey != None: updateScheduleArgs += f'businessKey: "{businessKey}"\n'
-            if cron != None: updateScheduleArgs += f'cron: "{cron}"\n'
-            if isActive != None: updateScheduleArgs += f'isActive: {str(isActive).lower()}\n'
-            if description != None: updateScheduleArgs +=  f'description: "{description}"\n'
-            if timeZone != None: updateScheduleArgs +=  f'timeZone: "{timeZone}"\n'
+            if name != None:
+                updateScheduleArgs += f'name: "{name}"\n'
+            if workflowId != None:
+                updateScheduleArgs += f'workflowId: "{workflowId}"\n'
+            if businessKey != None:
+                updateScheduleArgs += f'businessKey: "{businessKey}"\n'
+            if cron != None:
+                updateScheduleArgs += f'cron: "{cron}"\n'
+            if isActive != None:
+                updateScheduleArgs += f'isActive: {str(isActive).lower()}\n'
+            if description != None:
+                updateScheduleArgs += f'description: "{description}"\n'
+            if timeZone != None:
+                updateScheduleArgs += f'timeZone: "{timeZone}"\n'
 
             if variables != None:
                 _variables = 'variables: [\n'
-                for k,v in variables.items():
+                for k, v in variables.items():
                     _variables += f'{{key: "{k}", value: "{v}"}}\n'
                 _variables += ']'
                 updateScheduleArgs += _variables
 
             graphQLString = f'''mutation updateSchedule {{
                 updateSchedule(
                     scheduleId: "{scheduleId}"
@@ -211,64 +230,67 @@
                         message
                     }}
                 }}
             }}'''
 
             result = Utils._executeGraphQL(self, graphQLString, correlationId)
             logger.debug(graphQLString)
-            if result == None: return
+            if result == None:
+                return
 
             key = 'updateSchedule'
             if result[key]['errors']:
                 Utils._listGraphQlErrors(result, key)
             else:
                 logger.info(f"Schedule {scheduleId} updated.")
 
             return
 
-    def deleteSchedule(self, scheduleId:str, force:bool=False):
+    def deleteSchedule(self, scheduleId: str, force: bool = False):
         """Deletes a schedule"""
 
         if force == False:
             confirm = input(f"Press 'y' to delete schedule '{scheduleId}': ")
 
         graphQLString = f'''mutation deleteSchedule {{
             deleteSchedule (scheduleId: "{scheduleId}")
             {{
                 errors {{
                 message
                 }}
             }}
         }}
-        '''      
+        '''
 
-        if force == True: confirm = 'y'
+        if force == True:
+            confirm = 'y'
         if confirm == 'y':
             result = Utils._executeGraphQL(self, graphQLString)
-            if result == None: return
+            if result == None:
+                return
 
             key = 'deleteSchedule'
             if result[key]['errors']:
                 Utils._listGraphQlErrors(result, key)
             else:
                 logger.info(f"Schedule {scheduleId} deleted")
                 return None
 
-    def nextFireTimes(self, workflowId:str, fromTimepoint:str=None, toTimepoint:str=None, count:int=None):
+    def nextFireTimes(self, workflowId: str, fromTimepoint: str = None, toTimepoint: str = None, count: int = None):
         """Show next fire times of a workflow"""
 
         if fromTimepoint == None:
             fromTimepoint = datetime.today().isoformat()
 
         if toTimepoint == None:
             toTimepoint = datetime.today() + timedelta(days=3)
 
         if count == None:
             _count = ''
-        else: 
+        else:
             _count = f'count: {count}'
 
         graphQLString = f'''query nextFireTimes {{
             nextFireTimes (
                 workflowId: "{workflowId}",
                 from: "{fromTimepoint}", 
                 to: "{toTimepoint}",
@@ -276,14 +298,15 @@
                 
                 ) {{
                 scheduleId
                 fireTime
                 }}
             }}
         '''
-        
+
         result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        if result == None:
+            return
 
         df = pd.json_normalize(result['nextFireTimes'])
 
         return df
```

### Comparing `seven2one-4.3.0/seven2one/timeseries.py` & `seven2one-4.3.1/seven2one/timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut.py` & `seven2one-4.3.1/seven2one/utils/ut.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_autprog.py` & `seven2one-4.3.1/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_fileimport.py` & `seven2one-4.3.1/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_init.py` & `seven2one-4.3.1/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_log.py` & `seven2one-4.3.1/seven2one/utils/ut_log.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_meta.py` & `seven2one-4.3.1/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_time.py` & `seven2one-4.3.1/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one/utils/ut_timeseries.py` & `seven2one-4.3.1/seven2one/utils/ut_timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.3.0/seven2one.egg-info/PKG-INFO` & `seven2one-4.3.1/seven2one.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.3.0
+Version: 4.3.1
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.3.0/seven2one.egg-info/SOURCES.txt` & `seven2one-4.3.1/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*


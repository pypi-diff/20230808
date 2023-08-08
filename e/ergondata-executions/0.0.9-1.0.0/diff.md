# Comparing `tmp/ergondata-executions-0.0.9.tar.gz` & `tmp/ergondata-executions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergondata-executions-0.0.9.tar", last modified: Wed Jul 12 19:44:42 2023, max compression
+gzip compressed data, was "ergondata-executions-1.0.0.tar", last modified: Tue Aug  8 19:49:13 2023, max compression
```

## Comparing `ergondata-executions-0.0.9.tar` & `ergondata-executions-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.792914 ergondata-executions-0.0.9/
--rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:44:42.792656 ergondata-executions-0.0.9/PKG-INFO
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.790607 ergondata-executions-0.0.9/ergondata_executions/
--rw-r--r--   0 daniel     (502) staff       (20)       65 2023-03-24 20:47:01.000000 ergondata-executions-0.0.9/ergondata_executions/__init__.py
--rw-r--r--   0 daniel     (502) staff       (20)     7757 2023-07-12 19:43:47.000000 ergondata-executions-0.0.9/ergondata_executions/executions.py
-drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-07-12 19:44:42.792183 ergondata-executions-0.0.9/ergondata_executions.egg-info/
--rw-r--r--   0 daniel     (502) staff       (20)      308 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (502) staff       (20)      295 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (502) staff       (20)        1 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (502) staff       (20)       27 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/requires.txt
--rw-r--r--   0 daniel     (502) staff       (20)       21 2023-07-12 19:44:42.000000 ergondata-executions-0.0.9/ergondata_executions.egg-info/top_level.txt
--rw-r--r--   0 daniel     (502) staff       (20)       38 2023-07-12 19:44:42.793000 ergondata-executions-0.0.9/setup.cfg
--rw-r--r--   0 daniel     (502) staff       (20)      430 2023-07-12 19:44:38.000000 ergondata-executions-0.0.9/setup.py
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-08-08 19:49:13.526315 ergondata-executions-1.0.0/
+-rw-r--r--   0 daniel     (502) staff       (20)      308 2023-08-08 19:49:13.526083 ergondata-executions-1.0.0/PKG-INFO
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-08-08 19:49:13.524253 ergondata-executions-1.0.0/ergondata_executions/
+-rw-r--r--   0 daniel     (502) staff       (20)       65 2023-03-24 20:47:01.000000 ergondata-executions-1.0.0/ergondata_executions/__init__.py
+-rw-r--r--   0 daniel     (502) staff       (20)     9056 2023-08-08 19:46:28.000000 ergondata-executions-1.0.0/ergondata_executions/executions.py
+drwxr-xr-x   0 daniel     (502) staff       (20)        0 2023-08-08 19:49:13.525745 ergondata-executions-1.0.0/ergondata_executions.egg-info/
+-rw-r--r--   0 daniel     (502) staff       (20)      308 2023-08-08 19:49:13.000000 ergondata-executions-1.0.0/ergondata_executions.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (502) staff       (20)      295 2023-08-08 19:49:13.000000 ergondata-executions-1.0.0/ergondata_executions.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (502) staff       (20)        1 2023-08-08 19:49:13.000000 ergondata-executions-1.0.0/ergondata_executions.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       27 2023-08-08 19:49:13.000000 ergondata-executions-1.0.0/ergondata_executions.egg-info/requires.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       21 2023-08-08 19:49:13.000000 ergondata-executions-1.0.0/ergondata_executions.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (502) staff       (20)       38 2023-08-08 19:49:13.526388 ergondata-executions-1.0.0/setup.cfg
+-rw-r--r--   0 daniel     (502) staff       (20)      430 2023-08-08 19:48:41.000000 ergondata-executions-1.0.0/setup.py
```

### Comparing `ergondata-executions-0.0.9/ergondata_executions/executions.py` & `ergondata-executions-1.0.0/ergondata_executions/executions.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     __AUTH_URL = "auth"
     __CREATE_EXECUTION_URL = "executions/create/execution"
     __UPDATE_EXECUTION_URL = "executions/update/execution"
     __CREATE_QUEUE_ITEM_URL = "executions/create/queue-item"
     __UPDATE_QUEUE_ITEM_URL = "executions/update/queue-item"
     __GET_QUEUE_ITEM_URL = "executions/get/queue-item"
     __GET_QUEUE_SIZE_URL = "executions/get/queue-size"
+    __GET_QUEUE_ITEMS_URL = "executions/get/queue-items"
+    __GET_EXECUTIONS_URL = "executions/get/executions"
     __WRITE_LOG_URL = "executions/create/log"
 
     def __init__(self, username: str, password: str, timeout: int = 50) -> None:
 
         self.username = username
         self.password = password
         self.timeout = timeout
@@ -255,8 +257,49 @@
         )
 
         if response.status_code == 200:
             print("Queue item obtained with success")
         else:
             print("Failed to obtain queue item")
 
-        return response.json()
+        return response.json()
+
+    def get_queue_items(self) -> Response:
+
+        print(f"Obtaining queue items")
+        headers = {"Authorization": f"Bearer { self.__auth_token }"}
+        body = {}
+
+        response = requests.get(
+            url=f"{ ExecutionsController.__ROOT_URL }{ ExecutionsController.__GET_QUEUE_ITEMS_URL }",
+            headers=headers,
+            json=body,
+            timeout=self.timeout
+        )
+
+        if response.status_code == 200:
+            print("Queue items obtained with success")
+        else:
+            print("Failed to obtain queue items")
+
+        return response.json()
+
+    def get_executions(self) -> Response:
+
+        print(f"Obtaining executions")
+        headers = {"Authorization": f"Bearer { self.__auth_token }"}
+        body = {}
+
+        response = requests.get(
+            url=f"{ ExecutionsController.__ROOT_URL }{ ExecutionsController.__GET_EXECUTIONS_URL }",
+            headers=headers,
+            json=body,
+            timeout=self.timeout
+        )
+
+        if response.status_code == 200:
+            print("Executions obtained with success")
+        else:
+            print("Failed to obtain executions")
+
+        return response.json()
+
```


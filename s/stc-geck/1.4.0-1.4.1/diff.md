# Comparing `tmp/stc-geck-1.4.0.tar.gz` & `tmp/stc-geck-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.4.0.tar", last modified: Tue Aug  8 07:38:06 2023, max compression
+gzip compressed data, was "stc-geck-1.4.1.tar", last modified: Tue Aug  8 07:48:28 2023, max compression
```

## Comparing `stc-geck-1.4.0.tar` & `stc-geck-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:38:06.800068 stc-geck-1.4.0/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.4.0/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:38:06.799815 stc-geck-1.4.0/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.4.0/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-08 07:27:38.000000 stc-geck-1.4.0/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-08-08 07:37:57.000000 stc-geck-1.4.0/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 07:38:06.800167 stc-geck-1.4.0/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:38:06.797661 stc-geck-1.4.0/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.4.0/stc_geck/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     1464 2023-08-07 18:24:50.000000 stc-geck-1.4.0/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     7261 2023-08-07 19:06:08.000000 stc-geck-1.4.0/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     7268 2023-08-08 07:31:42.000000 stc-geck-1.4.0/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)    10455 2023-08-08 07:37:57.000000 stc-geck-1.4.0/stc_geck/query_processor.py
--rw-r--r--   0 pasha      (501) staff       (20)     3254 2023-08-07 18:22:54.000000 stc-geck-1.4.0/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:38:06.799353 stc-geck-1.4.0/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      369 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-08 07:38:06.000000 stc-geck-1.4.0/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:48:28.383159 stc-geck-1.4.1/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.4.1/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:48:28.382758 stc-geck-1.4.1/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     6985 2023-07-23 19:18:57.000000 stc-geck-1.4.1/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-08-08 07:48:15.000000 stc-geck-1.4.1/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-08-08 07:37:57.000000 stc-geck-1.4.1/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-08 07:48:28.383313 stc-geck-1.4.1/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:48:28.380051 stc-geck-1.4.1/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-19 19:56:31.000000 stc-geck-1.4.1/stc_geck/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1464 2023-08-07 18:24:50.000000 stc-geck-1.4.1/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7261 2023-08-07 19:06:08.000000 stc-geck-1.4.1/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     7405 2023-08-08 07:48:12.000000 stc-geck-1.4.1/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)    10455 2023-08-08 07:37:57.000000 stc-geck-1.4.1/stc_geck/query_processor.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3254 2023-08-07 18:22:54.000000 stc-geck-1.4.1/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-08 07:48:28.381917 stc-geck-1.4.1/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     7330 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      369 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-08-08 07:48:28.000000 stc-geck-1.4.1/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.4.0/PKG-INFO` & `stc-geck-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.4.0
+Version: 1.4.1
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.4.0/README.md` & `stc-geck-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.0/pyproject.toml` & `stc-geck-1.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.4.0"
+version = "1.4.1"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.4.0/stc_geck/advices.py` & `stc-geck-1.4.1/stc_geck/advices.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.0/stc_geck/cli.py` & `stc-geck-1.4.1/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.0/stc_geck/client.py` & `stc-geck-1.4.1/stc_geck/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,47 +101,50 @@
         self.starts.append(self.ipfs_api_client)
         self.ipfs_data_directory = '/' + ipfs_data_directory.strip('/') + '/'
         self.index_names = index_names
         self.grpc_api_endpoint = grpc_api_endpoint
         self.temp_dir = tempfile.TemporaryDirectory()
 
         self.is_embed = not is_endpoint_listening(self.grpc_api_endpoint)
-        server_config = get_config()
-        server_config['api']['grpc_endpoint'] = self.grpc_api_endpoint
-        server_config['data_path'] = self.temp_dir.name
-        server_config['log_path'] = self.temp_dir.name
-        for index_name in self.index_names:
-            query_parser_config = {
-                'default_fields': ['abstract', 'content', 'title']
-            }
-            full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index_name + '/'
-            headers_template = {'range': 'bytes={start}-{end}'}
-            remote_index_config = {'remote': {
-                'method': 'GET',
-                'url_template': f'{full_path}{{file_name}}',
-                'headers_template': headers_template,
-                'cache_config': {'cache_size': 536870912},
-            }}
-            if host_header := await detect_host_header(full_path):
-                headers_template['host'] = host_header
-            server_config['core']['indices'][index_name] = {
-                'query_parser_config': query_parser_config,
-                'config': remote_index_config,
-                'field_triggers': {},
-            }
-        self.summa_embed_server = summa_embed.SummaEmbedServerBin(server_config)
+        self.summa_embed_server = None
+
         self.query_processor = QueryProcessor('light' if self.is_embed else 'full')
         self.summa_client = SummaClient(
             endpoint=self.grpc_api_endpoint,
             max_message_length=2 * 1024 * 1024 * 1024 - 1,
         )
 
     async def start(self):
         if self.is_embed:
             logging.getLogger('info').info({'action': 'launching_embedded'})
+
+            server_config = get_config()
+            server_config['api']['grpc_endpoint'] = self.grpc_api_endpoint
+            server_config['data_path'] = self.temp_dir.name
+            server_config['log_path'] = self.temp_dir.name
+            for index_name in self.index_names:
+                query_parser_config = {
+                    'default_fields': ['abstract', 'content', 'title']
+                }
+                full_path = self.ipfs_http_base_url + self.ipfs_data_directory + index_name + '/'
+                headers_template = {'range': 'bytes={start}-{end}'}
+                remote_index_config = {'remote': {
+                    'method': 'GET',
+                    'url_template': f'{full_path}{{file_name}}',
+                    'headers_template': headers_template,
+                    'cache_config': {'cache_size': 536870912},
+                }}
+                if host_header := await detect_host_header(full_path):
+                    headers_template['host'] = host_header
+                server_config['core']['indices'][index_name] = {
+                    'query_parser_config': query_parser_config,
+                    'config': remote_index_config,
+                    'field_triggers': {},
+                }
+            self.summa_embed_server = summa_embed.SummaEmbedServerBin(server_config)
             await self.summa_embed_server.start()
         await self.summa_client.start()
 
     async def stop(self):
         await self.summa_client.stop()
         if self.summa_embed_server:
             await self.summa_embed_server.stop()
```

### Comparing `stc-geck-1.4.0/stc_geck/query_processor.py` & `stc-geck-1.4.1/stc_geck/query_processor.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.0/stc_geck/utils.py` & `stc-geck-1.4.1/stc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.4.0/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.4.1/stc_geck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.4.0
+Version: 1.4.1
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


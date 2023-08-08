# Comparing `tmp/mini-document-storage-1.0.80.tar.gz` & `tmp/mini-document-storage-1.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini-document-storage-1.0.80.tar", last modified: Mon Aug  7 23:39:16 2023, max compression
+gzip compressed data, was "mini-document-storage-1.0.81.tar", last modified: Tue Aug  8 17:50:48 2023, max compression
```

## Comparing `mini-document-storage-1.0.80.tar` & `mini-document-storage-1.0.81.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-07 23:39:16.942686 mini-document-storage-1.0.80/
--rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.80/LICENSE
--rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.80/MANIFEST.in
--rw-r--r--   0 stevo      (501) staff       (20)      788 2023-08-07 23:39:16.942268 mini-document-storage-1.0.80/PKG-INFO
--rw-r--r--   0 stevo      (501) staff       (20)      264 2023-07-25 23:56:31.000000 mini-document-storage-1.0.80/README.md
--rw-r--r--   0 stevo      (501) staff       (20)     1021 2023-08-07 22:53:46.000000 mini-document-storage-1.0.80/pyproject.toml
--rw-r--r--   0 stevo      (501) staff       (20)       38 2023-08-07 23:39:16.942800 mini-document-storage-1.0.80/setup.cfg
-drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-07 23:39:16.931071 mini-document-storage-1.0.80/src/
-drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-07 23:39:16.931500 mini-document-storage-1.0.80/src/mini_document_storage/
-drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-07 23:39:16.941593 mini-document-storage-1.0.80/src/mini_document_storage/client/
--rw-r--r--   0 stevo      (501) staff       (20)    35376 2023-08-07 22:53:36.000000 mini-document-storage-1.0.80/src/mini_document_storage/client/MDSClient.py
--rw-r--r--   0 stevo      (501) staff       (20)     5239 2023-08-07 16:53:54.000000 mini-document-storage-1.0.80/src/mini_document_storage/client/MDSDocument.py
--rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.80/src/mini_document_storage/client/__init__.py
-drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-07 23:39:16.938383 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/
--rw-r--r--   0 stevo      (501) staff       (20)      788 2023-08-07 23:39:16.000000 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/PKG-INFO
--rw-r--r--   0 stevo      (501) staff       (20)      427 2023-08-07 23:39:16.000000 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/SOURCES.txt
--rw-r--r--   0 stevo      (501) staff       (20)        1 2023-08-07 23:39:16.000000 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/dependency_links.txt
--rw-r--r--   0 stevo      (501) staff       (20)        8 2023-08-07 23:39:16.000000 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/requires.txt
--rw-r--r--   0 stevo      (501) staff       (20)       22 2023-08-07 23:39:16.000000 mini-document-storage-1.0.80/src/mini_document_storage.egg-info/top_level.txt
+drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-08 17:50:48.590418 mini-document-storage-1.0.81/
+-rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.81/LICENSE
+-rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.81/MANIFEST.in
+-rw-r--r--   0 stevo      (501) staff       (20)      788 2023-08-08 17:50:48.589653 mini-document-storage-1.0.81/PKG-INFO
+-rw-r--r--   0 stevo      (501) staff       (20)      264 2023-07-25 23:56:31.000000 mini-document-storage-1.0.81/README.md
+-rw-r--r--   0 stevo      (501) staff       (20)     1021 2023-08-08 17:42:59.000000 mini-document-storage-1.0.81/pyproject.toml
+-rw-r--r--   0 stevo      (501) staff       (20)       38 2023-08-08 17:50:48.590539 mini-document-storage-1.0.81/setup.cfg
+drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-08 17:50:48.578861 mini-document-storage-1.0.81/src/
+drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-08 17:50:48.579357 mini-document-storage-1.0.81/src/mini_document_storage/
+drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-08 17:50:48.588626 mini-document-storage-1.0.81/src/mini_document_storage/client/
+-rw-r--r--   0 stevo      (501) staff       (20)    35740 2023-08-08 17:42:53.000000 mini-document-storage-1.0.81/src/mini_document_storage/client/MDSClient.py
+-rw-r--r--   0 stevo      (501) staff       (20)     5239 2023-08-08 17:29:22.000000 mini-document-storage-1.0.81/src/mini_document_storage/client/MDSDocument.py
+-rw-r--r--   0 stevo      (501) staff       (20)        0 2023-07-25 23:56:31.000000 mini-document-storage-1.0.81/src/mini_document_storage/client/__init__.py
+drwxr-xr-x   0 stevo      (501) staff       (20)        0 2023-08-08 17:50:48.585687 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/
+-rw-r--r--   0 stevo      (501) staff       (20)      788 2023-08-08 17:50:48.000000 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/PKG-INFO
+-rw-r--r--   0 stevo      (501) staff       (20)      427 2023-08-08 17:50:48.000000 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 stevo      (501) staff       (20)        1 2023-08-08 17:50:48.000000 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 stevo      (501) staff       (20)        8 2023-08-08 17:50:48.000000 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/requires.txt
+-rw-r--r--   0 stevo      (501) staff       (20)       22 2023-08-08 17:50:48.000000 mini-document-storage-1.0.81/src/mini_document_storage.egg-info/top_level.txt
```

### Comparing `mini-document-storage-1.0.80/PKG-INFO` & `mini-document-storage-1.0.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-document-storage
-Version: 1.0.80
+Version: 1.0.81
 Summary: Fast, inexpensive document storage backed by a standard database connector.
 Author-email: Stevo Brock <StevoGTA@aol.com>
 Project-URL: Homepage, https://github.com/StevoGTA/Mini-Document-Storage
 Keywords: document storage
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mini-document-storage-1.0.80/pyproject.toml` & `mini-document-storage-1.0.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mini-document-storage"
-version = "1.0.80"
+version = "1.0.81"
 description = "Fast, inexpensive document storage backed by a standard database connector."
 readme = "README.md"
 authors = [{ name = "Stevo Brock", email = "StevoGTA@aol.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mini-document-storage-1.0.80/src/mini_document_storage/client/MDSClient.py` & `mini-document-storage-1.0.81/src/mini_document_storage/client/MDSClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Created by Stevo on 5/16/2023.
 # Copyright © 2023 Stevo Brock.  All rights reserved
 #
 
 # Imports
 import aiohttp
 import asyncio
+import base64
+import json
 
 #-----------------------------------------------------------------------------------------------------------------------
 # MDSClient
 class MDSClient:
     
 	# Lifecycle methods
 	#-------------------------------------------------------------------------------------------------------------------
@@ -86,90 +88,90 @@
 			await self.process_response(response)
 
 			return response
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_register(self, name, from_document_type, to_document_type, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		json = {
 			'name': name,
 			'fromDocumentType': from_document_type,
 			'toDocumentType': to_document_type,
 		}
 
 		# Queue request
-		async with self.session.put(f'/v1/association/{document_storage_id_use}', headers = self.headers,
+		async with self.session.put(f'/v1/association/{document_storage_id}', headers = self.headers,
 				json = json) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_update(self, name, updates, document_storage_id = None):
 		# Check if have updates
 		if len(updates) == 0:
 			# No updates
 			return
 
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
-		async with self.session.put(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.put(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				json = updates) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_document_infos(self, name, start_index = 0, count = None, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'startIndex': start_index}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.get(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_document_infos_from(self, name, document, start_index = 0, count = None,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'fromID': document.document_id, 'startIndex': start_index, 'fullInfo': 0}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.get(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_documents_from(self, name, document, start_index, count, document_creation_function,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'fromID': document.document_id, 'startIndex': start_index, 'fullInfo': 1}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.get(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			# Decode
 			infos = await response.json()
 
@@ -253,40 +255,40 @@
 
 		return to_documents_by_from_document_id
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_document_infos_to(self, name, document, start_index = 0, count = None,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'toID': document.document_id, 'startIndex': start_index, 'fullInfo': 0}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.get(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_documents_to(self, name, document, start_index, count, document_creation_function,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'toID': document.document_id, 'startIndex': start_index, 'fullInfo': 1}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}', headers = self.headers,
+		async with self.session.get(f'/v1/association/{document_storage_id}/{name}', headers = self.headers,
 				params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			# Decode
 			infos = await response.json()
 
@@ -370,28 +372,28 @@
 
 		return from_documents_by_to_document_id
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def association_get_value(self, name, action, from_documents, cache_name, cached_value_names,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		from_document_ids = list(map(lambda document: document.document_id, from_documents))
 
 		params = {
 			'cacheName': cache_name,
 			'cachedValueName': cached_value_names
 		}
 
 		async def worker(document_ids):
 			# Setup
 			params['fromID'] = document_ids
 
 			# Queue request
-			async with self.session.get(f'/v1/association/{document_storage_id_use}/{name}/{action}',
+			async with self.session.get(f'/v1/association/{document_storage_id}/{name}/{action}',
 					headers = self.headers, params = params) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					await self.process_response(response)
 
 					return await response.json()
@@ -416,57 +418,57 @@
 					break
 
 		return results
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def cache_register(self, name, document_type, relevant_properties, value_infos, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		json = {
 			'name': name,
 			'documentType': document_type,
 			'relevantProperties': relevant_properties,
 			'valueInfos': value_infos,
 		}
 
 		# Queue request
-		async with self.session.put(f'/v1/cache/{document_storage_id_use}', headers = self.headers,
+		async with self.session.put(f'/v1/cache/{document_storage_id}', headers = self.headers,
 				json = json) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def collection_register(self, name, document_type, relevant_properties, is_up_to_date, is_included_selector,
 			is_included_selector_info, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		json = {
 			'name': name,
 			'documentType': document_type,
 			'relevantProperties': relevant_properties,
 			'isUpToDate': is_up_to_date,
 			'isIncludedSelector': is_included_selector,
 			'isIncludedSelectorInfo': is_included_selector_info,
 		}
 
 		# Queue request
-		async with self.session.put(f'/v1/collection/{document_storage_id_use}', headers = self.headers,
+		async with self.session.put(f'/v1/collection/{document_storage_id}', headers = self.headers,
 				json = json) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def collection_get_document_count(self, name, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Loop until up-to-date
 		while True:
 			# Queue request
-			async with self.session.head(f'/v1/collection/{document_storage_id_use}/{name}',
+			async with self.session.head(f'/v1/collection/{document_storage_id}/{name}',
 					headers = self.headers) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					if not response.ok:
 						# Some error, but no additional info
 						raise Exception(f'HTTP response: {response.status}')
@@ -480,46 +482,46 @@
 					else:
 						# Don't have count
 						raise Exception('Unable to get count from response')
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def collection_get_document_infos(self, name, start_index = 0, count = None, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'startIndex': start_index, 'fullInfo': 0}
 		if count:
 			params['count'] = count
 
 		# Loop until up-to-date
 		while True:
 			# Queue request
-			async with self.session.get(f'/v1/collection/{document_storage_id_use}/{name}', headers = self.headers,
+			async with self.session.get(f'/v1/collection/{document_storage_id}/{name}', headers = self.headers,
 					params = params) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					await self.process_response(response)
 
 					return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def collection_get_documents(self, name, start_index, count, document_creation_function,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'startIndex': start_index, 'fullInfo': 1}
 		if count:
 			params['count'] = count
 
 		# Loop until up-to-date
 		while True:
 			# Queue request
-			async with self.session.get(f'/v1/collection/{document_storage_id_use}/{name}', headers = self.headers,
+			async with self.session.get(f'/v1/collection/{document_storage_id}/{name}', headers = self.headers,
 					params = params) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					await self.process_response(response)
 
 					# Decode
@@ -532,19 +534,19 @@
 		# Collect documents to create
 		documents_to_create = list(filter(lambda document: document.has_create_info, documents))
 		if len(documents_to_create) == 0:
 			# No documents
 			return
 		
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		json = [document.create_info() for document in documents_to_create]
 
 		# Queue request
-		async with self.session.post(f'/v1/document/{document_storage_id_use}/{document_type}', headers = self.headers,
+		async with self.session.post(f'/v1/document/{document_storage_id}/{document_type}', headers = self.headers,
 				json = json) as response:
 			# Process response
 			await self.process_response(response)
 
 			# Decode info
 			results = await response.json()
 
@@ -553,18 +555,18 @@
 			for result in results:
 				# Update document
 				documents_by_id[result['documentID']].update_from_create(result)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_get_count(self, document_type, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
-		async with self.session.head(f'/v1/document/{document_storage_id_use}/{document_type}',
+		async with self.session.head(f'/v1/document/{document_storage_id}/{document_type}',
 				headers = self.headers) as response:
 			# Process response
 			if not response.ok:
 				# Some error, but no additional info
 				raise Exception(f'HTTP response: {response.status}')
 			
 			# Decode header
@@ -577,50 +579,50 @@
 				# Don't have count
 				raise Exception('Unable to get count from response')
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_get_since_revision(self, document_type, since_revision, count, document_creation_function,
 			full_info = True, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'sinceRevision': since_revision, 'fullInfo': 1 if full_info else 0}
 		if count:
 			params['count'] = count
 
 		# Queue request
-		async with self.session.get(f'/v1/document/{document_storage_id_use}/{document_type}',
+		async with self.session.get(f'/v1/document/{document_storage_id}/{document_type}',
 				headers = self.headers, params = params) as response:
 			# Process response
 			await self.process_response(response)
 
 			# Decode info and add Documents
 			results = await response.json()
 
 			return list(map(document_creation_function, results))
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_get_all_since_revision(self, document_type, since_revision, batch_count,
 			document_creation_function, document_storage_id = None, proc = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		params = {'fullInfo': 1}
 		if batch_count:
 			params['count'] = batch_count
 
 		since_revision_use = since_revision
 		total_document_count = None
 
 		# Loop until done
 		documents = []
 		while True:
 			# Retrieve next batch of Documents
 			params['sinceRevision'] = since_revision_use
-			async with self.session.get(f'/v1/document/{document_storage_id_use}/{document_type}',
+			async with self.session.get(f'/v1/document/{document_storage_id}/{document_type}',
 					headers = self.headers, params = params) as response:
 				# Process response
 				await self.process_response(response)
 
 				# Decode
 				infos = await response.json()
 				documents_batch = list(map(document_creation_function, infos))
@@ -644,20 +646,20 @@
 				else:
 					# Have all Documents
 					return documents
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_get(self, document_type, document_ids, document_creation_function, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		documents = []
 		async def worker(document_ids):
 			# Queue request
-			async with self.session.get(f'/v1/document/{document_storage_id_use}/{document_type}',
+			async with self.session.get(f'/v1/document/{document_storage_id}/{document_type}',
 					headers = self.headers, params = {'id': document_ids, 'fullInfo': 1}) as response:
 				# Process response
 				await self.process_response(response)
 
 				# Decode info and add Documents
 				results = await response.json()
 				documents.extend(list(map(document_creation_function, results)))
@@ -676,22 +678,22 @@
 		# Collect documents to update
 		documents_to_update = list(filter(lambda document: document.has_update_info, documents))
 		if len(documents_to_update) == 0:
 			# No documents
 			return
 		
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		async def worker(documents):
 			# Setup
 			json = [document.update_info() for document in documents]
 
 			# Queue request
-			async with self.session.patch(f'/v1/document/{document_storage_id_use}/{document_type}',
+			async with self.session.patch(f'/v1/document/{document_storage_id}/{document_type}',
 					headers = self.headers, json = json) as response:
 				# Process response
 				await self.process_response(response)
 
 				# Decode info and add Documents
 				results = await response.json()
 
@@ -711,149 +713,169 @@
 			# Query for existing Folder
 			tasks.append(asyncio.ensure_future(worker(documents_to_update[i:i+10])))
 		await asyncio.gather(*tasks, return_exceptions = True)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_attachment_add(self, document_type, document_id, info, content, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
+
+		if type(content) is dict:
+			# Convert to string
+			content = json.dumps(content)
+		if type(content) is str:
+			# Convert to bytes
+			content = content.encode('utf-8')
+		if type(content) is bytes:
+			# Convert to Base64 string
+			content = base64.b64encode(content).decode('ascii')
 
 		# Queue request
-		async with self.session.post(f'/v1/document/{document_storage_id_use}/{document_type}/{document_id}/attachment',
+		async with self.session.post(f'/v1/document/{document_storage_id}/{document_type}/{document_id}/attachment',
 				headers = self.headers, json = {'info': info, 'content': content}) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_attachment_get(self, document_type, document_id, attachment_id, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
 		async with self.session.get(
-				f'/v1/document/{document_storage_id_use}/{document_type}/{document_id}/attachment/{attachment_id}',
+				f'/v1/document/{document_storage_id}/{document_type}/{document_id}/attachment/{attachment_id}',
 				headers = self.headers) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.read()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_attachment_update(self, document_type, document_id, attachment_id, info, content,
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
+
+		if type(content) is dict:
+			# Convert to string
+			content = json.dumps(content)
+		if type(content) is str:
+			# Convert to bytes
+			content = content.encode('utf-8')
+		if type(content) is bytes:
+			# Convert to Base64 string
+			content = base64.b64encode(content).decode('ascii')
 
 		# Queue request
 		async with self.session.patch(
-				f'/v1/document/{document_storage_id_use}/{document_type}/{document_id}/attachment/{attachment_id}',
+				f'/v1/document/{document_storage_id}/{document_type}/{document_id}/attachment/{attachment_id}',
 				headers = self.headers, json = {'info': info, 'content': content}) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def document_attachment_remove(self, document_type, document_id, attachment_id, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
 		async with self.session.delete(
-				f'/v1/document/{document_storage_id_use}/{document_type}/{document_id}/attachment/{attachment_id}',
+				f'/v1/document/{document_storage_id}/{document_type}/{document_id}/attachment/{attachment_id}',
 				headers = self.headers) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def index_register(self, name, document_type, relevant_properties, keys_selector, keys_selector_info = {},
 			document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 		json = {
 			'name': name,
 			'documentType': document_type,
 			'relevantProperties': relevant_properties,
 			'keysSelector': keys_selector,
 			'keysSelectorInfo': keys_selector_info,
 		}
 
 		# Queue request
-		async with self.session.put(f'/v1/index/{document_storage_id_use}', headers = self.headers,
+		async with self.session.put(f'/v1/index/{document_storage_id}', headers = self.headers,
 				json = json) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def index_get_document_infos(self, name, keys, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Loop until up-to-date
 		while True:
 			# Queue request
-			async with self.session.get(f'/v1/index/{document_storage_id_use}/{name}', headers = self.headers,
+			async with self.session.get(f'/v1/index/{document_storage_id}/{name}', headers = self.headers,
 					params = {'key': keys, 'fullInfo': 0}) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					await self.process_response(response)
 
 					return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def index_get_documents(self, name, keys, document_creation_function, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Loop until up-to-date
 		while True:
 			# Queue request
-			async with self.session.get(f'/v1/index/{document_storage_id_use}/{name}', headers = self.headers,
+			async with self.session.get(f'/v1/index/{document_storage_id}/{name}', headers = self.headers,
 					params = {'key': keys, 'fullInfo': 1}) as response:
 				# Handle results
 				if response.status != 409:
 					# Process response
 					await self.process_response(response)
 
 					results = await response.json()
 
 					return {k: document_creation_function(v) for k, v in results.items()}
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def info_get(self, keys, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
-		async with self.session.get(f'/v1/info/{document_storage_id_use}', headers = self.headers,
+		async with self.session.get(f'/v1/info/{document_storage_id}', headers = self.headers,
 				params = {'key': keys}) as response:
 			# Process response
 			await self.process_response(response)
 
 			return await response.json()
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def info_set(self, info, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
-		async with self.session.post(f'/v1/info/{document_storage_id_use}', headers = self.headers,
+		async with self.session.post(f'/v1/info/{document_storage_id}', headers = self.headers,
 				json = info) as response:
 			# Process response
 			await self.process_response(response)
 
 	#-------------------------------------------------------------------------------------------------------------------
 	async def internal_set(self, info, document_storage_id = None):
 		# Setup
-		document_storage_id_use = document_storage_id if document_storage_id else self.document_storage_id
+		document_storage_id = document_storage_id if document_storage_id else self.document_storage_id
 
 		# Queue request
-		async with self.session.post(f'/v1/internal/{document_storage_id_use}', headers = self.headers,
+		async with self.session.post(f'/v1/internal/{document_storage_id}', headers = self.headers,
 				json = info) as response:
 			# Process response
 			await self.process_response(response)
 
 	# Private methods
 	#-------------------------------------------------------------------------------------------------------------------
 	async def process_response(self, response):
```

### Comparing `mini-document-storage-1.0.80/src/mini_document_storage/client/MDSDocument.py` & `mini-document-storage-1.0.81/src/mini_document_storage/client/MDSDocument.py`

 * *Files identical despite different names*

### Comparing `mini-document-storage-1.0.80/src/mini_document_storage.egg-info/PKG-INFO` & `mini-document-storage-1.0.81/src/mini_document_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-document-storage
-Version: 1.0.80
+Version: 1.0.81
 Summary: Fast, inexpensive document storage backed by a standard database connector.
 Author-email: Stevo Brock <StevoGTA@aol.com>
 Project-URL: Homepage, https://github.com/StevoGTA/Mini-Document-Storage
 Keywords: document storage
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/starpoint-0.1.4.tar.gz` & `tmp/starpoint-0.2.0.tar.gz`

## Comparing `starpoint-0.1.4.tar` & `starpoint-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,18 @@
--rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.1.4/dev-requirements.txt
--rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.1.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.4/starpoint/__init__.py
--rw-r--r--   0        0        0    20438 2020-02-02 00:00:00.000000 starpoint-0.1.4/starpoint/db.py
--rw-r--r--   0        0        0    26788 2020-02-02 00:00:00.000000 starpoint-0.1.4/tests/test_db.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.4/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.4/LICENSE
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.1.4/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 starpoint-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    47395 2020-02-02 00:00:00.000000 starpoint-0.2.0/dev-requirements.txt
+-rw-r--r--   0        0        0    34194 2020-02-02 00:00:00.000000 starpoint-0.2.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/__init__.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/_utils.py
+-rw-r--r--   0        0        0     9626 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/db.py
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/openai.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/reader.py
+-rw-r--r--   0        0        0    12880 2020-02-02 00:00:00.000000 starpoint-0.2.0/starpoint/writer.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 starpoint-0.2.0/tests/test__utils.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 starpoint-0.2.0/tests/test_db.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 starpoint-0.2.0/tests/test_openai.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 starpoint-0.2.0/tests/test_reader.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 starpoint-0.2.0/tests/test_writer.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.2.0/LICENSE
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 starpoint-0.2.0/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 starpoint-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 starpoint-0.2.0/PKG-INFO
```

### Comparing `starpoint-0.1.4/dev-requirements.txt` & `starpoint-0.2.0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.4/requirements.txt` & `starpoint-0.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.4/starpoint/db.py` & `starpoint-0.2.0/starpoint/writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,70 @@
 import logging
-from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Dict, List, Optional
 from uuid import UUID
 
-import openai
 import requests
-import validators
 
-LOGGER = logging.getLogger(__name__)
+from starpoint._utils import (
+    _build_header,
+    _check_collection_identifier_collision,
+    _validate_host,
+)
 
-COLLECTIONS_PATH = "/api/v1/collections"
-DOCUMENTS_PATH = "/api/v1/documents"
-QUERY_PATH = "/api/v1/query"
-INFER_SCHEMA_PATH = "/api/v1/infer_schema"
-API_HEADER_KEY = "x-starpoint-key"
+LOGGER = logging.getLogger(__name__)
 
-READER_URL = "https://reader.starpoint.ai"
+# Host
 WRITER_URL = "https://writer.starpoint.ai"
 
-HEALTH_CHECK_MESSAGE = "hello."
+# Endpoints
+COLLECTIONS_PATH = "/api/v1/collections"
+DOCUMENTS_PATH = "/api/v1/documents"
 
-NO_HOST_ERROR = "No host value provided. A host must be provided."
-NO_COLLECTION_VALUE_ERROR = (
-    "Please provide at least one value for either collection_id or collection_name."
-)
-MULTI_COLLECTION_VALUE_ERROR = (
-    "Please only provide either collection_id or collection_name in your request."
-)
-NO_API_KEY_VALUE_ERROR = "Please provide at least one value for either api_key or filepath where the api key lives."
-MULTI_API_KEY_VALUE_ERROR = "Please only provide either api_key or filepath with the api_key in your initialization."
-NO_API_KEY_FILE_ERROR = "The provided filepath for the API key is not a valid file."
-SSL_ERROR_MSG = "Request failed due to SSLError. Error is likely due to invalid API key. Please check if your API is correct and still valid."
+# Error and warning messages
+DIMENSIONALITY_ERROR = "Dimensionality must be greater than 0."
 EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING = (
     "The length of the embeddings and document_metadata provided are different. There may be a mismatch "
     "between embeddings and the expected document metadata length; this may cause undesired collection insert or update."
 )
-NO_EMBEDDING_DATA_FOUND = (
-    "No embedding data found in the embedding response from OpenAI."
-)
-DIMENSIONALITY_ERROR = "Dimensionality must be greater than 0."
-
-
-def _build_header(api_key: UUID, additional_headers: Optional[Dict[str, str]] = None):
-    header = {API_HEADER_KEY: str(api_key)}
-    if additional_headers is not None:
-        header.update(additional_headers)
-    return header
-
-
-def _check_host_health(hostname: str):
-    resp = requests.get(hostname)
-    assert (
-        resp.ok
-    ), f"Host cannot be validated, response from host {hostname}: {resp.text}"
-    if resp.text != HEALTH_CHECK_MESSAGE:
-        LOGGER.warning(
-            f"{hostname} returned {resp.text} instead of {HEALTH_CHECK_MESSAGE}; host may be unhealthy and "
-            "may be unable to serve requests."
-        )
-
-
-def _set_and_validate_host(host: str):
-    if not host:
-        raise ValueError("No host value provided. A host must be provided.")
-    elif validators.url(host) is not True:  # type: ignore
-        raise ValueError(f"Provided host {host} is not a valid url format.")
-
-    # Make sure we don't have dangling backslashes in the url during url composition later
-    trimmed_hostname = host.rstrip("/")
-
-    _check_host_health(trimmed_hostname)
-
-    return trimmed_hostname
-
-
-def _check_collection_identifier_collision(
-    collection_id: Optional[str] = None, collection_name: Optional[str] = None
-):
-    if collection_id is None and collection_name is None:
-        raise ValueError(NO_COLLECTION_VALUE_ERROR)
-    elif collection_id and collection_name:
-        raise ValueError(MULTI_COLLECTION_VALUE_ERROR)
+SSL_ERROR_MSG = "Request failed due to SSLError. Error is likely due to invalid API key. Please check if your API is correct and still valid."
 
 
 class Writer(object):
-    """docstring for Writer"""
+    """Client for the Writer endpoints. If you do not need to separate reading or
+    writing for, consider using the [`Client` object](#client-objects)."""
 
     def __init__(self, api_key: UUID, host: Optional[str] = None):
         if host is None:
             host = WRITER_URL
 
-        self.host = _set_and_validate_host(host)
+        self.host = _validate_host(host)
         self.api_key = api_key
 
     def delete(
         self,
         documents: List[str],
         collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
+        """Remove documents in an existing collection.
+
+        Args:
+            documents: The documents to remove from the collection.
+            collection_id: The collection's id to remove the documents from.
+                This or the `collection_name` needs to be provided.
+            collection_name: The collection's name to remove the documents from.
+                This or the `collection_id` needs to be provided.
+
+        Returns:
+            dict: delete response json
+
+        Raises:
+            ValueError: If neither collection id and collection name are provided.
+            ValueError: If both collection id and collection name are provided.
+        """
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
         """
         dict(
             collection_id="collection_id_example",
@@ -140,14 +102,32 @@
 
     def insert(
         self,
         documents: List[Dict[Any, Any]],
         collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
+        """Insert documents into an existing collection.
+
+        Args:
+            documents: The documents to insert into the collection.
+            collection_id: The collection's id to insert the documents to.
+                This or the `collection_name` needs to be provided.
+            collection_name: The collection's name to insert the documents to.
+                This or the `collection_id` needs to be provided.
+
+        Returns:
+            dict: insert response json
+
+        Raises:
+            ValueError: If neither collection id and collection name are provided.
+            ValueError: If both collection id and collection name are provided.
+            requests.exceptions.SSLError: Failure likely due to network issues.
+        """
+
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
         """
         dict(
             collection_id="collection_id_example",
@@ -190,14 +170,35 @@
     def column_insert(
         self,
         embeddings: List[float],
         document_metadatas: List[Dict[Any, Any]],
         collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
+        """Insert documents into an existing collection by embedding and document metadata arrays.
+        The arrays are zipped together and inserted as a document in the order of the two arrays.
+
+        Args:
+            embeddings: A list of embeddings.
+                Order of the embeddings should match the document_metadatas.
+            document_metadatas: A list of metadata to be associated with embeddings.
+                Order of these metadatas should match the embeddings.
+            collection_id: The collection's id to insert the documents to.
+                This or the `collection_name` needs to be provided.
+            collection_name: The collection's name to insert the documents to.
+                This or the `collection_id` needs to be provided.
+
+        Returns:
+            dict: insert response json
+
+        Raises:
+            ValueError: If neither collection id and collection name are provided.
+            ValueError: If both collection id and collection name are provided.
+            requests.exceptions.SSLError: Failure likely due to network issues.
+        """
         if len(embeddings) != len(document_metadatas):
             LOGGER.warning(EMBEDDING_METADATA_LENGTH_MISMATCH_WARNING)
 
         documents = [
             {
                 "embedding": embedding,
                 "metadata": document_metadata,
@@ -213,14 +214,31 @@
 
     def update(
         self,
         documents: List[Dict[Any, Any]],
         collection_id: Optional[str] = None,
         collection_name: Optional[str] = None,
     ) -> Dict[Any, Any]:
+        """Update documents in an existing collection.
+
+        Args:
+            documents: The documents to update in the collection.
+            collection_id: The collection's id where the documents will be updated.
+                This or the `collection_name` needs to be provided.
+            collection_name: The collection's name where the documents will be updated.
+                This or the `collection_id` needs to be provided.
+
+        Returns:
+            dict: update response json
+
+        Raises:
+            ValueError: If neither collection id and collection name are provided.
+            ValueError: If both collection id and collection name are provided.
+            requests.exceptions.SSLError: Failure likely due to network issues.
+        """
         _check_collection_identifier_collision(collection_id, collection_name)
         # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
 
         # TODO: filter through documents to make sure values are what we expect them to be
         """
         dict(
             collection_id="collection_id_example",
@@ -259,19 +277,28 @@
             )
             return {}
         return response.json()
 
     def create_collection(
         self, collection_name: str, dimensionality: int
     ) -> Dict[Any, Any]:
-        """
-        dict(
-            name="collection_name_example",
-            dimensionality=1024,
-        )
+        """Creates a collection by name and dimensionality. Dimensionality
+        should be greater than 0.
+
+        Args:
+            collection_name: The name of the collection that will be created.
+            dimensionality: The number of dimensions the collection will have.
+                Must be an int larger than 0.
+
+        Returns:
+            dict: create collections response json
+
+        Raises:
+            ValueError: If dimensionality is 0 or less.
+            requests.exceptions.SSLError: Failure likely due to network issues.
         """
 
         if dimensionality <= 0:
             raise ValueError(DIMENSIONALITY_ERROR)
 
         request_data = dict(
             name=collection_name,
@@ -295,86 +322,31 @@
                 f"Request failed with status code {response.status_code} "
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
 
     def delete_collection(self, collection_id: str) -> Dict[Any, Any]:
-        """
-        dict(
-            collection_id="collection_id_example",
-        )
-        """
-
-        request_data = dict(
-            collection_id=collection_id,
-        )
-        try:
-            response = requests.delete(
-                url=f"{self.host}{COLLECTIONS_PATH}",
-                json=request_data,
-                headers=_build_header(
-                    api_key=self.api_key,
-                    additional_headers={"Content-Type": "application/json"},
-                ),
-            )
-        except requests.exceptions.SSLError as e:
-            LOGGER.error(SSL_ERROR_MSG)
-            raise e
+        """Deletes a collection.
 
-        if not response.ok:
-            LOGGER.error(
-                f"Request failed with status code {response.status_code} "
-                f"and the following message:\n{response.text}"
-            )
-            return {}
-        return response.json()
+        Args:
+            collection_id: The id of the collection that will be deleted.
 
+        Returns:
+            dict: deleted collection response json
 
-class Reader(object):
-    """docstring for Reader"""
-
-    def __init__(self, api_key: UUID, host: Optional[str] = None):
-        if host is None:
-            host = READER_URL
-
-        self.host = _set_and_validate_host(host)
-        self.api_key = api_key
-
-    def query(
-        self,
-        sql: Optional[str] = None,
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-        query_embedding: Optional[List[float]] = None,
-        params: Optional[List[Any]] = None,
-    ) -> Dict[Any, Any]:
-        _check_collection_identifier_collision(collection_id, collection_name)
-        # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
-
-        # TODO: filter through query_embedding to make sure values are what we expect
+        Raises:
+            requests.exceptions.SSLError: Failure likely due to network issues.
         """
-        dict(
-            collection_id="collection_id_example",
-            collection_name="collection_name_example",
-            query_embedding=None,
-            sql="sql_example",
-        )
-        """
-
         request_data = dict(
             collection_id=collection_id,
-            collection_name=collection_name,
-            query_embedding=query_embedding,
-            sql=sql,
-            params=params,
         )
         try:
-            response = requests.post(
-                url=f"{self.host}{QUERY_PATH}",
+            response = requests.delete(
+                url=f"{self.host}{COLLECTIONS_PATH}",
                 json=request_data,
                 headers=_build_header(
                     api_key=self.api_key,
                     additional_headers={"Content-Type": "application/json"},
                 ),
             )
         except requests.exceptions.SSLError as e:
@@ -384,230 +356,7 @@
         if not response.ok:
             LOGGER.error(
                 f"Request failed with status code {response.status_code} "
                 f"and the following message:\n{response.text}"
             )
             return {}
         return response.json()
-
-    def infer_schema(
-        self,
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        _check_collection_identifier_collision(collection_id, collection_name)
-        # TODO: Be safe and make sure the item passed through that doesn't hold a value is a None
-
-        """
-        dict(
-            collection_id="collection_id_example",
-            collection_name="collection_name_example",
-        )
-        """
-
-        request_data = dict(
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-        response = requests.post(
-            url=f"{self.host}{INFER_SCHEMA_PATH}",
-            json=request_data,
-            headers=_build_header(
-                api_key=self.api_key,
-                additional_headers={"Content-Type": "application/json"},
-            ),
-        )
-
-        if not response.ok:
-            LOGGER.error(
-                f"Request failed with status code {response.status_code} "
-                f"and the following message:\n{response.text}"
-            )
-            return {}
-        return response.json()
-
-
-class Client(object):
-    """docstring for Client"""
-
-    def __init__(
-        self,
-        api_key: UUID,
-        reader_host: Optional[str] = None,
-        writer_host: Optional[str] = None,
-    ):
-        self.writer = Writer(api_key=api_key, host=writer_host)
-        self.reader = Reader(api_key=api_key, host=reader_host)
-
-        # Consider a wrapper around openai once this class gets bloated
-        self.openai = None
-
-    def delete(
-        self,
-        documents: List[str],
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        return self.writer.delete(
-            documents=documents,
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-
-    def insert(
-        self,
-        documents: List[Dict[Any, Any]],
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        return self.writer.insert(
-            documents=documents,
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-
-    def column_insert(
-        self,
-        embeddings: List[float],
-        document_metadatas: List[Dict[Any, Any]],
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        return self.writer.column_insert(
-            embeddings=embeddings,
-            document_metadatas=document_metadatas,
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-
-    def query(
-        self,
-        sql: Optional[str] = None,
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-        query_embedding: Optional[List[float]] = None,
-        params: Optional[List[Any]] = None,
-    ) -> Dict[Any, Any]:
-        return self.reader.query(
-            sql=sql,
-            collection_id=collection_id,
-            collection_name=collection_name,
-            query_embedding=query_embedding,
-            params=params,
-        )
-
-    def infer_schema(
-        self,
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        return self.reader.infer_schema(
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-
-    def update(
-        self,
-        documents: List[Dict[Any, Any]],
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        return self.writer.update(
-            documents=documents,
-            collection_id=collection_id,
-            collection_name=collection_name,
-        )
-
-    def create_collection(
-        self, collection_name: str, dimensionality: int
-    ) -> Dict[Any, Any]:
-        return self.writer.create_collection(
-            collection_name=collection_name,
-            dimensionality=dimensionality,
-        )
-
-    def delete_collection(self, collection_id: str) -> Dict[Any, Any]:
-        return self.writer.delete_collection(
-            collection_id=collection_id,
-        )
-
-    """
-    OpenAI convenience wrappers
-    """
-
-    def init_openai(
-        self,
-        openai_key: Optional[str] = None,
-        openai_key_filepath: Optional[str] = None,
-    ):
-        """Initializes openai functionality"""
-        self.openai = openai
-        # TODO: maybe do this for starpoint api_key also
-
-        # If the init is unsuccessful, we deinitialize openai from this object in the except
-        try:
-            if openai_key and openai_key_filepath:
-                raise ValueError(MULTI_API_KEY_VALUE_ERROR)
-            elif openai_key is None:
-                if openai_key_filepath is None:
-                    raise ValueError(NO_API_KEY_VALUE_ERROR)
-                if not Path(openai_key_filepath).is_file():
-                    raise ValueError(NO_API_KEY_FILE_ERROR)
-                self.openai.api_key_path = openai_key_filepath
-            else:
-                self.openai.api_key = openai_key
-        except ValueError as e:
-            self.openai = None
-            raise e
-
-    def build_and_insert_embeddings_from_openai(
-        self,
-        model: str,
-        input_data: Union[str, Iterable[Any]],
-        document_metadatas: Optional[List[Dict[Any, Any]]] = None,
-        collection_id: Optional[str] = None,
-        collection_name: Optional[str] = None,
-        openai_user: Optional[str] = None,
-    ) -> Dict[Any, Any]:
-        if self.openai is None:
-            raise RuntimeError(
-                "OpenAI instance has not been initialized. Please initialize it using "
-                "Client.init_openai()"
-            )
-
-        _check_collection_identifier_collision(collection_id, collection_name)
-
-        embedding_response = self.openai.Embedding.create(
-            model=model, input=input_data, user=openai_user
-        )
-
-        embedding_data = embedding_response.get("data")
-        if embedding_data is None:
-            LOGGER.warning(NO_EMBEDDING_DATA_FOUND)
-            return embedding_response
-
-        if document_metadatas is None:
-            LOGGER.info(
-                "No custom document_metadatas provided. Using input_data for the document_metadatas"
-            )
-            if isinstance(input_data, str):
-                document_metadatas = [{"input": input_data}]
-            else:
-                document_metadatas = [{"input": data} for data in input_data]
-
-        # Return the embedding response no matter what issues/bugs we might run into in the sdk
-        try:
-            sorted_embedding_data = sorted(embedding_data, key=lambda x: x["index"])
-            embeddings = map(lambda x: x.get("embedding"), sorted_embedding_data)
-            self.column_insert(
-                embeddings=embeddings,
-                document_metadatas=document_metadatas,
-                collection_id=collection_id,
-                collection_name=collection_name,
-            )
-        except Exception as e:
-            LOGGER.error(
-                "An exception has occurred while trying to load embeddings into the db. "
-                f"This is the error:\n{e}"
-            )
-
-        return embedding_response
```

### Comparing `starpoint-0.1.4/LICENSE` & `starpoint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.4/README.md` & `starpoint-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `starpoint-0.1.4/pyproject.toml` & `starpoint-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "starpoint"
-version = "0.1.4"
+version = "0.2.0"
 authors = [{ name = "pointable", email = "package-maintainers@pointable.ai" }]
 description = "SDK for Starpoint DB"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `starpoint-0.1.4/PKG-INFO` & `starpoint-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starpoint
-Version: 0.1.4
+Version: 0.2.0
 Summary: SDK for Starpoint DB
 Project-URL: Homepage, https://github.com/starpoint-ai/sdk
 Project-URL: Bug Tracker, https://github.com/starpoint-ai/sdk/issues
 Author-email: pointable <package-maintainers@pointable.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


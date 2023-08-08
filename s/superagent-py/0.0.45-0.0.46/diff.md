# Comparing `tmp/superagent_py-0.0.45.tar.gz` & `tmp/superagent_py-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.45.tar", max compression
+gzip compressed data, was "superagent_py-0.0.46.tar", max compression
```

## Comparing `superagent_py-0.0.45.tar` & `superagent_py-0.0.46.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-08-06 18:48:07.029797 superagent_py-0.0.45/LICENSE
--rw-r--r--   0        0        0     3251 2023-08-06 18:48:07.029797 superagent_py-0.0.45/README.md
--rw-r--r--   0        0        0      380 2023-08-06 18:48:07.029797 superagent_py-0.0.45/pyproject.toml
--rw-r--r--   0        0        0      656 2023-08-06 18:48:07.029797 superagent_py-0.0.45/src/superagent/__init__.py
--rw-r--r--   0        0        0     3186 2023-08-06 18:48:07.029797 superagent_py-0.0.45/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-08-06 18:48:07.029797 superagent_py-0.0.45/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-06 18:48:07.029797 superagent_py-0.0.45/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/py.typed
--rw-r--r--   0        0        0      361 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14615 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     8684 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    12904 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/tags/__init__.py
--rw-r--r--   0        0        0    10575 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/tags/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0    11638 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-08-06 18:48:07.033798 superagent_py-0.0.45/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-07 15:14:33.979917 superagent_py-0.0.46/LICENSE
+-rw-r--r--   0        0        0     3251 2023-08-07 15:14:33.979917 superagent_py-0.0.46/README.md
+-rw-r--r--   0        0        0      380 2023-08-07 15:14:33.979917 superagent_py-0.0.46/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-07 15:14:33.979917 superagent_py-0.0.46/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    16778 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-08-07 15:14:33.983917 superagent_py-0.0.46/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     8684 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    12904 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-07 15:14:33.987917 superagent_py-0.0.46/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.46/PKG-INFO
```

### Comparing `superagent_py-0.0.45/LICENSE` & `superagent_py-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/README.md` & `superagent_py-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/__init__.py` & `superagent_py-0.0.46/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/client.py` & `superagent_py-0.0.46/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.46/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.46/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/agent/client.py` & `superagent_py-0.0.46/src/superagent/resources/agent/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,19 +40,25 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent(
         self,
         *,
         name: str,
         type: str,
+        description: typing.Optional[str] = OMIT,
+        avatar_url: typing.Optional[str] = OMIT,
         llm: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         has_memory: typing.Optional[bool] = OMIT,
         prompt_id: typing.Optional[str] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
+        if description is not OMIT:
+            _request["description"] = description
+        if avatar_url is not OMIT:
+            _request["avatarUrl"] = avatar_url
         if llm is not OMIT:
             _request["llm"] = llm
         if has_memory is not OMIT:
             _request["hasMemory"] = has_memory
         if prompt_id is not OMIT:
             _request["promptId"] = prompt_id
         _response = httpx.request(
@@ -70,14 +76,31 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def list_library_agents(self) -> typing.Any:
+        _response = httpx.request(
+            "GET",
+            urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents/library"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_agent(self, agent_id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -189,19 +212,25 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_agent(
         self,
         *,
         name: str,
         type: str,
+        description: typing.Optional[str] = OMIT,
+        avatar_url: typing.Optional[str] = OMIT,
         llm: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         has_memory: typing.Optional[bool] = OMIT,
         prompt_id: typing.Optional[str] = OMIT,
     ) -> typing.Any:
         _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
+        if description is not OMIT:
+            _request["description"] = description
+        if avatar_url is not OMIT:
+            _request["avatarUrl"] = avatar_url
         if llm is not OMIT:
             _request["llm"] = llm
         if has_memory is not OMIT:
             _request["hasMemory"] = has_memory
         if prompt_id is not OMIT:
             _request["promptId"] = prompt_id
         async with httpx.AsyncClient() as _client:
@@ -220,14 +249,32 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def list_library_agents(self) -> typing.Any:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "GET",
+                urllib.parse.urljoin(f"{self._environment}/", "api/v1/agents/library"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def get_agent(self, agent_id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/agents/{agent_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
```

### Comparing `superagent_py-0.0.45/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.46/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.46/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.46/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/auth/client.py` & `superagent_py-0.0.46/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/documents/client.py` & `superagent_py-0.0.46/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.46/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/tags/client.py` & `superagent_py-0.0.46/src/superagent/resources/tags/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/tools/client.py` & `superagent_py-0.0.46/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/traces/client.py` & `superagent_py-0.0.46/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/resources/user/client.py` & `superagent_py-0.0.46/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.46/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/src/superagent/types/validation_error.py` & `superagent_py-0.0.46/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.45/PKG-INFO` & `superagent_py-0.0.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.45
+Version: 0.0.46
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


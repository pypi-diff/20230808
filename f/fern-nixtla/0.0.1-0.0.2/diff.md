# Comparing `tmp/fern_nixtla-0.0.1.tar.gz` & `tmp/fern_nixtla-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_nixtla-0.0.1.tar", max compression
+gzip compressed data, was "fern_nixtla-0.0.2.tar", max compression
```

## Comparing `fern_nixtla-0.0.1.tar` & `fern_nixtla-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/README.md
--rw-r--r--   0        0        0      390 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      427 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/__init__.py
--rw-r--r--   0        0        0    18510 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/client.py
--rw-r--r--   0        0        0      519 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/api_error.py
--rw-r--r--   0        0        0     1202 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      162 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/environment.py
--rw-r--r--   0        0        0      170 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/py.typed
--rw-r--r--   0        0        0      377 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/types/__init__.py
--rw-r--r--   0        0        0      843 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/types/http_validation_error.py
--rw-r--r--   0        0        0      800 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/types/multi_series_input.py
--rw-r--r--   0        0        0      869 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-08-08 15:40:21.056161 fern_nixtla-0.0.1/src/nixtla/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_nixtla-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/README.md
+-rw-r--r--   0        0        0      390 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      427 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/__init__.py
+-rw-r--r--   0        0        0    18356 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/client.py
+-rw-r--r--   0        0        0      519 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/api_error.py
+-rw-r--r--   0        0        0     1202 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      162 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/environment.py
+-rw-r--r--   0        0        0      170 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/py.typed
+-rw-r--r--   0        0        0      377 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/types/http_validation_error.py
+-rw-r--r--   0        0        0      800 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/types/multi_series_input.py
+-rw-r--r--   0        0        0      869 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-08 15:47:16.073918 fern_nixtla-0.0.2/src/nixtla/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_nixtla-0.0.2/PKG-INFO
```

### Comparing `fern_nixtla-0.0.1/src/nixtla/client.py` & `fern_nixtla-0.0.2/src/nixtla/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         environment: NixtlaEnvironment = NixtlaEnvironment.DEFAULT,
         api_key: typing.Union[str, typing.Callable[[], str]],
         timeout: typing.Optional[float] = 60,
     ):
         self._environment = environment
         self._client_wrapper = SyncClientWrapper(api_key=api_key, httpx_client=httpx.Client(timeout=timeout))
 
-    def timegpt_timegpt_post(
+    def timegpt(
         self,
         *,
         fh: typing.Optional[int] = OMIT,
         y: typing.Optional[typing.Dict[str, float]] = OMIT,
         x: typing.Optional[typing.Dict[str, typing.Optional[typing.List[float]]]] = OMIT,
         freq: typing.Optional[str] = OMIT,
         clean_ex_first: typing.Optional[bool] = OMIT,
@@ -85,15 +85,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def timegpt_historic_timegpt_historic_post(
+    def historic(
         self,
         *,
         y: typing.Optional[typing.Any] = OMIT,
         x: typing.Optional[typing.Any] = OMIT,
         freq: typing.Optional[str] = OMIT,
         level: typing.Optional[typing.List[int]] = OMIT,
     ) -> typing.Any:
@@ -129,15 +129,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def timegpt_multi_series_timegpt_multi_series_post(
+    def multi_series(
         self,
         *,
         fh: typing.Optional[int] = OMIT,
         y: typing.Optional[MultiSeriesInput] = OMIT,
         x: typing.Optional[MultiSeriesInput] = OMIT,
         freq: typing.Optional[str] = OMIT,
         clean_ex_first: typing.Optional[bool] = OMIT,
@@ -200,15 +200,15 @@
         environment: NixtlaEnvironment = NixtlaEnvironment.DEFAULT,
         api_key: typing.Union[str, typing.Callable[[], str]],
         timeout: typing.Optional[float] = 60,
     ):
         self._environment = environment
         self._client_wrapper = AsyncClientWrapper(api_key=api_key, httpx_client=httpx.AsyncClient(timeout=timeout))
 
-    async def timegpt_timegpt_post(
+    async def timegpt(
         self,
         *,
         fh: typing.Optional[int] = OMIT,
         y: typing.Optional[typing.Dict[str, float]] = OMIT,
         x: typing.Optional[typing.Dict[str, typing.Optional[typing.List[float]]]] = OMIT,
         freq: typing.Optional[str] = OMIT,
         clean_ex_first: typing.Optional[bool] = OMIT,
@@ -259,15 +259,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def timegpt_historic_timegpt_historic_post(
+    async def historic(
         self,
         *,
         y: typing.Optional[typing.Any] = OMIT,
         x: typing.Optional[typing.Any] = OMIT,
         freq: typing.Optional[str] = OMIT,
         level: typing.Optional[typing.List[int]] = OMIT,
     ) -> typing.Any:
@@ -303,15 +303,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def timegpt_multi_series_timegpt_multi_series_post(
+    async def multi_series(
         self,
         *,
         fh: typing.Optional[int] = OMIT,
         y: typing.Optional[MultiSeriesInput] = OMIT,
         x: typing.Optional[MultiSeriesInput] = OMIT,
         freq: typing.Optional[str] = OMIT,
         clean_ex_first: typing.Optional[bool] = OMIT,
```

### Comparing `fern_nixtla-0.0.1/src/nixtla/core/__init__.py` & `fern_nixtla-0.0.2/src/nixtla/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_nixtla-0.0.1/src/nixtla/core/client_wrapper.py` & `fern_nixtla-0.0.2/src/nixtla/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, *, api_key: typing.Union[str, typing.Callable[[], str]]):
         self._api_key = api_key
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "fern-nixtla",
-            "X-Fern-SDK-Version": "0.0.1",
+            "X-Fern-SDK-Version": "0.0.2",
         }
         headers["Authorization"] = f"Bearer {self._get_api_key()}"
         return headers
 
     def _get_api_key(self) -> str:
         if isinstance(self._api_key, str):
             return self._api_key
```

### Comparing `fern_nixtla-0.0.1/src/nixtla/core/datetime_utils.py` & `fern_nixtla-0.0.2/src/nixtla/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_nixtla-0.0.1/src/nixtla/core/jsonable_encoder.py` & `fern_nixtla-0.0.2/src/nixtla/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_nixtla-0.0.1/src/nixtla/types/http_validation_error.py` & `fern_nixtla-0.0.2/src/nixtla/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_nixtla-0.0.1/src/nixtla/types/multi_series_input.py` & `fern_nixtla-0.0.2/src/nixtla/types/multi_series_input.py`

 * *Files identical despite different names*

### Comparing `fern_nixtla-0.0.1/src/nixtla/types/validation_error.py` & `fern_nixtla-0.0.2/src/nixtla/types/validation_error.py`

 * *Files identical despite different names*


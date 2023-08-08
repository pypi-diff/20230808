# Comparing `tmp/agent_protocol_client-0.0.1.tar.gz` & `tmp/agent_protocol_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol_client-0.0.1.tar", max compression
+gzip compressed data, was "agent_protocol_client-0.2.0.tar", max compression
```

## Comparing `agent_protocol_client-0.0.1.tar` & `agent_protocol_client-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      379 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/README.md
--rw-r--r--   0        0        0     1452 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/__init__.py
--rw-r--r--   0        0        0      104 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/api/__init__.py
--rw-r--r--   0        0        0    41991 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/api/agent_api.py
--rw-r--r--   0        0        0    29106 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/api_client.py
--rw-r--r--   0        0        0      805 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/api_response.py
--rw-r--r--   0        0        0    14143 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/configuration.py
--rw-r--r--   0        0        0    12794 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/docs/AgentApi.md
--rw-r--r--   0        0        0     5073 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/exceptions.py
--rw-r--r--   0        0        0      788 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/__init__.py
--rw-r--r--   0        0        0     3215 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/step.py
--rw-r--r--   0        0        0     1935 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/step_all_of.py
--rw-r--r--   0        0        0     2088 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/step_request_body.py
--rw-r--r--   0        0        0     2591 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/step_result.py
--rw-r--r--   0        0        0     2386 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/task.py
--rw-r--r--   0        0        0     2026 2023-07-21 13:28:11.586878 agent_protocol_client-0.0.1/agent_protocol_client/models/task_all_of.py
--rw-r--r--   0        0        0     2083 2023-07-21 13:28:11.590879 agent_protocol_client-0.0.1/agent_protocol_client/models/task_request_body.py
--rw-r--r--   0        0        0     9525 2023-07-21 13:28:11.590879 agent_protocol_client-0.0.1/agent_protocol_client/rest.py
--rw-r--r--   0        0        0      718 2023-07-21 13:28:11.590879 agent_protocol_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 agent_protocol_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1449 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api/__init__.py
+-rw-r--r--   0        0        0    56212 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api/agent_api.py
+-rw-r--r--   0        0        0    29108 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api_client.py
+-rw-r--r--   0        0        0      805 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api_response.py
+-rw-r--r--   0        0        0    14147 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/configuration.py
+-rw-r--r--   0        0        0    19210 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/docs/AgentApi.md
+-rw-r--r--   0        0        0     5075 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/exceptions.py
+-rw-r--r--   0        0        0      785 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/__init__.py
+-rw-r--r--   0        0        0     4866 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step.py
+-rw-r--r--   0        0        0     4286 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_all_of.py
+-rw-r--r--   0        0        0     2334 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_request_body.py
+-rw-r--r--   0        0        0     2591 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_result.py
+-rw-r--r--   0        0        0     3138 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task.py
+-rw-r--r--   0        0        0     2583 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task_all_of.py
+-rw-r--r--   0        0        0     2329 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task_request_body.py
+-rw-r--r--   0        0        0     9527 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/rest.py
+-rw-r--r--   0        0        0      733 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 agent_protocol_client-0.2.0/PKG-INFO
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/__init__.py` & `agent_protocol_client-0.2.0/agent_protocol_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 __version__ = "1.0.0"
@@ -27,14 +27,14 @@
 from agent_protocol_client.exceptions import ApiTypeError
 from agent_protocol_client.exceptions import ApiValueError
 from agent_protocol_client.exceptions import ApiKeyError
 from agent_protocol_client.exceptions import ApiAttributeError
 from agent_protocol_client.exceptions import ApiException
 
 # import models into sdk package
+from agent_protocol_client.models.artifact import Artifact
 from agent_protocol_client.models.step import Step
 from agent_protocol_client.models.step_all_of import StepAllOf
 from agent_protocol_client.models.step_request_body import StepRequestBody
-from agent_protocol_client.models.step_result import StepResult
 from agent_protocol_client.models.task import Task
 from agent_protocol_client.models.task_all_of import TaskAllOf
 from agent_protocol_client.models.task_request_body import TaskRequestBody
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/api/agent_api.py` & `agent_protocol_client-0.2.0/agent_protocol_client/api/agent_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import re  # noqa: F401
@@ -18,16 +18,17 @@
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 from typing import overload, Optional, Union, Awaitable
 
 from pydantic import Field, StrictStr
 
-from typing import List, Optional
+from typing import List, Optional, Union
 
+from agent_protocol_client.models.artifact import Artifact
 from agent_protocol_client.models.step import Step
 from agent_protocol_client.models.step_request_body import StepRequestBody
 from agent_protocol_client.models.task import Task
 from agent_protocol_client.models.task_request_body import TaskRequestBody
 
 from agent_protocol_client.api_client import ApiClient
 from agent_protocol_client.api_response import ApiResponse
@@ -217,14 +218,194 @@
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
         )
 
     @overload
+    async def download_agent_task_artifact(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        artifact_id: Annotated[StrictStr, Field(..., description="ID of the artifact")],
+        **kwargs
+    ) -> bytearray:  # noqa: E501
+        ...
+
+    @overload
+    def download_agent_task_artifact(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        artifact_id: Annotated[StrictStr, Field(..., description="ID of the artifact")],
+        async_req: Optional[bool] = True,
+        **kwargs
+    ) -> bytearray:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def download_agent_task_artifact(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        artifact_id: Annotated[StrictStr, Field(..., description="ID of the artifact")],
+        async_req: Optional[bool] = None,
+        **kwargs
+    ) -> Union[bytearray, Awaitable[bytearray]]:  # noqa: E501
+        """Download a specified artifact.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.download_agent_task_artifact(task_id, artifact_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param artifact_id: ID of the artifact (required)
+        :type artifact_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: bytearray
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the download_agent_task_artifact_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        if async_req is not None:
+            kwargs["async_req"] = async_req
+        return self.download_agent_task_artifact_with_http_info(
+            task_id, artifact_id, **kwargs
+        )  # noqa: E501
+
+    @validate_arguments
+    def download_agent_task_artifact_with_http_info(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        artifact_id: Annotated[StrictStr, Field(..., description="ID of the artifact")],
+        **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """Download a specified artifact.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.download_agent_task_artifact_with_http_info(task_id, artifact_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param artifact_id: ID of the artifact (required)
+        :type artifact_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = ["task_id", "artifact_id"]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method download_agent_task_artifact" % _key
+                )
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["task_id"]:
+            _path_params["task_id"] = _params["task_id"]
+
+        if _params["artifact_id"]:
+            _path_params["artifact_id"] = _params["artifact_id"]
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(
+            ["application/octet-stream"]
+        )  # noqa: E501
+
+        # authentication setting
+        _auth_settings = []  # noqa: E501
+
+        _response_types_map = {
+            "200": "bytearray",
+        }
+
+        return self.api_client.call_api(
+            "/agent/tasks/{task_id}/artifacts/{artifact_id}",
+            "GET",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @overload
     async def execute_agent_task_step(
         self,
         task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
         step_request_body: Optional[StepRequestBody] = None,
         **kwargs
     ) -> Step:  # noqa: E501
         ...
@@ -741,14 +922,183 @@
             "GET",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get("async_req"),
+            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
+            _preload_content=_params.get("_preload_content", True),
+            _request_timeout=_params.get("_request_timeout"),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get("_request_auth"),
+        )
+
+    @overload
+    async def list_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        **kwargs
+    ) -> List[Artifact]:  # noqa: E501
+        ...
+
+    @overload
+    def list_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        async_req: Optional[bool] = True,
+        **kwargs
+    ) -> List[Artifact]:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def list_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        async_req: Optional[bool] = None,
+        **kwargs
+    ) -> Union[List[Artifact], Awaitable[List[Artifact]]]:  # noqa: E501
+        """List all artifacts that have been created for the given task.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_agent_task_artifacts(task_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: List[Artifact]
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the list_agent_task_artifacts_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        if async_req is not None:
+            kwargs["async_req"] = async_req
+        return self.list_agent_task_artifacts_with_http_info(
+            task_id, **kwargs
+        )  # noqa: E501
+
+    @validate_arguments
+    def list_agent_task_artifacts_with_http_info(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """List all artifacts that have been created for the given task.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_agent_task_artifacts_with_http_info(task_id, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(List[Artifact], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = ["task_id"]
+        _all_params.extend(
+            [
+                "async_req",
+                "_return_http_data_only",
+                "_preload_content",
+                "_request_timeout",
+                "_request_auth",
+                "_content_type",
+                "_headers",
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params["kwargs"].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_agent_task_artifacts" % _key
+                )
+            _params[_key] = _val
+        del _params["kwargs"]
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params["task_id"]:
+            _path_params["task_id"] = _params["task_id"]
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get("_headers", {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(
+            ["application/json"]
+        )  # noqa: E501
+
+        # authentication setting
+        _auth_settings = []  # noqa: E501
+
+        _response_types_map = {
+            "200": "List[Artifact]",
+        }
+
+        return self.api_client.call_api(
+            "/agent/tasks/{task_id}/artifacts",
+            "GET",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
             response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get("async_req"),
             _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/api_client.py` & `agent_protocol_client-0.2.0/agent_protocol_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import atexit
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/api_response.py` & `agent_protocol_client-0.2.0/agent_protocol_client/api_response.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/configuration.py` & `agent_protocol_client-0.2.0/agent_protocol_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import copy
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: v1\n"
+            "Version of the API: v0.2\n"
             "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/docs/AgentApi.md` & `agent_protocol_client-0.2.0/agent_protocol_client/docs/AgentApi.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # agent_protocol_client.AgentApi
 
-All URIs are relative to *http://localhost*
-
-Method | HTTP request | Description
-------------- | ------------- | -------------
-[**create_agent_task**](AgentApi.md#create_agent_task) | **POST** /agent/tasks | Creates a task for the agent.
-[**execute_agent_task_step**](AgentApi.md#execute_agent_task_step) | **POST** /agent/tasks/{task_id}/steps | Execute a step in the specified agent task.
-[**get_agent_task**](AgentApi.md#get_agent_task) | **GET** /agent/tasks/{task_id} | Get details about a specified agent task.
-[**get_agent_task_step**](AgentApi.md#get_agent_task_step) | **GET** /agent/tasks/{task_id}/steps/{step_id} | Get details about a specified task step.
-[**list_agent_task_steps**](AgentApi.md#list_agent_task_steps) | **GET** /agent/tasks/{task_id}/steps | List all steps for the specified task.
-[**list_agent_tasks_ids**](AgentApi.md#list_agent_tasks_ids) | **GET** /agent/tasks | List all tasks that have been created for the agent.
+All URIs are relative to _http://localhost_
 
+| Method                                                                       | HTTP request                                           | Description                                                   |
+| ---------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------------------------------- |
+| [**create_agent_task**](AgentApi.md#create_agent_task)                       | **POST** /agent/tasks                                  | Creates a task for the agent.                                 |
+| [**download_agent_task_artifact**](AgentApi.md#download_agent_task_artifact) | **GET** /agent/tasks/{task_id}/artifacts/{artifact_id} | Download a specified artifact.                                |
+| [**execute_agent_task_step**](AgentApi.md#execute_agent_task_step)           | **POST** /agent/tasks/{task_id}/steps                  | Execute a step in the specified agent task.                   |
+| [**get_agent_task**](AgentApi.md#get_agent_task)                             | **GET** /agent/tasks/{task_id}                         | Get details about a specified agent task.                     |
+| [**get_agent_task_step**](AgentApi.md#get_agent_task_step)                   | **GET** /agent/tasks/{task_id}/steps/{step_id}         | Get details about a specified task step.                      |
+| [**list_agent_task_artifacts**](AgentApi.md#list_agent_task_artifacts)       | **GET** /agent/tasks/{task_id}/artifacts               | List all artifacts that have been created for the given task. |
+| [**list_agent_task_steps**](AgentApi.md#list_agent_task_steps)               | **GET** /agent/tasks/{task_id}/steps                   | List all steps for the specified task.                        |
+| [**list_agent_tasks_ids**](AgentApi.md#list_agent_tasks_ids)                 | **GET** /agent/tasks                                   | List all tasks that have been created for the agent.          |
 
 # **create_agent_task**
+
 > Task create_agent_task(task_request_body=task_request_body)
 
 Creates a task for the agent.
 
 ### Example
 
 ```python
@@ -46,43 +48,111 @@
         api_response = await api_instance.create_agent_task(task_request_body=task_request_body)
         print("The response of AgentApi->create_agent_task:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->create_agent_task: %s\n" % e)
 ```
 
-
 ### Parameters
 
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **task_request_body** | [**TaskRequestBody**](TaskRequestBody.md)|  | [optional] 
+| Name                  | Type                                      | Description | Notes      |
+| --------------------- | ----------------------------------------- | ----------- | ---------- |
+| **task_request_body** | [**TaskRequestBody**](TaskRequestBody.md) |             | [optional] |
 
 ### Return type
 
 [**Task**](Task.md)
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: application/json
- - **Accept**: application/json
+- **Content-Type**: application/json
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | A new agent task was successfuly created. |  -  |
-**0** | Internal Server Error |  -  |
+
+| Status code | Description                                | Response headers |
+| ----------- | ------------------------------------------ | ---------------- |
+| **200**     | A new agent task was successfully created. | -                |
+| **0**       | Internal Server Error                      | -                |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
+# **download_agent_task_artifact**
+
+> bytearray download_agent_task_artifact(task_id, artifact_id)
+
+Download a specified artifact.
+
+### Example
+
+```python
+import time
+import os
+import agent_protocol_client
+from agent_protocol_client.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to http://localhost
+# See configuration.py for a list of all supported configuration parameters.
+configuration = agent_protocol_client.Configuration(
+    host = "http://localhost"
+)
+
+
+# Enter a context with an instance of the API client
+async with agent_protocol_client.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = agent_protocol_client.AgentApi(api_client)
+    task_id = 'task_id_example' # str | ID of the task
+    artifact_id = 'artifact_id_example' # str | ID of the artifact
+
+    try:
+        # Download a specified artifact.
+        api_response = await api_instance.download_agent_task_artifact(task_id, artifact_id)
+        print("The response of AgentApi->download_agent_task_artifact:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling AgentApi->download_agent_task_artifact: %s\n" % e)
+```
+
+### Parameters
+
+| Name            | Type    | Description        | Notes |
+| --------------- | ------- | ------------------ | ----- |
+| **task_id**     | **str** | ID of the task     |
+| **artifact_id** | **str** | ID of the artifact |
+
+### Return type
+
+**bytearray**
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
+- **Content-Type**: Not defined
+- **Accept**: application/octet-stream
+
+### HTTP response details
+
+| Status code | Description                           | Response headers |
+| ----------- | ------------------------------------- | ---------------- |
+| **200**     | Returned the content of the artifact. | -                |
+| **0**       | Internal Server Error                 | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **execute_agent_task_step**
+
 > Step execute_agent_task_step(task_id, step_request_body=step_request_body)
 
 Execute a step in the specified agent task.
 
 ### Example
 
 ```python
@@ -113,44 +183,45 @@
         api_response = await api_instance.execute_agent_task_step(task_id, step_request_body=step_request_body)
         print("The response of AgentApi->execute_agent_task_step:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->execute_agent_task_step: %s\n" % e)
 ```
 
-
 ### Parameters
 
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **task_id** | **str**| ID of the task | 
- **step_request_body** | [**StepRequestBody**](StepRequestBody.md)|  | [optional] 
+| Name                  | Type                                      | Description    | Notes      |
+| --------------------- | ----------------------------------------- | -------------- | ---------- |
+| **task_id**           | **str**                                   | ID of the task |
+| **step_request_body** | [**StepRequestBody**](StepRequestBody.md) |                | [optional] |
 
 ### Return type
 
 [**Step**](Step.md)
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: application/json
- - **Accept**: application/json
+- **Content-Type**: application/json
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | Executed step for the agent task. |  -  |
-**0** | Internal Server Error |  -  |
+
+| Status code | Description                       | Response headers |
+| ----------- | --------------------------------- | ---------------- |
+| **200**     | Executed step for the agent task. | -                |
+| **0**       | Internal Server Error             | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **get_agent_task**
+
 > Task get_agent_task(task_id)
 
 Get details about a specified agent task.
 
 ### Example
 
 ```python
@@ -179,43 +250,44 @@
         api_response = await api_instance.get_agent_task(task_id)
         print("The response of AgentApi->get_agent_task:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->get_agent_task: %s\n" % e)
 ```
 
-
 ### Parameters
 
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **task_id** | **str**| ID of the task | 
+| Name        | Type    | Description    | Notes |
+| ----------- | ------- | -------------- | ----- |
+| **task_id** | **str** | ID of the task |
 
 ### Return type
 
 [**Task**](Task.md)
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: Not defined
- - **Accept**: application/json
+- **Content-Type**: Not defined
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | Returned details about an agent task. |  -  |
-**0** | Internal Server Error |  -  |
+
+| Status code | Description                           | Response headers |
+| ----------- | ------------------------------------- | ---------------- |
+| **200**     | Returned details about an agent task. | -                |
+| **0**       | Internal Server Error                 | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **get_agent_task_step**
+
 > Step get_agent_task_step(task_id, step_id)
 
 Get details about a specified task step.
 
 ### Example
 
 ```python
@@ -245,44 +317,111 @@
         api_response = await api_instance.get_agent_task_step(task_id, step_id)
         print("The response of AgentApi->get_agent_task_step:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->get_agent_task_step: %s\n" % e)
 ```
 
-
 ### Parameters
 
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **task_id** | **str**| ID of the task | 
- **step_id** | **str**| ID of the step | 
+| Name        | Type    | Description    | Notes |
+| ----------- | ------- | -------------- | ----- |
+| **task_id** | **str** | ID of the task |
+| **step_id** | **str** | ID of the step |
 
 ### Return type
 
 [**Step**](Step.md)
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: Not defined
- - **Accept**: application/json
+- **Content-Type**: Not defined
+- **Accept**: application/json
+
+### HTTP response details
+
+| Status code | Description                                | Response headers |
+| ----------- | ------------------------------------------ | ---------------- |
+| **200**     | Returned details about an agent task step. | -                |
+| **0**       | Internal Server Error                      | -                |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
+# **list_agent_task_artifacts**
+
+> List[Artifact] list_agent_task_artifacts(task_id)
+
+List all artifacts that have been created for the given task.
+
+### Example
+
+```python
+import time
+import os
+import agent_protocol_client
+from agent_protocol_client.models.artifact import Artifact
+from agent_protocol_client.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to http://localhost
+# See configuration.py for a list of all supported configuration parameters.
+configuration = agent_protocol_client.Configuration(
+    host = "http://localhost"
+)
+
+
+# Enter a context with an instance of the API client
+async with agent_protocol_client.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = agent_protocol_client.AgentApi(api_client)
+    task_id = 'task_id_example' # str | ID of the task
+
+    try:
+        # List all artifacts that have been created for the given task.
+        api_response = await api_instance.list_agent_task_artifacts(task_id)
+        print("The response of AgentApi->list_agent_task_artifacts:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling AgentApi->list_agent_task_artifacts: %s\n" % e)
+```
+
+### Parameters
+
+| Name        | Type    | Description    | Notes |
+| ----------- | ------- | -------------- | ----- |
+| **task_id** | **str** | ID of the task |
+
+### Return type
+
+[**List[Artifact]**](Artifact.md)
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
+- **Content-Type**: Not defined
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | Returned details about an agent task step. |  -  |
-**0** | Internal Server Error |  -  |
+
+| Status code | Description                           | Response headers |
+| ----------- | ------------------------------------- | ---------------- |
+| **200**     | Returned the content of the artifact. | -                |
+| **0**       | Internal Server Error                 | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **list_agent_task_steps**
+
 > List[str] list_agent_task_steps(task_id)
 
 List all steps for the specified task.
 
 ### Example
 
 ```python
@@ -310,43 +449,44 @@
         api_response = await api_instance.list_agent_task_steps(task_id)
         print("The response of AgentApi->list_agent_task_steps:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->list_agent_task_steps: %s\n" % e)
 ```
 
-
 ### Parameters
 
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **task_id** | **str**| ID of the task | 
+| Name        | Type    | Description    | Notes |
+| ----------- | ------- | -------------- | ----- |
+| **task_id** | **str** | ID of the task |
 
 ### Return type
 
 **List[str]**
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: Not defined
- - **Accept**: application/json
+- **Content-Type**: Not defined
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | Returned list of agent&#39;s step IDs for the specified task. |  -  |
-**0** | Internal Server Error |  -  |
+
+| Status code | Description                                                   | Response headers |
+| ----------- | ------------------------------------------------------------- | ---------------- |
+| **200**     | Returned list of agent&#39;s step IDs for the specified task. | -                |
+| **0**       | Internal Server Error                                         | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **list_agent_tasks_ids**
+
 > List[str] list_agent_tasks_ids()
 
 List all tasks that have been created for the agent.
 
 ### Example
 
 ```python
@@ -373,32 +513,32 @@
         api_response = await api_instance.list_agent_tasks_ids()
         print("The response of AgentApi->list_agent_tasks_ids:\n")
         pprint(api_response)
     except Exception as e:
         print("Exception when calling AgentApi->list_agent_tasks_ids: %s\n" % e)
 ```
 
-
 ### Parameters
+
 This endpoint does not need any parameter.
 
 ### Return type
 
 **List[str]**
 
 ### Authorization
 
 No authorization required
 
 ### HTTP request headers
 
- - **Content-Type**: Not defined
- - **Accept**: application/json
+- **Content-Type**: Not defined
+- **Accept**: application/json
 
 ### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**200** | Returned list of agent&#39;s task IDs. |  -  |
-**0** | Internal Server Error |  -  |
 
-[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+| Status code | Description                            | Response headers |
+| ----------- | -------------------------------------- | ---------------- |
+| **200**     | Returned list of agent&#39;s task IDs. | -                |
+| **0**       | Internal Server Error                  | -                |
 
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/exceptions.py` & `agent_protocol_client-0.2.0/agent_protocol_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 class OpenApiException(Exception):
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/__init__.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # flake8: noqa
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
+from agent_protocol_client.models.artifact import Artifact
 from agent_protocol_client.models.step import Step
 from agent_protocol_client.models.step_all_of import StepAllOf
 from agent_protocol_client.models.step_request_body import StepRequestBody
-from agent_protocol_client.models.step_result import StepResult
 from agent_protocol_client.models.task import Task
 from agent_protocol_client.models.task_all_of import TaskAllOf
 from agent_protocol_client.models.task_request_body import TaskRequestBody
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/step.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/step_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,40 +15,33 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictBool, conlist
 
 
-class Step(BaseModel):
+class StepResult(BaseModel):
     """
-    Step
+    Result of the task step.
     """
 
-    input: Optional[Any] = Field(
-        None, description="Input parameters for the task step. Any value is allowed."
-    )
     output: Optional[Any] = Field(
         None,
         description="Output that the task step has produced. Any value is allowed.",
     )
     artifacts: conlist(Any) = Field(
         ..., description="A list of artifacts that the step has produced."
     )
     is_last: Optional[StrictBool] = Field(
         False, description="Whether this is the last step in the task."
     )
-    task_id: StrictStr = Field(
-        ..., description="The ID of the task this step belongs to."
-    )
-    step_id: StrictStr = Field(..., description="The ID of the task step.")
-    __properties = ["input", "output", "artifacts", "is_last", "task_id", "step_id"]
+    __properties = ["output", "artifacts", "is_last"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -57,48 +50,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Step:
-        """Create an instance of Step from a JSON string"""
+    def from_json(cls, json_str: str) -> StepResult:
+        """Create an instance of StepResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if input (nullable) is None
-        # and __fields_set__ contains the field
-        if self.input is None and "input" in self.__fields_set__:
-            _dict["input"] = None
-
         # set to None if output (nullable) is None
         # and __fields_set__ contains the field
         if self.output is None and "output" in self.__fields_set__:
             _dict["output"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Step:
-        """Create an instance of Step from a dict"""
+    def from_dict(cls, obj: dict) -> StepResult:
+        """Create an instance of StepResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Step.parse_obj(obj)
+            return StepResult.parse_obj(obj)
 
-        _obj = Step.parse_obj(
+        _obj = StepResult.parse_obj(
             {
-                "input": obj.get("input"),
                 "output": obj.get("output"),
                 "artifacts": obj.get("artifacts"),
                 "is_last": obj.get("is_last")
                 if obj.get("is_last") is not None
                 else False,
-                "task_id": obj.get("task_id"),
-                "step_id": obj.get("step_id"),
             }
         )
         return _obj
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/step_all_of.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/task_all_of.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from pydantic import BaseModel, Field, StrictStr
+from typing import List
+from pydantic import BaseModel, Field, StrictStr, conlist
+from agent_protocol_client.models.artifact import Artifact
 
 
-class StepAllOf(BaseModel):
+class TaskAllOf(BaseModel):
     """
-    StepAllOf
+    Definition of an agent task.
     """
 
-    task_id: StrictStr = Field(
-        ..., description="The ID of the task this step belongs to."
+    task_id: StrictStr = Field(..., description="The ID of the task.")
+    artifacts: conlist(Artifact) = Field(
+        ..., description="A list of artifacts that the task has produced."
     )
-    step_id: StrictStr = Field(..., description="The ID of the task step.")
-    __properties = ["task_id", "step_id"]
+    __properties = ["task_id", "artifacts"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -43,29 +45,43 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StepAllOf:
-        """Create an instance of StepAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> TaskAllOf:
+        """Create an instance of TaskAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in artifacts (list)
+        _items = []
+        if self.artifacts:
+            for _item in self.artifacts:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["artifacts"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StepAllOf:
-        """Create an instance of StepAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> TaskAllOf:
+        """Create an instance of TaskAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return StepAllOf.parse_obj(obj)
+            return TaskAllOf.parse_obj(obj)
 
-        _obj = StepAllOf.parse_obj(
-            {"task_id": obj.get("task_id"), "step_id": obj.get("step_id")}
+        _obj = TaskAllOf.parse_obj(
+            {
+                "task_id": obj.get("task_id"),
+                "artifacts": [
+                    Artifact.from_dict(_item) for _item in obj.get("artifacts")
+                ]
+                if obj.get("artifacts") is not None
+                else None,
+            }
         )
         return _obj
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/step_request_body.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/step_request_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Optional
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, StrictStr
 
 
 class StepRequestBody(BaseModel):
     """
     Body of the task request.
     """
 
-    input: Optional[Any] = Field(
+    input: Optional[StrictStr] = Field(None, description="Input prompt for the step.")
+    additional_input: Optional[Any] = Field(
         None, description="Input parameters for the task step. Any value is allowed."
     )
-    __properties = ["input"]
+    __properties = ["input", "additional_input"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -50,25 +51,27 @@
     def from_json(cls, json_str: str) -> StepRequestBody:
         """Create an instance of StepRequestBody from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if input (nullable) is None
+        # set to None if additional_input (nullable) is None
         # and __fields_set__ contains the field
-        if self.input is None and "input" in self.__fields_set__:
-            _dict["input"] = None
+        if self.additional_input is None and "additional_input" in self.__fields_set__:
+            _dict["additional_input"] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> StepRequestBody:
         """Create an instance of StepRequestBody from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return StepRequestBody.parse_obj(obj)
 
-        _obj = StepRequestBody.parse_obj({"input": obj.get("input")})
+        _obj = StepRequestBody.parse_obj(
+            {"input": obj.get("input"), "additional_input": obj.get("additional_input")}
+        )
         return _obj
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/step_result.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictBool, conlist
+from pydantic import BaseModel, Field, StrictStr, conlist
+from agent_protocol_client.models.artifact import Artifact
 
 
-class StepResult(BaseModel):
+class Task(BaseModel):
     """
-    Result of the task step.
+    Task
     """
 
-    output: Optional[Any] = Field(
-        None,
-        description="Output that the task step has produced. Any value is allowed.",
+    input: Optional[StrictStr] = Field(None, description="Input prompt for the task.")
+    additional_input: Optional[Any] = Field(
+        None, description="Input parameters for the task. Any value is allowed."
     )
-    artifacts: conlist(Any) = Field(
-        ..., description="A list of artifacts that the step has produced."
+    task_id: StrictStr = Field(..., description="The ID of the task.")
+    artifacts: conlist(Artifact) = Field(
+        ..., description="A list of artifacts that the task has produced."
     )
-    is_last: Optional[StrictBool] = Field(
-        False, description="Whether this is the last step in the task."
-    )
-    __properties = ["output", "artifacts", "is_last"]
+    __properties = ["input", "additional_input", "task_id", "artifacts"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -50,40 +49,50 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> StepResult:
-        """Create an instance of StepResult from a JSON string"""
+    def from_json(cls, json_str: str) -> Task:
+        """Create an instance of Task from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if output (nullable) is None
+        # override the default output from pydantic by calling `to_dict()` of each item in artifacts (list)
+        _items = []
+        if self.artifacts:
+            for _item in self.artifacts:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["artifacts"] = _items
+        # set to None if additional_input (nullable) is None
         # and __fields_set__ contains the field
-        if self.output is None and "output" in self.__fields_set__:
-            _dict["output"] = None
+        if self.additional_input is None and "additional_input" in self.__fields_set__:
+            _dict["additional_input"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> StepResult:
-        """Create an instance of StepResult from a dict"""
+    def from_dict(cls, obj: dict) -> Task:
+        """Create an instance of Task from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return StepResult.parse_obj(obj)
+            return Task.parse_obj(obj)
 
-        _obj = StepResult.parse_obj(
+        _obj = Task.parse_obj(
             {
-                "output": obj.get("output"),
-                "artifacts": obj.get("artifacts"),
-                "is_last": obj.get("is_last")
-                if obj.get("is_last") is not None
-                else False,
+                "input": obj.get("input"),
+                "additional_input": obj.get("additional_input"),
+                "task_id": obj.get("task_id"),
+                "artifacts": [
+                    Artifact.from_dict(_item) for _item in obj.get("artifacts")
+                ]
+                if obj.get("artifacts") is not None
+                else None,
             }
         )
         return _obj
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/models/task.py` & `agent_protocol_client-0.2.0/agent_protocol_client/models/task_request_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, conlist
+from typing import Any, Optional
+from pydantic import BaseModel, Field, StrictStr
 
 
-class Task(BaseModel):
+class TaskRequestBody(BaseModel):
     """
-    Task
+    Body of the task request.
     """
 
-    input: Optional[Any] = Field(
+    input: Optional[StrictStr] = Field(None, description="Input prompt for the task.")
+    additional_input: Optional[Any] = Field(
         None, description="Input parameters for the task. Any value is allowed."
     )
-    task_id: StrictStr = Field(..., description="The ID of the task.")
-    artifacts: Optional[conlist(Any)] = Field(
-        None, description="A list of artifacts that the task has produced."
-    )
-    __properties = ["input", "task_id", "artifacts"]
+    __properties = ["input", "additional_input"]
 
     class Config:
         """Pydantic configuration"""
 
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -47,38 +44,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Task:
-        """Create an instance of Task from a JSON string"""
+    def from_json(cls, json_str: str) -> TaskRequestBody:
+        """Create an instance of TaskRequestBody from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # set to None if input (nullable) is None
+        # set to None if additional_input (nullable) is None
         # and __fields_set__ contains the field
-        if self.input is None and "input" in self.__fields_set__:
-            _dict["input"] = None
+        if self.additional_input is None and "additional_input" in self.__fields_set__:
+            _dict["additional_input"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Task:
-        """Create an instance of Task from a dict"""
+    def from_dict(cls, obj: dict) -> TaskRequestBody:
+        """Create an instance of TaskRequestBody from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Task.parse_obj(obj)
+            return TaskRequestBody.parse_obj(obj)
 
-        _obj = Task.parse_obj(
-            {
-                "input": obj.get("input"),
-                "task_id": obj.get("task_id"),
-                "artifacts": obj.get("artifacts"),
-            }
+        _obj = TaskRequestBody.parse_obj(
+            {"input": obj.get("input"), "additional_input": obj.get("additional_input")}
         )
         return _obj
```

### Comparing `agent_protocol_client-0.0.1/agent_protocol_client/rest.py` & `agent_protocol_client-0.2.0/agent_protocol_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Agent Communication Protocol
 
     Specification of the API protocol for communication with an agent.  # noqa: E501
 
-    The version of the OpenAPI document: v1
+    The version of the OpenAPI document: v0.2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import io
```

### Comparing `agent_protocol_client-0.0.1/pyproject.toml` & `agent_protocol_client-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent-protocol-client"
-version = "0.0.1"
+version = "0.2.0"
 description = "Agent Communication Protocol Client"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/sdk/tree/main/agent_client/python/"
 packages = [{ include = "agent_protocol_client" }]
@@ -22,8 +22,8 @@
 black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/e2b/sdk/issues"
+"Bug Tracker" = "https://github.com/e2b-dev/agent-protocol/issues"
```

### Comparing `agent_protocol_client-0.0.1/PKG-INFO` & `agent_protocol_client-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-protocol-client
-Version: 0.0.1
+Version: 0.2.0
 Summary: Agent Communication Protocol Client
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.11)
 Requires-Dist: aiohttp (>=3.8.4)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: urllib3 (>=1.25.3)
-Project-URL: Bug Tracker, https://github.com/e2b/sdk/issues
+Project-URL: Bug Tracker, https://github.com/e2b-dev/agent-protocol/issues
 Project-URL: Repository, https://github.com/e2b-dev/sdk/tree/main/agent_client/python/
 Description-Content-Type: text/markdown
 
 # Agent Communication Protocol - Python Client
 
 Python client for Agent Communication Protocol. This client simplifies the communication with the agent.
 
 ## Installation
+
 ```bash
 pip install agent-protocol-client
 ```
 
 ## Getting Started
 
 You can find simple usage in the example [here](./examples/minimal.py).
```


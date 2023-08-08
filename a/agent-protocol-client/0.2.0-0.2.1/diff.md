# Comparing `tmp/agent_protocol_client-0.2.0.tar.gz` & `tmp/agent_protocol_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_protocol_client-0.2.0.tar", max compression
+gzip compressed data, was "agent_protocol_client-0.2.1.tar", max compression
```

## Comparing `agent_protocol_client-0.2.0.tar` & `agent_protocol_client-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      380 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/README.md
--rw-r--r--   0        0        0     1449 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/__init__.py
--rw-r--r--   0        0        0      104 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api/__init__.py
--rw-r--r--   0        0        0    56212 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api/agent_api.py
--rw-r--r--   0        0        0    29108 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api_client.py
--rw-r--r--   0        0        0      805 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/api_response.py
--rw-r--r--   0        0        0    14147 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/configuration.py
--rw-r--r--   0        0        0    19210 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/docs/AgentApi.md
--rw-r--r--   0        0        0     5075 2023-08-08 09:27:04.422541 agent_protocol_client-0.2.0/agent_protocol_client/exceptions.py
--rw-r--r--   0        0        0      785 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/__init__.py
--rw-r--r--   0        0        0     4866 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step.py
--rw-r--r--   0        0        0     4286 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_all_of.py
--rw-r--r--   0        0        0     2334 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_request_body.py
--rw-r--r--   0        0        0     2591 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/step_result.py
--rw-r--r--   0        0        0     3138 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task.py
--rw-r--r--   0        0        0     2583 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task_all_of.py
--rw-r--r--   0        0        0     2329 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/models/task_request_body.py
--rw-r--r--   0        0        0     9527 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/agent_protocol_client/rest.py
--rw-r--r--   0        0        0      733 2023-08-08 09:27:04.426541 agent_protocol_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 agent_protocol_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/README.md
+-rw-r--r--   0        0        0     1449 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/api/__init__.py
+-rw-r--r--   0        0        0    65201 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/api/agent_api.py
+-rw-r--r--   0        0        0    29108 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/api_client.py
+-rw-r--r--   0        0        0      805 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/api_response.py
+-rw-r--r--   0        0        0    14147 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/configuration.py
+-rw-r--r--   0        0        0    22122 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/docs/AgentApi.md
+-rw-r--r--   0        0        0     5075 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/exceptions.py
+-rw-r--r--   0        0        0      785 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/__init__.py
+-rw-r--r--   0        0        0     4866 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/step.py
+-rw-r--r--   0        0        0     4286 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/step_all_of.py
+-rw-r--r--   0        0        0     2334 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/step_request_body.py
+-rw-r--r--   0        0        0     2591 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/step_result.py
+-rw-r--r--   0        0        0     3138 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/task.py
+-rw-r--r--   0        0        0     2583 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/task_all_of.py
+-rw-r--r--   0        0        0     2329 2023-08-08 13:03:54.416584 agent_protocol_client-0.2.1/agent_protocol_client/models/task_request_body.py
+-rw-r--r--   0        0        0     9527 2023-08-08 13:03:54.420584 agent_protocol_client-0.2.1/agent_protocol_client/rest.py
+-rw-r--r--   0        0        0      733 2023-08-08 13:03:54.420584 agent_protocol_client-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 agent_protocol_client-0.2.1/PKG-INFO
```

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/__init__.py` & `agent_protocol_client-0.2.1/agent_protocol_client/__init__.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/api/agent_api.py` & `agent_protocol_client-0.2.1/agent_protocol_client/api/agent_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 from typing import overload, Optional, Union, Awaitable
 
-from pydantic import Field, StrictStr
+from pydantic import Field, StrictBytes, StrictStr
 
 from typing import List, Optional, Union
 
 from agent_protocol_client.models.artifact import Artifact
 from agent_protocol_client.models.step import Step
 from agent_protocol_client.models.step_request_body import StepRequestBody
 from agent_protocol_client.models.task import Task
@@ -1410,14 +1410,241 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
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
+    async def upload_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        file: Annotated[
+            Union[StrictBytes, StrictStr], Field(..., description="File to upload.")
+        ],
+        relative_path: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Relative path of the artifact in the agent's workspace."
+            ),
+        ] = None,
+        **kwargs
+    ) -> Artifact:  # noqa: E501
+        ...
+
+    @overload
+    def upload_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        file: Annotated[
+            Union[StrictBytes, StrictStr], Field(..., description="File to upload.")
+        ],
+        relative_path: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Relative path of the artifact in the agent's workspace."
+            ),
+        ] = None,
+        async_req: Optional[bool] = True,
+        **kwargs
+    ) -> Artifact:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def upload_agent_task_artifacts(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        file: Annotated[
+            Union[StrictBytes, StrictStr], Field(..., description="File to upload.")
+        ],
+        relative_path: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Relative path of the artifact in the agent's workspace."
+            ),
+        ] = None,
+        async_req: Optional[bool] = None,
+        **kwargs
+    ) -> Union[Artifact, Awaitable[Artifact]]:  # noqa: E501
+        """Upload an artifact for the specified task.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.upload_agent_task_artifacts(task_id, file, relative_path, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param file: File to upload. (required)
+        :type file: bytearray
+        :param relative_path: Relative path of the artifact in the agent's workspace.
+        :type relative_path: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: Artifact
+        """
+        kwargs["_return_http_data_only"] = True
+        if "_preload_content" in kwargs:
+            raise ValueError(
+                "Error! Please call the upload_agent_task_artifacts_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"
+            )
+        if async_req is not None:
+            kwargs["async_req"] = async_req
+        return self.upload_agent_task_artifacts_with_http_info(
+            task_id, file, relative_path, **kwargs
+        )  # noqa: E501
+
+    @validate_arguments
+    def upload_agent_task_artifacts_with_http_info(
+        self,
+        task_id: Annotated[StrictStr, Field(..., description="ID of the task")],
+        file: Annotated[
+            Union[StrictBytes, StrictStr], Field(..., description="File to upload.")
+        ],
+        relative_path: Annotated[
+            Optional[StrictStr],
+            Field(
+                description="Relative path of the artifact in the agent's workspace."
+            ),
+        ] = None,
+        **kwargs
+    ) -> ApiResponse:  # noqa: E501
+        """Upload an artifact for the specified task.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.upload_agent_task_artifacts_with_http_info(task_id, file, relative_path, async_req=True)
+        >>> result = thread.get()
+
+        :param task_id: ID of the task (required)
+        :type task_id: str
+        :param file: File to upload. (required)
+        :type file: bytearray
+        :param relative_path: Relative path of the artifact in the agent's workspace.
+        :type relative_path: str
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
+        :rtype: tuple(Artifact, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = ["task_id", "file", "relative_path"]
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
+                    " to method upload_agent_task_artifacts" % _key
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
+        if _params["file"]:
+            _files["file"] = _params["file"]
+
+        if _params["relative_path"]:
+            _form_params.append(("relative_path", _params["relative_path"]))
+
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params["Accept"] = self.api_client.select_header_accept(
+            ["application/json"]
+        )  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get(
+            "_content_type",
+            self.api_client.select_header_content_type(["multipart/form-data"]),
+        )
+        if _content_types_list:
+            _header_params["Content-Type"] = _content_types_list
+
+        # authentication setting
+        _auth_settings = []  # noqa: E501
+
+        _response_types_map = {
+            "200": "Artifact",
+        }
+
+        return self.api_client.call_api(
+            "/agent/tasks/{task_id}/artifacts",
+            "POST",
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get("async_req"),
             _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
             _preload_content=_params.get("_preload_content", True),
             _request_timeout=_params.get("_request_timeout"),
             collection_formats=_collection_formats,
             _request_auth=_params.get("_request_auth"),
```

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/api_client.py` & `agent_protocol_client-0.2.1/agent_protocol_client/api_client.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/api_response.py` & `agent_protocol_client-0.2.1/agent_protocol_client/api_response.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/configuration.py` & `agent_protocol_client-0.2.1/agent_protocol_client/configuration.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/docs/AgentApi.md` & `agent_protocol_client-0.2.1/agent_protocol_client/docs/AgentApi.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 | [**download_agent_task_artifact**](AgentApi.md#download_agent_task_artifact) | **GET** /agent/tasks/{task_id}/artifacts/{artifact_id} | Download a specified artifact.                                |
 | [**execute_agent_task_step**](AgentApi.md#execute_agent_task_step)           | **POST** /agent/tasks/{task_id}/steps                  | Execute a step in the specified agent task.                   |
 | [**get_agent_task**](AgentApi.md#get_agent_task)                             | **GET** /agent/tasks/{task_id}                         | Get details about a specified agent task.                     |
 | [**get_agent_task_step**](AgentApi.md#get_agent_task_step)                   | **GET** /agent/tasks/{task_id}/steps/{step_id}         | Get details about a specified task step.                      |
 | [**list_agent_task_artifacts**](AgentApi.md#list_agent_task_artifacts)       | **GET** /agent/tasks/{task_id}/artifacts               | List all artifacts that have been created for the given task. |
 | [**list_agent_task_steps**](AgentApi.md#list_agent_task_steps)               | **GET** /agent/tasks/{task_id}/steps                   | List all steps for the specified task.                        |
 | [**list_agent_tasks_ids**](AgentApi.md#list_agent_tasks_ids)                 | **GET** /agent/tasks                                   | List all tasks that have been created for the agent.          |
+| [**upload_agent_task_artifacts**](AgentApi.md#upload_agent_task_artifacts)   | **POST** /agent/tasks/{task_id}/artifacts              | Upload an artifact for the specified task.                    |
 
 # **create_agent_task**
 
 > Task create_agent_task(task_request_body=task_request_body)
 
 Creates a task for the agent.
 
@@ -538,7 +539,77 @@
 
 | Status code | Description                            | Response headers |
 | ----------- | -------------------------------------- | ---------------- |
 | **200**     | Returned list of agent&#39;s task IDs. | -                |
 | **0**       | Internal Server Error                  | -                |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
+# **upload_agent_task_artifacts**
+
+> Artifact upload_agent_task_artifacts(task_id, file, relative_path=relative_path)
+
+Upload an artifact for the specified task.
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
+    file = None # bytearray | File to upload.
+    relative_path = 'relative_path_example' # str | Relative path of the artifact in the agent's workspace. (optional)
+
+    try:
+        # Upload an artifact for the specified task.
+        api_response = await api_instance.upload_agent_task_artifacts(task_id, file, relative_path=relative_path)
+        print("The response of AgentApi->upload_agent_task_artifacts:\n")
+        pprint(api_response)
+    except Exception as e:
+        print("Exception when calling AgentApi->upload_agent_task_artifacts: %s\n" % e)
+```
+
+### Parameters
+
+| Name              | Type          | Description                                                 | Notes      |
+| ----------------- | ------------- | ----------------------------------------------------------- | ---------- |
+| **task_id**       | **str**       | ID of the task                                              |
+| **file**          | **bytearray** | File to upload.                                             |
+| **relative_path** | **str**       | Relative path of the artifact in the agent&#39;s workspace. | [optional] |
+
+### Return type
+
+[**Artifact**](Artifact.md)
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
+- **Content-Type**: multipart/form-data
+- **Accept**: application/json
+
+### HTTP response details
+
+| Status code | Description                           | Response headers |
+| ----------- | ------------------------------------- | ---------------- |
+| **200**     | Returned the content of the artifact. | -                |
+| **0**       | Internal Server Error                 | -                |
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
```

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/exceptions.py` & `agent_protocol_client-0.2.1/agent_protocol_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/__init__.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/step.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/step.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/step_all_of.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/step_all_of.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/step_request_body.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/step_request_body.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/step_result.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/step_result.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/task.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/task.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/task_all_of.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/task_all_of.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/models/task_request_body.py` & `agent_protocol_client-0.2.1/agent_protocol_client/models/task_request_body.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/agent_protocol_client/rest.py` & `agent_protocol_client-0.2.1/agent_protocol_client/rest.py`

 * *Files identical despite different names*

### Comparing `agent_protocol_client-0.2.0/pyproject.toml` & `agent_protocol_client-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent-protocol-client"
-version = "0.2.0"
+version = "0.2.1"
 description = "Agent Communication Protocol Client"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/sdk/tree/main/agent_client/python/"
 packages = [{ include = "agent_protocol_client" }]
```

### Comparing `agent_protocol_client-0.2.0/PKG-INFO` & `agent_protocol_client-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-protocol-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Agent Communication Protocol Client
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


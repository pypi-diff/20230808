# Comparing `tmp/snitch-protos-0.0.57.tar.gz` & `tmp/snitch-protos-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.57.tar", last modified: Tue Aug  8 17:45:18 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.58.tar", last modified: Tue Aug  8 21:46:16 2023, max compression
```

## Comparing `snitch-protos-0.0.57.tar` & `snitch-protos-0.0.58.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 17:45:17.000000 snitch-protos-0.0.57/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 17:44:35.000000 snitch-protos-0.0.57/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:45:18.347193 snitch-protos-0.0.57/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 17:45:18.000000 snitch-protos-0.0.57/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    35734 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 21:45:47.000000 snitch-protos-0.0.58/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:46:16.802993 snitch-protos-0.0.58/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 21:46:16.000000 snitch-protos-0.0.58/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.57/PKG-INFO` & `snitch-protos-0.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.57
+Version: 0.0.58
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.57/setup.py` & `snitch-protos-0.0.58/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.57',
+    version='0.0.58',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.57/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.58/snitch_protos/protos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
     """
 
     PIPELINE_STEP_CONDITION_UNSET = 0
     PIPELINE_STEP_CONDITION_ABORT = 1
     PIPELINE_STEP_CONDITION_NOTIFY = 2
 
 
+class PipelineState(betterproto.Enum):
+    PIPELINE_STATE_UNSET = 0
+    PIPELINE_STATE_PAUSED = 1
+
+
 class ClientType(betterproto.Enum):
     CLIENT_TYPE_UNSET = 0
     CLIENT_TYPE_SDK = 1
     CLIENT_TYPE_SHIM = 2
 
 
 class WasmExitCode(betterproto.Enum):
@@ -142,74 +147,94 @@
     """What should SDK do if step fails?"""
 
     detective: "steps.DetectiveStep" = betterproto.message_field(1000, group="step")
     transform: "steps.TransformStep" = betterproto.message_field(1001, group="step")
     encode: "steps.EncodeStep" = betterproto.message_field(1002, group="step")
     decode: "steps.DecodeStep" = betterproto.message_field(1003, group="step")
     custom: "steps.CustomStep" = betterproto.message_field(1004, group="step")
+    wasm_id: Optional[str] = betterproto.string_field(
+        10000, optional=True, group="X_wasm_id"
+    )
+    """ID is a uuid(sha256(_wasm_bytes)) that is set by snitch-server"""
+
     wasm_bytes: Optional[bytes] = betterproto.bytes_field(
         10001, optional=True, group="X_wasm_bytes"
     )
     """WASM module bytes (set by snitch-server)"""
 
     wasm_function: Optional[str] = betterproto.string_field(
         10002, optional=True, group="X_wasm_function"
     )
     """WASM function name to execute (set by snitch-server)"""
 
 
 @dataclass(eq=False, repr=False)
-class ServiceInfo(betterproto.Message):
-    name: str = betterproto.string_field(1)
-    description: str = betterproto.string_field(2)
-    pipelines: List["PipelineInfo"] = betterproto.message_field(100)
-    consumers: List["ConsumerInfo"] = betterproto.message_field(101)
-    producers: List["ProducerInfo"] = betterproto.message_field(102)
-    clients: List["ClientInfo"] = betterproto.message_field(103)
-
+class LiveInfo(betterproto.Message):
+    audience: List["Audience"] = betterproto.message_field(1)
+    """If empty, client has not announced any audiences"""
 
-@dataclass(eq=False, repr=False)
-class PipelineInfo(betterproto.Message):
-    audience: "Audience" = betterproto.message_field(1)
-    pipeline: "Pipeline" = betterproto.message_field(2)
+    client: "ClientInfo" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
-class ConsumerInfo(betterproto.Message):
-    pass
-
+class PipelineInfo(betterproto.Message):
+    audiences: List["Audience"] = betterproto.message_field(1)
+    """If empty, pipeline is not attached to any audience"""
 
-@dataclass(eq=False, repr=False)
-class ProducerInfo(betterproto.Message):
-    pass
+    pipeline: "Pipeline" = betterproto.message_field(2)
+    state: "PipelineState" = betterproto.enum_field(3)
 
 
 @dataclass(eq=False, repr=False)
 class ClientInfo(betterproto.Message):
-    """This should come from the register call"""
+    """
+    Most of this is constructed by client SDKs and provided during Register
+    call
+    """
 
     client_type: "ClientType" = betterproto.enum_field(1)
     library_name: str = betterproto.string_field(2)
     library_version: str = betterproto.string_field(3)
     language: str = betterproto.string_field(4)
     arch: str = betterproto.string_field(5)
     os: str = betterproto.string_field(6)
+    session_id: Optional[str] = betterproto.string_field(
+        7, optional=True, group="X_session_id"
+    )
+    """Filled out by snitch_server on GetAll()"""
+
+    service_name: Optional[str] = betterproto.string_field(
+        8, optional=True, group="X_service_name"
+    )
+    node_name: Optional[str] = betterproto.string_field(
+        9, optional=True, group="X_node_name"
+    )
 
 
 @dataclass(eq=False, repr=False)
-class GetServiceMapRequest(betterproto.Message):
+class GetAllRequest(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
-class GetServiceMapResponse(betterproto.Message):
-    service_map: Dict[str, "ServiceInfo"] = betterproto.map_field(
-        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
+class GetAllResponse(betterproto.Message):
+    live: List["LiveInfo"] = betterproto.message_field(1)
+    """Clients currently connected to the server"""
+
+    audiences: List["Audience"] = betterproto.message_field(2)
+    """All of the audiences that are known to the server"""
+
+    pipelines: Dict[str, "PipelineInfo"] = betterproto.map_field(
+        3, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    """Key == service name"""
+    """
+    All of the pipelines known to the server + pipeline <-> audience mappings
+    key == pipeline_id; if "Audience" is not filled out - pipeline is not
+    attached to any audience.
+    """
 
 
 @dataclass(eq=False, repr=False)
 class GetPipelinesRequest(betterproto.Message):
     pass
 
 
@@ -466,26 +491,26 @@
 
     output: bytes = betterproto.bytes_field(1)
     exit_code: "WasmExitCode" = betterproto.enum_field(2)
     exit_msg: str = betterproto.string_field(3)
 
 
 class ExternalStub(betterproto.ServiceStub):
-    async def get_service_map(
+    async def get_all(
         self,
-        get_service_map_request: "GetServiceMapRequest",
+        get_all_request: "GetAllRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetServiceMapResponse":
+    ) -> "GetAllResponse":
         return await self._unary_unary(
-            "/protos.External/GetServiceMap",
-            get_service_map_request,
-            GetServiceMapResponse,
+            "/protos.External/GetAll",
+            get_all_request,
+            GetAllResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     async def get_pipelines(
         self,
@@ -743,17 +768,15 @@
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
 
 class ExternalBase(ServiceBase):
-    async def get_service_map(
-        self, get_service_map_request: "GetServiceMapRequest"
-    ) -> "GetServiceMapResponse":
+    async def get_all(self, get_all_request: "GetAllRequest") -> "GetAllResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def get_pipelines(
         self, get_pipelines_request: "GetPipelinesRequest"
     ) -> "GetPipelinesResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
@@ -796,20 +819,19 @@
         self, resume_pipeline_request: "ResumePipelineRequest"
     ) -> "StandardResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def test(self, test_request: "TestRequest") -> "TestResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def __rpc_get_service_map(
-        self,
-        stream: "grpclib.server.Stream[GetServiceMapRequest, GetServiceMapResponse]",
+    async def __rpc_get_all(
+        self, stream: "grpclib.server.Stream[GetAllRequest, GetAllResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.get_service_map(request)
+        response = await self.get_all(request)
         await stream.send_message(response)
 
     async def __rpc_get_pipelines(
         self, stream: "grpclib.server.Stream[GetPipelinesRequest, GetPipelinesResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.get_pipelines(request)
@@ -876,19 +898,19 @@
     ) -> None:
         request = await stream.recv_message()
         response = await self.test(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/protos.External/GetServiceMap": grpclib.const.Handler(
-                self.__rpc_get_service_map,
+            "/protos.External/GetAll": grpclib.const.Handler(
+                self.__rpc_get_all,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                GetServiceMapRequest,
-                GetServiceMapResponse,
+                GetAllRequest,
+                GetAllResponse,
             ),
             "/protos.External/GetPipelines": grpclib.const.Handler(
                 self.__rpc_get_pipelines,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 GetPipelinesRequest,
                 GetPipelinesResponse,
             ),
```

### Comparing `snitch-protos-0.0.57/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.58/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.57/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.58/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.57
+Version: 0.0.58
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```


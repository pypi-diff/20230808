# Comparing `tmp/alibabacloud_aiworkspace20210204-1.2.9.tar.gz` & `tmp/alibabacloud_aiworkspace20210204-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-1.2.9.tar", last modified: Mon Mar 13 02:43:09 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-2.0.0.tar", last modified: Tue Aug  8 08:19:41 2023, max compression
```

## Comparing `alibabacloud_aiworkspace20210204-1.2.9.tar` & `alibabacloud_aiworkspace20210204-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/
--rw-r--r--   0 root         (0) root         (0)      162 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/__init__.py
--rw-r--r--   0 root         (0) root         (0)   193814 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/client.py
--rw-r--r--   0 root         (0) root         (0)   288243 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-03-13 02:43:09.000000 alibabacloud_aiworkspace20210204-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   203838 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/client.py
+-rw-r--r--   0 root         (0) root         (0)   310457 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-08-08 08:19:41.000000 alibabacloud_aiworkspace20210204-2.0.0/setup.py
```

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/LICENSE` & `alibabacloud_aiworkspace20210204-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/PKG-INFO` & `alibabacloud_aiworkspace20210204-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiworkspace20210204
-Version: 1.2.9
+Version: 2.0.0
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/README-CN.md` & `alibabacloud_aiworkspace20210204-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/README.md` & `alibabacloud_aiworkspace20210204-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/client.py` & `alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,24 @@
     ) -> aiwork_space_20210204_models.AddImageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.image_id):
+            body['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.image_uri):
             body['ImageUri'] = request.image_uri
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -89,20 +93,24 @@
     ) -> aiwork_space_20210204_models.AddImageResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.accessibility):
             body['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
+        if not UtilClient.is_unset(request.image_id):
+            body['ImageId'] = request.image_id
         if not UtilClient.is_unset(request.image_uri):
             body['ImageUri'] = request.image_uri
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
@@ -419,14 +427,16 @@
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.property):
             body['Property'] = request.property
+        if not UtilClient.is_unset(request.provider_type):
+            body['ProviderType'] = request.provider_type
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.uri):
             body['Uri'] = request.uri
         if not UtilClient.is_unset(request.workspace_id):
@@ -471,14 +481,16 @@
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.property):
             body['Property'] = request.property
+        if not UtilClient.is_unset(request.provider_type):
+            body['ProviderType'] = request.provider_type
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.uri):
             body['Uri'] = request.uri
         if not UtilClient.is_unset(request.workspace_id):
@@ -695,14 +707,16 @@
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.model_description):
             body['ModelDescription'] = request.model_description
         if not UtilClient.is_unset(request.model_doc):
             body['ModelDoc'] = request.model_doc
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
+        if not UtilClient.is_unset(request.order_number):
+            body['OrderNumber'] = request.order_number
         if not UtilClient.is_unset(request.origin):
             body['Origin'] = request.origin
         if not UtilClient.is_unset(request.task):
             body['Task'] = request.task
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
@@ -741,14 +755,16 @@
             body['Labels'] = request.labels
         if not UtilClient.is_unset(request.model_description):
             body['ModelDescription'] = request.model_description
         if not UtilClient.is_unset(request.model_doc):
             body['ModelDoc'] = request.model_doc
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
+        if not UtilClient.is_unset(request.order_number):
+            body['OrderNumber'] = request.order_number
         if not UtilClient.is_unset(request.origin):
             body['Origin'] = request.origin
         if not UtilClient.is_unset(request.task):
             body['Task'] = request.task
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
@@ -882,14 +898,16 @@
             body['FormatType'] = request.format_type
         if not UtilClient.is_unset(request.framework_type):
             body['FrameworkType'] = request.framework_type
         if not UtilClient.is_unset(request.inference_spec):
             body['InferenceSpec'] = request.inference_spec
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
+        if not UtilClient.is_unset(request.metrics):
+            body['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.training_spec):
@@ -935,14 +953,16 @@
             body['FormatType'] = request.format_type
         if not UtilClient.is_unset(request.framework_type):
             body['FrameworkType'] = request.framework_type
         if not UtilClient.is_unset(request.inference_spec):
             body['InferenceSpec'] = request.inference_spec
         if not UtilClient.is_unset(request.labels):
             body['Labels'] = request.labels
+        if not UtilClient.is_unset(request.metrics):
+            body['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.training_spec):
@@ -1996,14 +2016,16 @@
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.option):
             query['Option'] = request.option
         if not UtilClient.is_unset(request.product_type):
             query['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteWorkspaceResource',
             version='2021-02-04',
@@ -2031,14 +2053,16 @@
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.option):
             query['Option'] = request.option
         if not UtilClient.is_unset(request.product_type):
             query['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.resource_type):
+            query['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DeleteWorkspaceResource',
             version='2021-02-04',
@@ -2661,14 +2685,80 @@
         permission_code: str,
         request: aiwork_space_20210204_models.GetPermissionRequest,
     ) -> aiwork_space_20210204_models.GetPermissionResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_permission_with_options_async(workspace_id, permission_code, request, headers, runtime)
 
+    def get_service_template_with_options(
+        self,
+        service_template_id: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> aiwork_space_20210204_models.GetServiceTemplateResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetServiceTemplate',
+            version='2021-02-04',
+            protocol='HTTPS',
+            pathname=f'/api/v1/servicetemplates/{OpenApiUtilClient.get_encode_param(service_template_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiwork_space_20210204_models.GetServiceTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_service_template_with_options_async(
+        self,
+        service_template_id: str,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> aiwork_space_20210204_models.GetServiceTemplateResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GetServiceTemplate',
+            version='2021-02-04',
+            protocol='HTTPS',
+            pathname=f'/api/v1/servicetemplates/{OpenApiUtilClient.get_encode_param(service_template_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiwork_space_20210204_models.GetServiceTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_service_template(
+        self,
+        service_template_id: str,
+    ) -> aiwork_space_20210204_models.GetServiceTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_service_template_with_options(service_template_id, headers, runtime)
+
+    async def get_service_template_async(
+        self,
+        service_template_id: str,
+    ) -> aiwork_space_20210204_models.GetServiceTemplateResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_service_template_with_options_async(service_template_id, headers, runtime)
+
     def get_workspace_with_options(
         self,
         workspace_id: str,
         request: aiwork_space_20210204_models.GetWorkspaceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.GetWorkspaceResponse:
@@ -3053,26 +3143,30 @@
         self,
         request: aiwork_space_20210204_models.ListImagesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.ListImagesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.accessibility):
+            query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.labels):
             query['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_user_id):
             query['ParentUserId'] = request.parent_user_id
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
         if not UtilClient.is_unset(request.sort_by):
             query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         if not UtilClient.is_unset(request.workspace_id):
@@ -3101,26 +3195,30 @@
         self,
         request: aiwork_space_20210204_models.ListImagesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.ListImagesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.accessibility):
+            query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.labels):
             query['Labels'] = request.labels
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.parent_user_id):
             query['ParentUserId'] = request.parent_user_id
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
         if not UtilClient.is_unset(request.sort_by):
             query['SortBy'] = request.sort_by
         if not UtilClient.is_unset(request.user_id):
             query['UserId'] = request.user_id
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         if not UtilClient.is_unset(request.workspace_id):
@@ -3735,14 +3833,16 @@
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.product_types):
             query['ProductTypes'] = request.product_types
         if not UtilClient.is_unset(request.resource_name):
             query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -3779,14 +3879,16 @@
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.product_types):
             query['ProductTypes'] = request.product_types
         if not UtilClient.is_unset(request.resource_name):
             query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_types):
+            query['ResourceTypes'] = request.resource_types
         if not UtilClient.is_unset(request.verbose):
             query['Verbose'] = request.verbose
         if not UtilClient.is_unset(request.workspace_id):
             query['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
@@ -3819,22 +3921,132 @@
         self,
         request: aiwork_space_20210204_models.ListResourcesRequest,
     ) -> aiwork_space_20210204_models.ListResourcesResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_resources_with_options_async(request, headers, runtime)
 
+    def list_service_templates_with_options(
+        self,
+        request: aiwork_space_20210204_models.ListServiceTemplatesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> aiwork_space_20210204_models.ListServiceTemplatesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label):
+            query['Label'] = request.label
+        if not UtilClient.is_unset(request.order):
+            query['Order'] = request.order
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.provider):
+            query['Provider'] = request.provider
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.service_template_name):
+            query['ServiceTemplateName'] = request.service_template_name
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListServiceTemplates',
+            version='2021-02-04',
+            protocol='HTTPS',
+            pathname=f'/api/v1/servicetemplates',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiwork_space_20210204_models.ListServiceTemplatesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_service_templates_with_options_async(
+        self,
+        request: aiwork_space_20210204_models.ListServiceTemplatesRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> aiwork_space_20210204_models.ListServiceTemplatesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.label):
+            query['Label'] = request.label
+        if not UtilClient.is_unset(request.order):
+            query['Order'] = request.order
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.provider):
+            query['Provider'] = request.provider
+        if not UtilClient.is_unset(request.query):
+            query['Query'] = request.query
+        if not UtilClient.is_unset(request.service_template_name):
+            query['ServiceTemplateName'] = request.service_template_name
+        if not UtilClient.is_unset(request.sort_by):
+            query['SortBy'] = request.sort_by
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListServiceTemplates',
+            version='2021-02-04',
+            protocol='HTTPS',
+            pathname=f'/api/v1/servicetemplates',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            aiwork_space_20210204_models.ListServiceTemplatesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_service_templates(
+        self,
+        request: aiwork_space_20210204_models.ListServiceTemplatesRequest,
+    ) -> aiwork_space_20210204_models.ListServiceTemplatesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_service_templates_with_options(request, headers, runtime)
+
+    async def list_service_templates_async(
+        self,
+        request: aiwork_space_20210204_models.ListServiceTemplatesRequest,
+    ) -> aiwork_space_20210204_models.ListServiceTemplatesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_service_templates_with_options_async(request, headers, runtime)
+
     def list_workspace_users_with_options(
         self,
         workspace_id: str,
+        request: aiwork_space_20210204_models.ListWorkspaceUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.ListWorkspaceUsersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListWorkspaceUsers',
             version='2021-02-04',
             protocol='HTTPS',
             pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/users',
             method='GET',
@@ -3847,19 +4059,25 @@
             aiwork_space_20210204_models.ListWorkspaceUsersResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_workspace_users_with_options_async(
         self,
         workspace_id: str,
+        request: aiwork_space_20210204_models.ListWorkspaceUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.ListWorkspaceUsersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.user_name):
+            query['UserName'] = request.user_name
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListWorkspaceUsers',
             version='2021-02-04',
             protocol='HTTPS',
             pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/users',
             method='GET',
@@ -3872,26 +4090,28 @@
             aiwork_space_20210204_models.ListWorkspaceUsersResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_workspace_users(
         self,
         workspace_id: str,
+        request: aiwork_space_20210204_models.ListWorkspaceUsersRequest,
     ) -> aiwork_space_20210204_models.ListWorkspaceUsersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_workspace_users_with_options(workspace_id, headers, runtime)
+        return self.list_workspace_users_with_options(workspace_id, request, headers, runtime)
 
     async def list_workspace_users_async(
         self,
         workspace_id: str,
+        request: aiwork_space_20210204_models.ListWorkspaceUsersRequest,
     ) -> aiwork_space_20210204_models.ListWorkspaceUsersResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_workspace_users_with_options_async(workspace_id, headers, runtime)
+        return await self.list_workspace_users_with_options_async(workspace_id, request, headers, runtime)
 
     def list_workspaces_with_options(
         self,
         request: aiwork_space_20210204_models.ListWorkspacesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.ListWorkspacesResponse:
@@ -4592,14 +4812,16 @@
             body['Domain'] = request.domain
         if not UtilClient.is_unset(request.model_description):
             body['ModelDescription'] = request.model_description
         if not UtilClient.is_unset(request.model_doc):
             body['ModelDoc'] = request.model_doc
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
+        if not UtilClient.is_unset(request.order_number):
+            body['OrderNumber'] = request.order_number
         if not UtilClient.is_unset(request.origin):
             body['Origin'] = request.origin
         if not UtilClient.is_unset(request.task):
             body['Task'] = request.task
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -4635,14 +4857,16 @@
             body['Domain'] = request.domain
         if not UtilClient.is_unset(request.model_description):
             body['ModelDescription'] = request.model_description
         if not UtilClient.is_unset(request.model_doc):
             body['ModelDoc'] = request.model_doc
         if not UtilClient.is_unset(request.model_name):
             body['ModelName'] = request.model_name
+        if not UtilClient.is_unset(request.order_number):
+            body['OrderNumber'] = request.order_number
         if not UtilClient.is_unset(request.origin):
             body['Origin'] = request.origin
         if not UtilClient.is_unset(request.task):
             body['Task'] = request.task
         req = open_api_models.OpenApiRequest(
             headers=headers,
             body=OpenApiUtilClient.parse_to_map(body)
@@ -4691,14 +4915,16 @@
     ) -> aiwork_space_20210204_models.UpdateModelVersionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.approval_status):
             body['ApprovalStatus'] = request.approval_status
         if not UtilClient.is_unset(request.inference_spec):
             body['InferenceSpec'] = request.inference_spec
+        if not UtilClient.is_unset(request.metrics):
+            body['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.training_spec):
@@ -4735,14 +4961,16 @@
     ) -> aiwork_space_20210204_models.UpdateModelVersionResponse:
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.approval_status):
             body['ApprovalStatus'] = request.approval_status
         if not UtilClient.is_unset(request.inference_spec):
             body['InferenceSpec'] = request.inference_spec
+        if not UtilClient.is_unset(request.metrics):
+            body['Metrics'] = request.metrics
         if not UtilClient.is_unset(request.options):
             body['Options'] = request.options
         if not UtilClient.is_unset(request.source_id):
             body['SourceId'] = request.source_id
         if not UtilClient.is_unset(request.source_type):
             body['SourceType'] = request.source_type
         if not UtilClient.is_unset(request.training_spec):
@@ -4877,25 +5105,25 @@
         self,
         workspace_id: str,
         request: aiwork_space_20210204_models.UpdateWorkspaceResourceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.UpdateWorkspaceResourceResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.group_name):
-            query['GroupName'] = request.group_name
         body = {}
+        if not UtilClient.is_unset(request.group_name):
+            body['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.is_default):
             body['IsDefault'] = request.is_default
         if not UtilClient.is_unset(request.product_type):
             body['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.resource_type):
+            body['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateWorkspaceResource',
             version='2021-02-04',
             protocol='HTTPS',
             pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/resources',
@@ -4914,25 +5142,25 @@
         self,
         workspace_id: str,
         request: aiwork_space_20210204_models.UpdateWorkspaceResourceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> aiwork_space_20210204_models.UpdateWorkspaceResourceResponse:
         UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.group_name):
-            query['GroupName'] = request.group_name
         body = {}
+        if not UtilClient.is_unset(request.group_name):
+            body['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.is_default):
             body['IsDefault'] = request.is_default
         if not UtilClient.is_unset(request.product_type):
             body['ProductType'] = request.product_type
+        if not UtilClient.is_unset(request.resource_type):
+            body['ResourceType'] = request.resource_type
         req = open_api_models.OpenApiRequest(
             headers=headers,
-            query=OpenApiUtilClient.query(query),
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateWorkspaceResource',
             version='2021-02-04',
             protocol='HTTPS',
             pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/resources',
```

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204/models.py` & `alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
         gmt_create_time: str = None,
         gmt_modified_time: str = None,
         labels: List[Label] = None,
         name: str = None,
         options: str = None,
         owner_id: str = None,
         property: str = None,
+        provider_type: str = None,
         source_id: str = None,
         source_type: str = None,
         uri: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
@@ -171,14 +172,15 @@
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.labels = labels
         self.name = name
         self.options = options
         self.owner_id = owner_id
         self.property = property
+        self.provider_type = provider_type
         self.source_id = source_id
         self.source_type = source_type
         self.uri = uri
         self.user_id = user_id
         self.workspace_id = workspace_id
 
     def validate(self):
@@ -215,14 +217,16 @@
             result['Name'] = self.name
         if self.options is not None:
             result['Options'] = self.options
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.property is not None:
             result['Property'] = self.property
+        if self.provider_type is not None:
+            result['ProviderType'] = self.provider_type
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.uri is not None:
             result['Uri'] = self.uri
         if self.user_id is not None:
@@ -256,14 +260,16 @@
             self.name = m.get('Name')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('Property') is not None:
             self.property = m.get('Property')
+        if m.get('ProviderType') is not None:
+            self.provider_type = m.get('ProviderType')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Uri') is not None:
             self.uri = m.get('Uri')
         if m.get('UserId') is not None:
@@ -312,14 +318,15 @@
         approval_status: str = None,
         format_type: str = None,
         framework_type: str = None,
         gmt_create_time: str = None,
         gmt_modified_time: str = None,
         inference_spec: Dict[str, Any] = None,
         labels: List[Label] = None,
+        metrics: Dict[str, Any] = None,
         options: str = None,
         owner_id: str = None,
         source_id: str = None,
         source_type: str = None,
         training_spec: Dict[str, Any] = None,
         uri: str = None,
         user_id: str = None,
@@ -329,14 +336,15 @@
         self.approval_status = approval_status
         self.format_type = format_type
         self.framework_type = framework_type
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.inference_spec = inference_spec
         self.labels = labels
+        self.metrics = metrics
         self.options = options
         self.owner_id = owner_id
         self.source_id = source_id
         self.source_type = source_type
         self.training_spec = training_spec
         self.uri = uri
         self.user_id = user_id
@@ -367,14 +375,16 @@
             result['GmtModifiedTime'] = self.gmt_modified_time
         if self.inference_spec is not None:
             result['InferenceSpec'] = self.inference_spec
         result['Labels'] = []
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
+        if self.metrics is not None:
+            result['Metrics'] = self.metrics
         if self.options is not None:
             result['Options'] = self.options
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
@@ -406,14 +416,16 @@
         if m.get('InferenceSpec') is not None:
             self.inference_spec = m.get('InferenceSpec')
         self.labels = []
         if m.get('Labels') is not None:
             for k in m.get('Labels'):
                 temp_model = Label()
                 self.labels.append(temp_model.from_map(k))
+        if m.get('Metrics') is not None:
+            self.metrics = m.get('Metrics')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
@@ -440,14 +452,15 @@
         gmt_modified_time: str = None,
         labels: List[Label] = None,
         latest_version: ModelVersion = None,
         model_description: str = None,
         model_doc: str = None,
         model_id: str = None,
         model_name: str = None,
+        order_number: int = None,
         origin: str = None,
         owner_id: str = None,
         provider: str = None,
         task: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
@@ -457,14 +470,15 @@
         self.gmt_modified_time = gmt_modified_time
         self.labels = labels
         self.latest_version = latest_version
         self.model_description = model_description
         self.model_doc = model_doc
         self.model_id = model_id
         self.model_name = model_name
+        self.order_number = order_number
         self.origin = origin
         self.owner_id = owner_id
         self.provider = provider
         self.task = task
         self.user_id = user_id
         self.workspace_id = workspace_id
 
@@ -500,14 +514,16 @@
             result['ModelDescription'] = self.model_description
         if self.model_doc is not None:
             result['ModelDoc'] = self.model_doc
         if self.model_id is not None:
             result['ModelId'] = self.model_id
         if self.model_name is not None:
             result['ModelName'] = self.model_name
+        if self.order_number is not None:
+            result['OrderNumber'] = self.order_number
         if self.origin is not None:
             result['Origin'] = self.origin
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.provider is not None:
             result['Provider'] = self.provider
         if self.task is not None:
@@ -540,14 +556,16 @@
             self.model_description = m.get('ModelDescription')
         if m.get('ModelDoc') is not None:
             self.model_doc = m.get('ModelDoc')
         if m.get('ModelId') is not None:
             self.model_id = m.get('ModelId')
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
+        if m.get('OrderNumber') is not None:
+            self.order_number = m.get('OrderNumber')
         if m.get('Origin') is not None:
             self.origin = m.get('Origin')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('Provider') is not None:
             self.provider = m.get('Provider')
         if m.get('Task') is not None:
@@ -555,38 +573,112 @@
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
-class ResourcesExecutorValue(TeaModel):
+class ServiceTemplate(TeaModel):
     def __init__(
         self,
+        gmt_create_time: str = None,
+        gmt_modified_time: str = None,
+        inference_spec: Dict[str, Any] = None,
+        labels: List[Label] = None,
+        order_number: int = None,
         owner_id: str = None,
+        provider: str = None,
+        service_template_description: str = None,
+        service_template_doc: str = None,
+        service_template_id: str = None,
+        service_template_name: str = None,
+        user_id: str = None,
     ):
+        self.gmt_create_time = gmt_create_time
+        self.gmt_modified_time = gmt_modified_time
+        self.inference_spec = inference_spec
+        self.labels = labels
+        self.order_number = order_number
         self.owner_id = owner_id
+        self.provider = provider
+        self.service_template_description = service_template_description
+        self.service_template_doc = service_template_doc
+        self.service_template_id = service_template_id
+        self.service_template_name = service_template_name
+        self.user_id = user_id
 
     def validate(self):
-        pass
+        if self.labels:
+            for k in self.labels:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.gmt_create_time is not None:
+            result['GmtCreateTime'] = self.gmt_create_time
+        if self.gmt_modified_time is not None:
+            result['GmtModifiedTime'] = self.gmt_modified_time
+        if self.inference_spec is not None:
+            result['InferenceSpec'] = self.inference_spec
+        result['Labels'] = []
+        if self.labels is not None:
+            for k in self.labels:
+                result['Labels'].append(k.to_map() if k else None)
+        if self.order_number is not None:
+            result['OrderNumber'] = self.order_number
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
+        if self.provider is not None:
+            result['Provider'] = self.provider
+        if self.service_template_description is not None:
+            result['ServiceTemplateDescription'] = self.service_template_description
+        if self.service_template_doc is not None:
+            result['ServiceTemplateDoc'] = self.service_template_doc
+        if self.service_template_id is not None:
+            result['ServiceTemplateId'] = self.service_template_id
+        if self.service_template_name is not None:
+            result['ServiceTemplateName'] = self.service_template_name
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('GmtCreateTime') is not None:
+            self.gmt_create_time = m.get('GmtCreateTime')
+        if m.get('GmtModifiedTime') is not None:
+            self.gmt_modified_time = m.get('GmtModifiedTime')
+        if m.get('InferenceSpec') is not None:
+            self.inference_spec = m.get('InferenceSpec')
+        self.labels = []
+        if m.get('Labels') is not None:
+            for k in m.get('Labels'):
+                temp_model = Label()
+                self.labels.append(temp_model.from_map(k))
+        if m.get('OrderNumber') is not None:
+            self.order_number = m.get('OrderNumber')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
+        if m.get('Provider') is not None:
+            self.provider = m.get('Provider')
+        if m.get('ServiceTemplateDescription') is not None:
+            self.service_template_description = m.get('ServiceTemplateDescription')
+        if m.get('ServiceTemplateDoc') is not None:
+            self.service_template_doc = m.get('ServiceTemplateDoc')
+        if m.get('ServiceTemplateId') is not None:
+            self.service_template_id = m.get('ServiceTemplateId')
+        if m.get('ServiceTemplateName') is not None:
+            self.service_template_name = m.get('ServiceTemplateName')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
         return self
 
 
 class AddImageRequestLabels(TeaModel):
     def __init__(
         self,
         key: str = None,
@@ -620,24 +712,28 @@
 
 
 class AddImageRequest(TeaModel):
     def __init__(
         self,
         accessibility: str = None,
         description: str = None,
+        image_id: str = None,
         image_uri: str = None,
         labels: List[AddImageRequestLabels] = None,
         name: str = None,
+        size: int = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
         self.description = description
+        self.image_id = image_id
         self.image_uri = image_uri
         self.labels = labels
         self.name = name
+        self.size = size
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
@@ -648,41 +744,49 @@
             return _map
 
         result = dict()
         if self.accessibility is not None:
             result['Accessibility'] = self.accessibility
         if self.description is not None:
             result['Description'] = self.description
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
         if self.image_uri is not None:
             result['ImageUri'] = self.image_uri
         result['Labels'] = []
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
+        if self.size is not None:
+            result['Size'] = self.size
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Accessibility') is not None:
             self.accessibility = m.get('Accessibility')
         if m.get('Description') is not None:
             self.description = m.get('Description')
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
         if m.get('ImageUri') is not None:
             self.image_uri = m.get('ImageUri')
         self.labels = []
         if m.get('Labels') is not None:
             for k in m.get('Labels'):
                 temp_model = AddImageRequestLabels()
                 self.labels.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
 class AddImageResponseBody(TeaModel):
     def __init__(
@@ -1130,27 +1234,29 @@
         data_source_type: str = None,
         data_type: str = None,
         description: str = None,
         labels: List[Label] = None,
         name: str = None,
         options: str = None,
         property: str = None,
+        provider_type: str = None,
         source_id: str = None,
         source_type: str = None,
         uri: str = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
         self.data_source_type = data_source_type
         self.data_type = data_type
         self.description = description
         self.labels = labels
         self.name = name
         self.options = options
         self.property = property
+        self.provider_type = provider_type
         self.source_id = source_id
         self.source_type = source_type
         self.uri = uri
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.labels:
@@ -1178,14 +1284,16 @@
                 result['Labels'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
         if self.options is not None:
             result['Options'] = self.options
         if self.property is not None:
             result['Property'] = self.property
+        if self.provider_type is not None:
+            result['ProviderType'] = self.provider_type
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.uri is not None:
             result['Uri'] = self.uri
         if self.workspace_id is not None:
@@ -1209,14 +1317,16 @@
                 self.labels.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('Property') is not None:
             self.property = m.get('Property')
+        if m.get('ProviderType') is not None:
+            self.provider_type = m.get('ProviderType')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Uri') is not None:
             self.uri = m.get('Uri')
         if m.get('WorkspaceId') is not None:
@@ -1610,24 +1720,26 @@
         self,
         accessibility: str = None,
         domain: str = None,
         labels: List[Label] = None,
         model_description: str = None,
         model_doc: str = None,
         model_name: str = None,
+        order_number: int = None,
         origin: str = None,
         task: str = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
         self.domain = domain
         self.labels = labels
         self.model_description = model_description
         self.model_doc = model_doc
         self.model_name = model_name
+        self.order_number = order_number
         self.origin = origin
         self.task = task
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
@@ -1650,14 +1762,16 @@
                 result['Labels'].append(k.to_map() if k else None)
         if self.model_description is not None:
             result['ModelDescription'] = self.model_description
         if self.model_doc is not None:
             result['ModelDoc'] = self.model_doc
         if self.model_name is not None:
             result['ModelName'] = self.model_name
+        if self.order_number is not None:
+            result['OrderNumber'] = self.order_number
         if self.origin is not None:
             result['Origin'] = self.origin
         if self.task is not None:
             result['Task'] = self.task
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
@@ -1675,14 +1789,16 @@
                 self.labels.append(temp_model.from_map(k))
         if m.get('ModelDescription') is not None:
             self.model_description = m.get('ModelDescription')
         if m.get('ModelDoc') is not None:
             self.model_doc = m.get('ModelDoc')
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
+        if m.get('OrderNumber') is not None:
+            self.order_number = m.get('OrderNumber')
         if m.get('Origin') is not None:
             self.origin = m.get('Origin')
         if m.get('Task') is not None:
             self.task = m.get('Task')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
@@ -1875,27 +1991,29 @@
     def __init__(
         self,
         approval_status: str = None,
         format_type: str = None,
         framework_type: str = None,
         inference_spec: Dict[str, Any] = None,
         labels: List[Label] = None,
+        metrics: Dict[str, Any] = None,
         options: str = None,
         source_id: str = None,
         source_type: str = None,
         training_spec: Dict[str, Any] = None,
         uri: str = None,
         version_description: str = None,
         version_name: str = None,
     ):
         self.approval_status = approval_status
         self.format_type = format_type
         self.framework_type = framework_type
         self.inference_spec = inference_spec
         self.labels = labels
+        self.metrics = metrics
         self.options = options
         self.source_id = source_id
         self.source_type = source_type
         self.training_spec = training_spec
         self.uri = uri
         self.version_description = version_description
         self.version_name = version_name
@@ -1920,14 +2038,16 @@
             result['FrameworkType'] = self.framework_type
         if self.inference_spec is not None:
             result['InferenceSpec'] = self.inference_spec
         result['Labels'] = []
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
+        if self.metrics is not None:
+            result['Metrics'] = self.metrics
         if self.options is not None:
             result['Options'] = self.options
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.training_spec is not None:
@@ -1951,14 +2071,16 @@
         if m.get('InferenceSpec') is not None:
             self.inference_spec = m.get('InferenceSpec')
         self.labels = []
         if m.get('Labels') is not None:
             for k in m.get('Labels'):
                 temp_model = Label()
                 self.labels.append(temp_model.from_map(k))
+        if m.get('Metrics') is not None:
+            self.metrics = m.get('Metrics')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('TrainingSpec') is not None:
@@ -2265,42 +2387,48 @@
         return self
 
 
 class CreateProductOrdersRequest(TeaModel):
     def __init__(
         self,
         auto_pay: bool = None,
-        products: CreateProductOrdersRequestProducts = None,
+        products: List[CreateProductOrdersRequestProducts] = None,
     ):
         self.auto_pay = auto_pay
         self.products = products
 
     def validate(self):
         if self.products:
-            self.products.validate()
+            for k in self.products:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auto_pay is not None:
             result['AutoPay'] = self.auto_pay
+        result['Products'] = []
         if self.products is not None:
-            result['Products'] = self.products.to_map()
+            for k in self.products:
+                result['Products'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AutoPay') is not None:
             self.auto_pay = m.get('AutoPay')
+        self.products = []
         if m.get('Products') is not None:
-            temp_model = CreateProductOrdersRequestProducts()
-            self.products = temp_model.from_map(m['Products'])
+            for k in m.get('Products'):
+                temp_model = CreateProductOrdersRequestProducts()
+                self.products.append(temp_model.from_map(k))
         return self
 
 
 class CreateProductOrdersResponseBody(TeaModel):
     def __init__(
         self,
         buy_product_request_id: str = None,
@@ -2543,23 +2671,25 @@
         self,
         env_type: str = None,
         group_name: str = None,
         is_default: bool = None,
         name: str = None,
         product_type: str = None,
         quotas: List[CreateWorkspaceResourceRequestResourcesQuotas] = None,
+        resource_type: str = None,
         spec: Dict[str, Any] = None,
         workspace_id: str = None,
     ):
         self.env_type = env_type
         self.group_name = group_name
         self.is_default = is_default
         self.name = name
         self.product_type = product_type
         self.quotas = quotas
+        self.resource_type = resource_type
         self.spec = spec
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.quotas:
             for k in self.quotas:
                 if k:
@@ -2581,14 +2711,16 @@
             result['Name'] = self.name
         if self.product_type is not None:
             result['ProductType'] = self.product_type
         result['Quotas'] = []
         if self.quotas is not None:
             for k in self.quotas:
                 result['Quotas'].append(k.to_map() if k else None)
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
         if self.spec is not None:
             result['Spec'] = self.spec
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
@@ -2604,14 +2736,16 @@
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
         self.quotas = []
         if m.get('Quotas') is not None:
             for k in m.get('Quotas'):
                 temp_model = CreateWorkspaceResourceRequestResourcesQuotas()
                 self.quotas.append(temp_model.from_map(k))
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
         if m.get('Spec') is not None:
             self.spec = m.get('Spec')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
@@ -3529,18 +3663,20 @@
 
 class DeleteWorkspaceResourceRequest(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         option: str = None,
         product_type: str = None,
+        resource_type: str = None,
     ):
         self.group_name = group_name
         self.option = option
         self.product_type = product_type
+        self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -3549,24 +3685,28 @@
         result = dict()
         if self.group_name is not None:
             result['GroupName'] = self.group_name
         if self.option is not None:
             result['Option'] = self.option
         if self.product_type is not None:
             result['ProductType'] = self.product_type
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('GroupName') is not None:
             self.group_name = m.get('GroupName')
         if m.get('Option') is not None:
             self.option = m.get('Option')
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
         return self
 
 
 class DeleteWorkspaceResourceResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
@@ -3803,14 +3943,15 @@
         gmt_create_time: str = None,
         gmt_modified_time: str = None,
         labels: List[Label] = None,
         name: str = None,
         options: str = None,
         owner_id: str = None,
         property: str = None,
+        provider_type: str = None,
         request_id: str = None,
         source_id: str = None,
         source_type: str = None,
         uri: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
@@ -3822,14 +3963,15 @@
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.labels = labels
         self.name = name
         self.options = options
         self.owner_id = owner_id
         self.property = property
+        self.provider_type = provider_type
         self.request_id = request_id
         self.source_id = source_id
         self.source_type = source_type
         self.uri = uri
         self.user_id = user_id
         self.workspace_id = workspace_id
 
@@ -3867,14 +4009,16 @@
             result['Name'] = self.name
         if self.options is not None:
             result['Options'] = self.options
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.property is not None:
             result['Property'] = self.property
+        if self.provider_type is not None:
+            result['ProviderType'] = self.provider_type
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.uri is not None:
@@ -3910,14 +4054,16 @@
             self.name = m.get('Name')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('Property') is not None:
             self.property = m.get('Property')
+        if m.get('ProviderType') is not None:
+            self.provider_type = m.get('ProviderType')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('Uri') is not None:
@@ -4294,26 +4440,28 @@
         gmt_create_time: str = None,
         gmt_modified_time: str = None,
         image_uri: str = None,
         labels: List[GetImageResponseBodyLabels] = None,
         name: str = None,
         parent_user_id: str = None,
         request_id: str = None,
+        size: int = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
         self.description = description
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.image_uri = image_uri
         self.labels = labels
         self.name = name
         self.parent_user_id = parent_user_id
         self.request_id = request_id
+        self.size = size
         self.user_id = user_id
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
@@ -4341,14 +4489,16 @@
                 result['Labels'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
         if self.parent_user_id is not None:
             result['ParentUserId'] = self.parent_user_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.size is not None:
+            result['Size'] = self.size
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
@@ -4370,14 +4520,16 @@
                 self.labels.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ParentUserId') is not None:
             self.parent_user_id = m.get('ParentUserId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
@@ -5065,14 +5217,159 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetPermissionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetServiceTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        gmt_create_time: str = None,
+        gmt_modified_time: str = None,
+        inference_spec: Dict[str, Any] = None,
+        labels: List[Label] = None,
+        owner_id: str = None,
+        provider: str = None,
+        request_id: str = None,
+        service_template_description: str = None,
+        service_template_doc: str = None,
+        service_template_id: str = None,
+        service_template_name: str = None,
+        user_id: str = None,
+    ):
+        self.gmt_create_time = gmt_create_time
+        self.gmt_modified_time = gmt_modified_time
+        self.inference_spec = inference_spec
+        self.labels = labels
+        self.owner_id = owner_id
+        self.provider = provider
+        self.request_id = request_id
+        self.service_template_description = service_template_description
+        self.service_template_doc = service_template_doc
+        self.service_template_id = service_template_id
+        self.service_template_name = service_template_name
+        self.user_id = user_id
+
+    def validate(self):
+        if self.labels:
+            for k in self.labels:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.gmt_create_time is not None:
+            result['GmtCreateTime'] = self.gmt_create_time
+        if self.gmt_modified_time is not None:
+            result['GmtModifiedTime'] = self.gmt_modified_time
+        if self.inference_spec is not None:
+            result['InferenceSpec'] = self.inference_spec
+        result['Labels'] = []
+        if self.labels is not None:
+            for k in self.labels:
+                result['Labels'].append(k.to_map() if k else None)
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.provider is not None:
+            result['Provider'] = self.provider
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.service_template_description is not None:
+            result['ServiceTemplateDescription'] = self.service_template_description
+        if self.service_template_doc is not None:
+            result['ServiceTemplateDoc'] = self.service_template_doc
+        if self.service_template_id is not None:
+            result['ServiceTemplateId'] = self.service_template_id
+        if self.service_template_name is not None:
+            result['ServiceTemplateName'] = self.service_template_name
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GmtCreateTime') is not None:
+            self.gmt_create_time = m.get('GmtCreateTime')
+        if m.get('GmtModifiedTime') is not None:
+            self.gmt_modified_time = m.get('GmtModifiedTime')
+        if m.get('InferenceSpec') is not None:
+            self.inference_spec = m.get('InferenceSpec')
+        self.labels = []
+        if m.get('Labels') is not None:
+            for k in m.get('Labels'):
+                temp_model = Label()
+                self.labels.append(temp_model.from_map(k))
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('Provider') is not None:
+            self.provider = m.get('Provider')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ServiceTemplateDescription') is not None:
+            self.service_template_description = m.get('ServiceTemplateDescription')
+        if m.get('ServiceTemplateDoc') is not None:
+            self.service_template_doc = m.get('ServiceTemplateDoc')
+        if m.get('ServiceTemplateId') is not None:
+            self.service_template_id = m.get('ServiceTemplateId')
+        if m.get('ServiceTemplateName') is not None:
+            self.service_template_name = m.get('ServiceTemplateName')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GetServiceTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetServiceTemplateResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetServiceTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetWorkspaceRequest(TeaModel):
     def __init__(
         self,
         verbose: bool = None,
     ):
         self.verbose = verbose
 
@@ -5792,81 +6089,93 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListImagesRequest(TeaModel):
     def __init__(
         self,
+        accessibility: str = None,
         labels: str = None,
         name: str = None,
         order: str = None,
         page_number: int = None,
         page_size: int = None,
         parent_user_id: str = None,
+        query: str = None,
         sort_by: str = None,
         user_id: str = None,
         verbose: bool = None,
         workspace_id: str = None,
     ):
+        self.accessibility = accessibility
         self.labels = labels
         self.name = name
         self.order = order
         self.page_number = page_number
         self.page_size = page_size
         self.parent_user_id = parent_user_id
+        self.query = query
         self.sort_by = sort_by
         self.user_id = user_id
         self.verbose = verbose
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.accessibility is not None:
+            result['Accessibility'] = self.accessibility
         if self.labels is not None:
             result['Labels'] = self.labels
         if self.name is not None:
             result['Name'] = self.name
         if self.order is not None:
             result['Order'] = self.order
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.parent_user_id is not None:
             result['ParentUserId'] = self.parent_user_id
+        if self.query is not None:
+            result['Query'] = self.query
         if self.sort_by is not None:
             result['SortBy'] = self.sort_by
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.verbose is not None:
             result['Verbose'] = self.verbose
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Accessibility') is not None:
+            self.accessibility = m.get('Accessibility')
         if m.get('Labels') is not None:
             self.labels = m.get('Labels')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Order') is not None:
             self.order = m.get('Order')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ParentUserId') is not None:
             self.parent_user_id = m.get('ParentUserId')
+        if m.get('Query') is not None:
+            self.query = m.get('Query')
         if m.get('SortBy') is not None:
             self.sort_by = m.get('SortBy')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('Verbose') is not None:
             self.verbose = m.get('Verbose')
         if m.get('WorkspaceId') is not None:
@@ -5915,26 +6224,28 @@
         gmt_create_time: str = None,
         gmt_modified_time: str = None,
         image_id: str = None,
         image_uri: str = None,
         labels: List[ListImagesResponseBodyImagesLabels] = None,
         name: str = None,
         parent_user_id: str = None,
+        size: int = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
         self.accessibility = accessibility
         self.description = description
         self.gmt_create_time = gmt_create_time
         self.gmt_modified_time = gmt_modified_time
         self.image_id = image_id
         self.image_uri = image_uri
         self.labels = labels
         self.name = name
         self.parent_user_id = parent_user_id
+        self.size = size
         self.user_id = user_id
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.labels:
             for k in self.labels:
                 if k:
@@ -5962,14 +6273,16 @@
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
         if self.name is not None:
             result['Name'] = self.name
         if self.parent_user_id is not None:
             result['ParentUserId'] = self.parent_user_id
+        if self.size is not None:
+            result['Size'] = self.size
         if self.user_id is not None:
             result['UserId'] = self.user_id
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
@@ -5991,14 +6304,16 @@
             for k in m.get('Labels'):
                 temp_model = ListImagesResponseBodyImagesLabels()
                 self.labels.append(temp_model.from_map(k))
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('ParentUserId') is not None:
             self.parent_user_id = m.get('ParentUserId')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
@@ -7275,23 +7590,25 @@
         self,
         group_name: str = None,
         option: str = None,
         page_number: int = None,
         page_size: int = None,
         product_types: str = None,
         resource_name: str = None,
+        resource_types: str = None,
         verbose: bool = None,
         workspace_id: str = None,
     ):
         self.group_name = group_name
         self.option = option
         self.page_number = page_number
         self.page_size = page_size
         self.product_types = product_types
         self.resource_name = resource_name
+        self.resource_types = resource_types
         self.verbose = verbose
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7308,14 +7625,16 @@
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
         if self.product_types is not None:
             result['ProductTypes'] = self.product_types
         if self.resource_name is not None:
             result['ResourceName'] = self.resource_name
+        if self.resource_types is not None:
+            result['ResourceTypes'] = self.resource_types
         if self.verbose is not None:
             result['Verbose'] = self.verbose
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
@@ -7328,21 +7647,89 @@
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('ProductTypes') is not None:
             self.product_types = m.get('ProductTypes')
         if m.get('ResourceName') is not None:
             self.resource_name = m.get('ResourceName')
+        if m.get('ResourceTypes') is not None:
+            self.resource_types = m.get('ResourceTypes')
         if m.get('Verbose') is not None:
             self.verbose = m.get('Verbose')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
+class ListResourcesResponseBodyResourcesEncryption(TeaModel):
+    def __init__(
+        self,
+        algorithm: str = None,
+        enabled: bool = None,
+        key: str = None,
+    ):
+        self.algorithm = algorithm
+        self.enabled = enabled
+        self.key = key
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.algorithm is not None:
+            result['Algorithm'] = self.algorithm
+        if self.enabled is not None:
+            result['Enabled'] = self.enabled
+        if self.key is not None:
+            result['Key'] = self.key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Algorithm') is not None:
+            self.algorithm = m.get('Algorithm')
+        if m.get('Enabled') is not None:
+            self.enabled = m.get('Enabled')
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        return self
+
+
+class ListResourcesResponseBodyResourcesExecutor(TeaModel):
+    def __init__(
+        self,
+        owner_id: str = None,
+    ):
+        self.owner_id = owner_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        return self
+
+
 class ListResourcesResponseBodyResourcesQuotasSpecs(TeaModel):
     def __init__(
         self,
         name: str = None,
         value: str = None,
     ):
         self.name = name
@@ -7448,60 +7835,64 @@
                 self.specs.append(temp_model.from_map(k))
         return self
 
 
 class ListResourcesResponseBodyResources(TeaModel):
     def __init__(
         self,
+        encryption: ListResourcesResponseBodyResourcesEncryption = None,
         env_type: str = None,
-        executor: Dict[str, ResourcesExecutorValue] = None,
+        executor: ListResourcesResponseBodyResourcesExecutor = None,
         gmt_create_time: str = None,
         group_name: str = None,
         id: str = None,
         is_default: bool = None,
         name: str = None,
         product_type: str = None,
         quotas: List[ListResourcesResponseBodyResourcesQuotas] = None,
+        resource_type: str = None,
         spec: Dict[str, Any] = None,
         workspace_id: str = None,
     ):
+        self.encryption = encryption
         self.env_type = env_type
         self.executor = executor
         self.gmt_create_time = gmt_create_time
         self.group_name = group_name
         self.id = id
         self.is_default = is_default
         self.name = name
         self.product_type = product_type
         self.quotas = quotas
+        self.resource_type = resource_type
         self.spec = spec
         self.workspace_id = workspace_id
 
     def validate(self):
+        if self.encryption:
+            self.encryption.validate()
         if self.executor:
-            for v in self.executor.values():
-                if v:
-                    v.validate()
+            self.executor.validate()
         if self.quotas:
             for k in self.quotas:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.encryption is not None:
+            result['Encryption'] = self.encryption.to_map()
         if self.env_type is not None:
             result['EnvType'] = self.env_type
-        result['Executor'] = {}
         if self.executor is not None:
-            for k, v in self.executor.items():
-                result['Executor'][k] = v.to_map()
+            result['Executor'] = self.executor.to_map()
         if self.gmt_create_time is not None:
             result['GmtCreateTime'] = self.gmt_create_time
         if self.group_name is not None:
             result['GroupName'] = self.group_name
         if self.id is not None:
             result['Id'] = self.id
         if self.is_default is not None:
@@ -7510,29 +7901,32 @@
             result['Name'] = self.name
         if self.product_type is not None:
             result['ProductType'] = self.product_type
         result['Quotas'] = []
         if self.quotas is not None:
             for k in self.quotas:
                 result['Quotas'].append(k.to_map() if k else None)
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
         if self.spec is not None:
             result['Spec'] = self.spec
         if self.workspace_id is not None:
             result['WorkspaceId'] = self.workspace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Encryption') is not None:
+            temp_model = ListResourcesResponseBodyResourcesEncryption()
+            self.encryption = temp_model.from_map(m['Encryption'])
         if m.get('EnvType') is not None:
             self.env_type = m.get('EnvType')
-        self.executor = {}
         if m.get('Executor') is not None:
-            for k, v in m.get('Executor').items():
-                temp_model = ResourcesExecutorValue()
-                self.executor[k] = temp_model.from_map(v)
+            temp_model = ListResourcesResponseBodyResourcesExecutor()
+            self.executor = temp_model.from_map(m['Executor'])
         if m.get('GmtCreateTime') is not None:
             self.gmt_create_time = m.get('GmtCreateTime')
         if m.get('GroupName') is not None:
             self.group_name = m.get('GroupName')
         if m.get('Id') is not None:
             self.id = m.get('Id')
         if m.get('IsDefault') is not None:
@@ -7542,14 +7936,16 @@
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
         self.quotas = []
         if m.get('Quotas') is not None:
             for k in m.get('Quotas'):
                 temp_model = ListResourcesResponseBodyResourcesQuotas()
                 self.quotas.append(temp_model.from_map(k))
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
         if m.get('Spec') is not None:
             self.spec = m.get('Spec')
         if m.get('WorkspaceId') is not None:
             self.workspace_id = m.get('WorkspaceId')
         return self
 
 
@@ -7640,14 +8036,201 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListServiceTemplatesRequest(TeaModel):
+    def __init__(
+        self,
+        label: str = None,
+        order: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        provider: str = None,
+        query: str = None,
+        service_template_name: str = None,
+        sort_by: str = None,
+    ):
+        self.label = label
+        self.order = order
+        self.page_number = page_number
+        self.page_size = page_size
+        self.provider = provider
+        self.query = query
+        self.service_template_name = service_template_name
+        self.sort_by = sort_by
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.label is not None:
+            result['Label'] = self.label
+        if self.order is not None:
+            result['Order'] = self.order
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.provider is not None:
+            result['Provider'] = self.provider
+        if self.query is not None:
+            result['Query'] = self.query
+        if self.service_template_name is not None:
+            result['ServiceTemplateName'] = self.service_template_name
+        if self.sort_by is not None:
+            result['SortBy'] = self.sort_by
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Label') is not None:
+            self.label = m.get('Label')
+        if m.get('Order') is not None:
+            self.order = m.get('Order')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('Provider') is not None:
+            self.provider = m.get('Provider')
+        if m.get('Query') is not None:
+            self.query = m.get('Query')
+        if m.get('ServiceTemplateName') is not None:
+            self.service_template_name = m.get('ServiceTemplateName')
+        if m.get('SortBy') is not None:
+            self.sort_by = m.get('SortBy')
+        return self
+
+
+class ListServiceTemplatesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        service_templates: List[ServiceTemplate] = None,
+        total_count: int = None,
+    ):
+        self.request_id = request_id
+        self.service_templates = service_templates
+        self.total_count = total_count
+
+    def validate(self):
+        if self.service_templates:
+            for k in self.service_templates:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['ServiceTemplates'] = []
+        if self.service_templates is not None:
+            for k in self.service_templates:
+                result['ServiceTemplates'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.service_templates = []
+        if m.get('ServiceTemplates') is not None:
+            for k in m.get('ServiceTemplates'):
+                temp_model = ServiceTemplate()
+                self.service_templates.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListServiceTemplatesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListServiceTemplatesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListServiceTemplatesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListWorkspaceUsersRequest(TeaModel):
+    def __init__(
+        self,
+        user_name: str = None,
+    ):
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
 class ListWorkspaceUsersResponseBodyUsers(TeaModel):
     def __init__(
         self,
         user_id: str = None,
         user_name: str = None,
     ):
         self.user_id = user_id
@@ -8689,22 +9272,24 @@
     def __init__(
         self,
         accessibility: str = None,
         domain: str = None,
         model_description: str = None,
         model_doc: str = None,
         model_name: str = None,
+        order_number: int = None,
         origin: str = None,
         task: str = None,
     ):
         self.accessibility = accessibility
         self.domain = domain
         self.model_description = model_description
         self.model_doc = model_doc
         self.model_name = model_name
+        self.order_number = order_number
         self.origin = origin
         self.task = task
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -8719,14 +9304,16 @@
             result['Domain'] = self.domain
         if self.model_description is not None:
             result['ModelDescription'] = self.model_description
         if self.model_doc is not None:
             result['ModelDoc'] = self.model_doc
         if self.model_name is not None:
             result['ModelName'] = self.model_name
+        if self.order_number is not None:
+            result['OrderNumber'] = self.order_number
         if self.origin is not None:
             result['Origin'] = self.origin
         if self.task is not None:
             result['Task'] = self.task
         return result
 
     def from_map(self, m: dict = None):
@@ -8737,14 +9324,16 @@
             self.domain = m.get('Domain')
         if m.get('ModelDescription') is not None:
             self.model_description = m.get('ModelDescription')
         if m.get('ModelDoc') is not None:
             self.model_doc = m.get('ModelDoc')
         if m.get('ModelName') is not None:
             self.model_name = m.get('ModelName')
+        if m.get('OrderNumber') is not None:
+            self.order_number = m.get('OrderNumber')
         if m.get('Origin') is not None:
             self.origin = m.get('Origin')
         if m.get('Task') is not None:
             self.task = m.get('Task')
         return self
 
 
@@ -8820,22 +9409,24 @@
 
 
 class UpdateModelVersionRequest(TeaModel):
     def __init__(
         self,
         approval_status: str = None,
         inference_spec: Dict[str, Any] = None,
+        metrics: Dict[str, Any] = None,
         options: str = None,
         source_id: str = None,
         source_type: str = None,
         training_spec: Dict[str, Any] = None,
         version_description: str = None,
     ):
         self.approval_status = approval_status
         self.inference_spec = inference_spec
+        self.metrics = metrics
         self.options = options
         self.source_id = source_id
         self.source_type = source_type
         self.training_spec = training_spec
         self.version_description = version_description
 
     def validate(self):
@@ -8847,14 +9438,16 @@
             return _map
 
         result = dict()
         if self.approval_status is not None:
             result['ApprovalStatus'] = self.approval_status
         if self.inference_spec is not None:
             result['InferenceSpec'] = self.inference_spec
+        if self.metrics is not None:
+            result['Metrics'] = self.metrics
         if self.options is not None:
             result['Options'] = self.options
         if self.source_id is not None:
             result['SourceId'] = self.source_id
         if self.source_type is not None:
             result['SourceType'] = self.source_type
         if self.training_spec is not None:
@@ -8865,14 +9458,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApprovalStatus') is not None:
             self.approval_status = m.get('ApprovalStatus')
         if m.get('InferenceSpec') is not None:
             self.inference_spec = m.get('InferenceSpec')
+        if m.get('Metrics') is not None:
+            self.metrics = m.get('Metrics')
         if m.get('Options') is not None:
             self.options = m.get('Options')
         if m.get('SourceId') is not None:
             self.source_id = m.get('SourceId')
         if m.get('SourceType') is not None:
             self.source_type = m.get('SourceType')
         if m.get('TrainingSpec') is not None:
@@ -9059,18 +9654,20 @@
 
 class UpdateWorkspaceResourceRequest(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         is_default: bool = None,
         product_type: str = None,
+        resource_type: str = None,
     ):
         self.group_name = group_name
         self.is_default = is_default
         self.product_type = product_type
+        self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -9079,24 +9676,28 @@
         result = dict()
         if self.group_name is not None:
             result['GroupName'] = self.group_name
         if self.is_default is not None:
             result['IsDefault'] = self.is_default
         if self.product_type is not None:
             result['ProductType'] = self.product_type
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('GroupName') is not None:
             self.group_name = m.get('GroupName')
         if m.get('IsDefault') is not None:
             self.is_default = m.get('IsDefault')
         if m.get('ProductType') is not None:
             self.product_type = m.get('ProductType')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
         return self
 
 
 class UpdateWorkspaceResourceResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
```

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO` & `alibabacloud_aiworkspace20210204-2.0.0/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiworkspace20210204
-Version: 1.2.9
+Version: 2.0.0
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-1.2.9/setup.py` & `alibabacloud_aiworkspace20210204-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiworkspace20210204.
 
-Created on 13/03/2023
+Created on 08/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiworkspace20210204"
 NAME = "alibabacloud_aiworkspace20210204" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```


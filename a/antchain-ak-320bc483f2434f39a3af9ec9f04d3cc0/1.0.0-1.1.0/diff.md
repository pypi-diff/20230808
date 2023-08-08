# Comparing `tmp/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0.tar.gz` & `tmp/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0.tar", last modified: Tue Jul 25 12:21:02 2023, max compression
+gzip compressed data, was "dist/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0.tar", last modified: Tue Aug  8 10:00:53 2023, max compression
```

## Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0.tar` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:21:02.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-25 12:21:02.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:21:02.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:21:02.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23502 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/client.py
--rw-r--r--   0 root         (0) root         (0)    35427 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-25 12:21:02.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2023-07-25 12:21:01.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:00:53.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-08 10:00:53.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:00:53.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:00:53.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23502 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/client.py
+-rw-r--r--   0 root         (0) root         (0)    36133 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-08 10:00:53.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-08-08 10:00:52.000000 antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/setup.py
```

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/LICENSE` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/PKG-INFO` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0
-Version: 1.0.0
+Version: 1.1.0
 Summary: Ant Chain Ak_320bc483f2434f39a3af9ec9f04d3cc0 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/README-CN.md` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/README.md` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/PKG-INFO` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-320bc483f2434f39a3af9ec9f04d3cc0
-Version: 1.0.0
+Version: 1.1.0
 Summary: Ant Chain Ak_320bc483f2434f39a3af9ec9f04d3cc0 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/SOURCES.txt` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/client.py` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'ak_320bc483f2434f39a3af9ec9f04d3cc0',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.1.0',
                     '_prod_code': 'ak_320bc483f2434f39a3af9ec9f04d3cc0',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/models.py` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,54 +484,54 @@
 
 
 class SignAntsaasStaffingcContractSendRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        out_biz_no: str = None,
         file_object: BinaryIO = None,
         file_object_name: str = None,
         file_id: str = None,
-        contract_file: str = None,
         contract_type: int = None,
         contract_name: str = None,
         contract_file_type: str = None,
         simple_form_fields: str = None,
         sign_platform: str = None,
         sign_user_list: List[SignUserInfo] = None,
         sign_enterprise_list: List[SignEnterpriseInfo] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 需要确保唯一（定位订单）
+        self.out_biz_no = out_biz_no
         # 合同或模版文件
         # 待上传文件
         self.file_object = file_object
         # 待上传文件名
         self.file_object_name = file_object_name
         self.file_id = file_id
-        # 合同文件（base64格式）
-        self.contract_file = contract_file
         # 合同类型（1合同文件 2合同模板）
         self.contract_type = contract_type
-        # 合同名称
+        # 合同名称, 必须带上文件名后缀。 .dpf .doc .docx
         self.contract_name = contract_name
         # 合同文件类型 （pdf、word）
         self.contract_file_type = contract_file_type
         # 合同模版参数，json格式，以key value格式存储，合同类型属于模板必填
         self.simple_form_fields = simple_form_fields
         # 签署平台（ALIPAY或H5）
         self.sign_platform = sign_platform
         # 合同用户信息列表
         self.sign_user_list = sign_user_list
         # 合同企业信息列表
         self.sign_enterprise_list = sign_enterprise_list
 
     def validate(self):
-        self.validate_required(self.contract_file, 'contract_file')
+        self.validate_required(self.out_biz_no, 'out_biz_no')
         self.validate_required(self.contract_type, 'contract_type')
         self.validate_required(self.contract_name, 'contract_name')
         self.validate_required(self.contract_file_type, 'contract_file_type')
         self.validate_required(self.sign_platform, 'sign_platform')
         self.validate_required(self.sign_user_list, 'sign_user_list')
         if self.sign_user_list:
             for k in self.sign_user_list:
@@ -549,22 +549,22 @@
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.out_biz_no is not None:
+            result['out_biz_no'] = self.out_biz_no
         if self.file_object is not None:
             result['fileObject'] = self.file_object
         if self.file_object_name is not None:
             result['fileObjectName'] = self.file_object_name
         if self.file_id is not None:
             result['file_id'] = self.file_id
-        if self.contract_file is not None:
-            result['contract_file'] = self.contract_file
         if self.contract_type is not None:
             result['contract_type'] = self.contract_type
         if self.contract_name is not None:
             result['contract_name'] = self.contract_name
         if self.contract_file_type is not None:
             result['contract_file_type'] = self.contract_file_type
         if self.simple_form_fields is not None:
@@ -583,22 +583,22 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('out_biz_no') is not None:
+            self.out_biz_no = m.get('out_biz_no')
         if m.get('fileObject') is not None:
             self.file_object = m.get('fileObject')
         if m.get('fileObjectName') is not None:
             self.file_object_name = m.get('fileObjectName')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
-        if m.get('contract_file') is not None:
-            self.contract_file = m.get('contract_file')
         if m.get('contract_type') is not None:
             self.contract_type = m.get('contract_type')
         if m.get('contract_name') is not None:
             self.contract_name = m.get('contract_name')
         if m.get('contract_file_type') is not None:
             self.contract_file_type = m.get('contract_file_type')
         if m.get('simple_form_fields') is not None:
@@ -721,14 +721,15 @@
         flow_desc: str = None,
         flow_start_time: str = None,
         flow_end_time: str = None,
         flow_status: int = None,
         file_id: str = None,
         file_name: str = None,
         file_url: str = None,
+        sign_url_list: List[SignUrlResp] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
@@ -746,17 +747,22 @@
         self.flow_status = flow_status
         # 合同文件id
         self.file_id = file_id
         # 合同文件名称
         self.file_name = file_name
         # 合同文件下载地址（1小时内有效）
         self.file_url = file_url
+        # 如果未签署，将返回签署链接
+        self.sign_url_list = sign_url_list
 
     def validate(self):
-        pass
+        if self.sign_url_list:
+            for k in self.sign_url_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -780,14 +786,18 @@
             result['flow_status'] = self.flow_status
         if self.file_id is not None:
             result['file_id'] = self.file_id
         if self.file_name is not None:
             result['file_name'] = self.file_name
         if self.file_url is not None:
             result['file_url'] = self.file_url
+        result['sign_url_list'] = []
+        if self.sign_url_list is not None:
+            for k in self.sign_url_list:
+                result['sign_url_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -808,14 +818,19 @@
             self.flow_status = m.get('flow_status')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
         if m.get('file_name') is not None:
             self.file_name = m.get('file_name')
         if m.get('file_url') is not None:
             self.file_url = m.get('file_url')
+        self.sign_url_list = []
+        if m.get('sign_url_list') is not None:
+            for k in m.get('sign_url_list'):
+                temp_model = SignUrlResp()
+                self.sign_url_list.append(temp_model.from_map(k))
         return self
 
 
 class CreateAntcloudGatewayxFileUploadRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.0.0/setup.py` & `antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0.
 
-Created on 25/07/2023
+Created on 08/08/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_320bc483f2434f39a3af9ec9f04d3cc0"
 NAME = "antchain_ak_320bc483f2434f39a3af9ec9f04d3cc0" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_320bc483f2434f39a3af9ec9f04d3cc0 SDK Library for Python"
```


# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.952.tar", last modified: Mon Aug  7 08:53:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.953.tar", last modified: Tue Aug  8 00:24:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.952.tar` & `tencentcloud-sdk-python-essbasic-3.0.953.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    57594 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   393411 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      733 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:53:47.000000 tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    57837 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   394018 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      733 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:24:58.000000 tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.953/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-essbasic',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Essbasic SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeFlowComponents(self, request):
-        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
+        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息和填写内容。 注意：使用此接口前，需要在【企业应用管理】-【应用集成】-【第三方应用管理】中开通【下载应用内全量合同文件及内容数据】功能。
 
         :param request: Request instance for ChannelDescribeFlowComponents.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeFlowComponentsRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeFlowComponentsResponse`
 
         """
         try:
@@ -623,15 +623,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelDescribeOrganizationSeals(self, request):
         """查询子客企业电子印章，需要操作者具有管理印章权限
-        客户指定需要获取的印章数量和偏移量，数量最多100，超过100按100处理；入参InfoType控制印章是否携带授权人信息，为1则携带，为0则返回的授权人信息为空数组。接口调用成功返回印章的信息列表还有企业印章的总数。
+        客户指定需要获取的印章数量和偏移量，数量最多100，超过100按100处理；入参InfoType控制印章是否携带授权人信息，为1则携带，为0则返回的授权人信息为空数组。接口调用成功返回印章的信息列表还有企业印章的总数，只返回启用的印章。
 
         :param request: Request instance for ChannelDescribeOrganizationSeals.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeOrganizationSealsRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeOrganizationSealsResponse`
 
         """
         try:
@@ -716,15 +716,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def ChannelVerifyPdf(self, request):
-        """对流程的合同文件进行验证，判断文件是否合法。
+        """对流程的合同文件进行数字签名验证，判断文件是否被篡改。
 
         :param request: Request instance for ChannelVerifyPdf.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelVerifyPdfRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelVerifyPdfResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3165,19 +3165,19 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param _RoleIds: 绑定角色的角色id列表
+        :param _RoleIds: 绑定角色的角色id列表，最多 100 个
         :type RoleIds: list of str
-        :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
+        :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数，最多 100 个
         :type UserIds: list of str
-        :param _OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数
+        :param _OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数，最多 100 个
         :type OpenIds: list of str
         :param _Operator: 操作者信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
         self._RoleIds = None
         self._UserIds = None
@@ -3385,19 +3385,19 @@
 
     def __init__(self):
         r"""
         :param _Agent: 代理信息此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _RoleId: 角色Id（非超管或法人角色Id）
         :type RoleId: str
-        :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
+        :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数，最多两百
         :type UserIds: list of str
         :param _Operator: 操作人信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
-        :param _OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数
+        :param _OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数，最多两百
         :type OpenIds: list of str
         """
         self._Agent = None
         self._RoleId = None
         self._UserIds = None
         self._Operator = None
         self._OpenIds = None
@@ -3628,50 +3628,50 @@
 class ChannelDescribeEmployeesRequest(AbstractModel):
     """ChannelDescribeEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Limit: 返回最大数量，最大为20
-        :type Limit: int
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
+        :param _Limit: 指定每页多少条数据，单页最大20
+        :type Limit: int
         :param _Filters: 查询过滤实名用户，Key为Status，Values为["IsVerified"]
 根据第三方系统openId过滤查询员工时,Key为StaffOpenId,Values为["OpenId","OpenId",...]
 查询离职员工时，Key为Status，Values为["QuiteJob"]
         :type Filters: list of Filter
-        :param _Offset: 偏移量，默认为0，最大为20000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0,最大为20000
         :type Offset: int
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
-        self._Limit = None
         self._Agent = None
+        self._Limit = None
         self._Filters = None
         self._Offset = None
         self._Operator = None
 
     @property
-    def Limit(self):
-        return self._Limit
-
-    @Limit.setter
-    def Limit(self, Limit):
-        self._Limit = Limit
-
-    @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
         self._Agent = Agent
 
     @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+    @property
     def Filters(self):
         return self._Filters
 
     @Filters.setter
     def Filters(self, Filters):
         self._Filters = Filters
 
@@ -3693,18 +3693,18 @@
     def Operator(self, Operator):
         warnings.warn("parameter `Operator` is deprecated", DeprecationWarning) 
 
         self._Operator = Operator
 
 
     def _deserialize(self, params):
-        self._Limit = params.get("Limit")
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
+        self._Limit = params.get("Limit")
         if params.get("Filters") is not None:
             self._Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self._Filters.append(obj)
         self._Offset = params.get("Offset")
@@ -3727,18 +3727,18 @@
     """
 
     def __init__(self):
         r"""
         :param _Employees: 员工数据列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type Employees: list of Staff
-        :param _Offset: 偏移量，默认为0，最大为20000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大20000
 注意：此字段可能返回 null，表示取不到有效值。
         :type Offset: int
-        :param _Limit: 返回最大数量，最大为20
+        :param _Limit: 指定每页多少条数据，单页最大20
         :type Limit: int
         :param _TotalCount: 符合条件的员工数量
         :type TotalCount: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Employees = None
@@ -3851,15 +3851,15 @@
 class ChannelDescribeFlowComponentsResponse(AbstractModel):
     """ChannelDescribeFlowComponents返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _RecipientComponentInfos: 流程关联的填写控件信息
+        :param _RecipientComponentInfos: 流程关联的填写控件信息，控件会按照参与方进行分类。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecipientComponentInfos: list of RecipientComponentInfo
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._RecipientComponentInfos = None
         self._RequestId = None
@@ -4051,17 +4051,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param _Offset: 查询起始偏移，最大2000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大2000
         :type Offset: int
-        :param _Limit: 查询数量，最大200
+        :param _Limit: 指定每页多少条数据，单页最大200
         :type Limit: str
         :param _Filters: 查询的关键字段:
 Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
 Key:"RoleStatus",Values:["1"]查询启用角色，Values:["2"]查询禁用角色
         :type Filters: list of Filter
         :param _Operator: 操作人信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -4145,17 +4145,17 @@
 class ChannelDescribeRolesResponse(AbstractModel):
     """ChannelDescribeRoles返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Offset: 页面偏移量，最大2000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大2000
         :type Offset: int
-        :param _Limit: 查询数量，最大200
+        :param _Limit: 指定每页多少条数据，单页最大200
         :type Limit: int
         :param _TotalCount: 查询角色的总数量
         :type TotalCount: int
         :param _ChannelRoles: 角色信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelRoles: list of ChannelRole
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.952'
+__version__ = '3.0.953'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.953/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.952/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.953/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


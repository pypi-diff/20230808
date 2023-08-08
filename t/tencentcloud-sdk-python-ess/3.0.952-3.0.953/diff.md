# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.952.tar", last modified: Mon Aug  7 08:53:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.953.tar", last modified: Tue Aug  8 00:24:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.952.tar` & `tencentcloud-sdk-python-ess-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    67169 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25058 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   478228 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 08:53:40.000000 tencentcloud-sdk-python-ess-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    68335 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25058 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   479921 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:24:54.000000 tencentcloud-sdk-python-ess-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/setup.py` & `tencentcloud-sdk-python-ess-3.0.953/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ess',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ess SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateConvertTaskApi(self, request):
         """上传了word、excel、图片文件后，通过该接口发起文件转换任务，将word、excel、图片文件转换为pdf文件。
+        注：如果是集团代子企业发起任务场景，可以通过对Agent参数（未列在入参列表）设置代理的相关应用信息来支持，Agent参数设置可以参考CreateFlow接口的Agent相关说明。
 
         :param request: Request instance for CreateConvertTaskApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateConvertTaskApiResponse`
 
         """
         try:
@@ -500,15 +501,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def CreateIntegrationEmployees(self, request):
-        """创建员工,此接口会发送提醒员工实名的短信
+        """创建员工,此接口会发送提醒员工实名的短信，如果通过手机号发现员工已经创建，则不会重新创建，会发送短信提醒员工实名
+        注意：此接口支持企微组织架构的 openid 创建员工，这种场景下传递明文的企微 openid 到WeworkOpenId字段即可（企微明文的 openid 一定要在应用的可见范围内才行），通过企微创建的员工，会发送企微消息去提醒实名
 
         :param request: Request instance for CreateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesResponse`
 
         """
         try:
@@ -844,14 +846,17 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DeleteIntegrationEmployees(self, request):
         """移除员工
+        这里分两个场景
+        如果不传交接人的ReceiveUserId或者ReceiveOpenId，则会直接把这个人进行离职
+        如果传了交接人，会把离职人未处理完的合同交接给交接人后再离职
 
         :param request: Request instance for DeleteIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationEmployeesResponse`
 
         """
         try:
@@ -984,15 +989,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeFlowComponents(self, request):
-        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
+        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息和填写内容。
+        注意：使用此接口前，需要在【企业应用管理】-【应用集成】-【第三方应用管理】中开通【下载应用内全量合同文件及内容数据】功能。
 
         :param request: Request instance for DescribeFlowComponents.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowComponentsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowComponentsResponse`
 
         """
         try:
@@ -1160,15 +1166,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeIntegrationRoles(self, request):
-        """查询企业角色列表
+        """分页查询企业角色列表，法人的角色是系统保留角色，不会返回，按照角色创建时间升序排列
 
         :param request: Request instance for DescribeIntegrationRoles.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationRolesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationRolesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.952/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.953/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4452,17 +4452,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _UserIds: 绑定角色的用户id列表
+        :param _UserIds: 绑定角色的用户id列表，不能重复，不能大于 100 个
         :type UserIds: list of str
-        :param _RoleIds: 绑定角色的角色id列表
+        :param _RoleIds: 绑定角色的角色id列表，不能重复，不能大于 100，可以通过DescribeIntegrationRoles接口获取
         :type RoleIds: list of str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._UserIds = None
         self._RoleIds = None
@@ -5393,27 +5393,30 @@
 取值：false：不做任何处理；
 true：做透明化处理和颜色增强。
         :type ProcessSeal: bool
         :param _FileId: 印章图片文件 id
 取值：
 填写的FileId通过UploadFiles接口上传文件获取。
         :type FileId: str
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._UserName = None
         self._IdCardNumber = None
         self._SealName = None
         self._Operator = None
         self._IdCardType = None
         self._SealImage = None
         self._SealImageCompress = None
         self._Mobile = None
         self._EnableAutoSign = None
         self._SealColor = None
         self._ProcessSeal = None
         self._FileId = None
+        self._Agent = None
 
     @property
     def UserName(self):
         return self._UserName
 
     @UserName.setter
     def UserName(self, UserName):
@@ -5507,14 +5510,22 @@
     def FileId(self):
         return self._FileId
 
     @FileId.setter
     def FileId(self, FileId):
         self._FileId = FileId
 
+    @property
+    def Agent(self):
+        return self._Agent
+
+    @Agent.setter
+    def Agent(self, Agent):
+        self._Agent = Agent
+
 
     def _deserialize(self, params):
         self._UserName = params.get("UserName")
         self._IdCardNumber = params.get("IdCardNumber")
         self._SealName = params.get("SealName")
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
@@ -5523,14 +5534,17 @@
         self._SealImage = params.get("SealImage")
         self._SealImageCompress = params.get("SealImageCompress")
         self._Mobile = params.get("Mobile")
         self._EnableAutoSign = params.get("EnableAutoSign")
         self._SealColor = params.get("SealColor")
         self._ProcessSeal = params.get("ProcessSeal")
         self._FileId = params.get("FileId")
+        if params.get("Agent") is not None:
+            self._Agent = Agent()
+            self._Agent._deserialize(params.get("Agent"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5729,38 +5743,44 @@
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _OrganizationName: 企业名称
         :type OrganizationName: str
         :param _Name: 姓名,最大长度50个字符
         :type Name: str
         :param _Mobile: 手机号，大陆手机号11位
         :type Mobile: str
-        :param _EndPoint: 链接类型
-HTTP：跳转电子签小程序的http_url，
-APP：第三方APP或小程序跳转电子签小程序的path。
-默认为HTTP类型
+        :param _EndPoint: 要跳转的链接类型
+
+- HTTP：跳转电子签小程序的http_url, 短信通知或者H5跳转适合此类型  (默认)
+- APP： 第三方APP或小程序跳转电子签小程序的path,  APP或者小程序跳转适合此类型
+
         :type EndPoint: str
         :param _FlowId: 签署流程编号 (PathType=1时必传)
         :type FlowId: str
         :param _FlowGroupId: 合同组ID 
         :type FlowGroupId: str
-        :param _PathType: 跳转页面 1: 小程序合同详情 2: 小程序合同列表页 0: 不传, 默认主页
+        :param _PathType: 要跳转到的页面类型 
+
+- 0: 不传, 主页 (默认)
+- 1: 小程序合同详情 
+- 2: 小程序合同列表页 
+
         :type PathType: int
         :param _AutoJumpBack: 是否自动回跳
 true：是，
 false：否。
 该参数只针对"APP" 类型的签署链接有效
         :type AutoJumpBack: bool
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Hides: 生成的签署链接在签署过程隐藏的按钮列表, 可以设置隐藏的按钮列表如下
 
-0:合同签署页面更多操作按钮
-1:合同签署页面更多操作的拒绝签署按钮
-2:合同签署页面更多操作的转他人处理按钮
-3:签署成功页的查看详情按钮
+- 0:合同签署页面更多操作按钮
+- 1:合同签署页面更多操作的拒绝签署按钮
+- 2:合同签署页面更多操作的转他人处理按钮
+- 3:签署成功页的查看详情按钮
         :type Hides: list of int
         """
         self._Operator = None
         self._OrganizationName = None
         self._Name = None
         self._Mobile = None
         self._EndPoint = None
@@ -6686,15 +6706,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _DeptId: 电子签中的部门id
+        :param _DeptId: 电子签中的部门id,通过DescribeIntegrationDepartments接口可获得
         :type DeptId: str
         :param _ReceiveDeptId: 交接部门ID。待删除部门中的合同、印章和模板数据，交接至该部门ID下，未填写交接至公司根部门。
         :type ReceiveDeptId: str
         """
         self._Operator = None
         self._DeptId = None
         self._ReceiveDeptId = None
@@ -6770,15 +6790,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _Employees: 待移除员工的信息，userId和openId二选一，必填一个
+        :param _Employees: 待移除员工的信息，userId和openId二选一，必填一个，如果需要指定交接人的话，ReceiveUserId或者ReceiveOpenId字段二选一
         :type Employees: list of Staff
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._Employees = None
         self._Agent = None
@@ -6877,15 +6897,15 @@
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _RoleId: 角色id
         :type RoleId: str
-        :param _Users: 用户信息
+        :param _Users: 用户信息,最多 200 个用户，并且 UserId 和 OpenId 二选一，其他字段不需要传
         :type Users: list of UserInfo
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._RoleId = None
         self._Users = None
@@ -7642,17 +7662,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作者信息
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _FlowId: 电子签流程的Id
+        :param _FlowId: 流程(合同)的编号
         :type FlowId: str
-        :param _Agent: 应用相关信息
+        :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         """
         self._Operator = None
         self._FlowId = None
         self._Agent = None
 
     @property
@@ -7701,15 +7721,15 @@
 class DescribeFlowComponentsResponse(AbstractModel):
     """DescribeFlowComponents返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _RecipientComponentInfos: 流程关联的填写控件信息
+        :param _RecipientComponentInfos: 流程关联的填写控件信息，按照参与方进行分类返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecipientComponentInfos: list of RecipientComponentInfo
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._RecipientComponentInfos = None
         self._RequestId = None
@@ -8346,22 +8366,22 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _Limit: 返回最大数量，最大为20
+        :param _Limit: 指定每页多少条数据，单页最大20
         :type Limit: int
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Filters: 查询过滤实名用户，Key为Status，Values为["IsVerified"]
 根据第三方系统openId过滤查询员工时,Key为StaffOpenId,Values为["OpenId","OpenId",...]
         :type Filters: list of Filter
-        :param _Offset: 偏移量，默认为0，最大为20000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大20000
         :type Offset: int
         """
         self._Operator = None
         self._Limit = None
         self._Agent = None
         self._Filters = None
         self._Offset = None
@@ -8438,18 +8458,18 @@
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
@@ -8592,24 +8612,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _Limit: 返回最大数量，最大为200
+        :param _Limit: 指定每页多少条数据，单页最大200
         :type Limit: int
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _Filters: 查询的关键字段:
 Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
 Key:"RoleStatus",Values:["1"]查询启用角色，Values:["2"]查询禁用角色
 Key:"IsGroupRole"，Values:["0"],查询非集团角色，Values:["1"]表示查询集团角色
         :type Filters: list of Filter
-        :param _Offset: 偏移量，默认为0，最大为2000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大2000
         :type Offset: int
         """
         self._Operator = None
         self._Limit = None
         self._Agent = None
         self._Filters = None
         self._Offset = None
@@ -8683,17 +8703,17 @@
 class DescribeIntegrationRolesResponse(AbstractModel):
     """DescribeIntegrationRoles返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Offset: 偏移量，默认为0，最大为2000
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0，最大2000
         :type Offset: int
-        :param _Limit: 返回最大数量，最大为200
+        :param _Limit: 指定每页多少条数据，单页最大200
         :type Limit: int
         :param _TotalCount: 符合查询条件的总的角色数
         :type TotalCount: int
         :param _IntegrateRoles: 企业角色信息列表
         :type IntegrateRoles: list of IntegrateRole
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -8763,25 +8783,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，userId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _Limit: 单次查询成员企业最大返回数量
+        :param _Limit: 指定每页多少条数据，单页最大1000
         :type Limit: int
-        :param _Offset: 页面偏移量
+        :param _Offset: 查询结果分页返回，此处指定第几页，如果不传默认从第一页返回。页码从 0 开始，即首页为 0
         :type Offset: int
         :param _Name: 查询成员企业的企业名，模糊匹配
         :type Name: str
         :param _Status: 成员企业加入集团的当前状态:1-待授权;2-已授权待激活;3-拒绝授权;4-已解除;5-已加入
         :type Status: int
         :param _Export: 是否导出当前成员企业数据
         :type Export: bool
-        :param _Id: 成员企业id
+        :param _Id: 成员企业机构 ID，在PC控制台 集团管理可获取
         :type Id: str
         """
         self._Operator = None
         self._Limit = None
         self._Offset = None
         self._Name = None
         self._Status = None
@@ -8877,15 +8897,15 @@
         :type Total: int
         :param _JoinedTotal: 已授权待激活的企业数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type JoinedTotal: int
         :param _ActivedTotal: 已加入的企业数量(废弃,请使用ActivatedTotal)
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActivedTotal: int
-        :param _ExportUrl: 导出文件的url
+        :param _ExportUrl: 如果入参Export为 true 时使用，表示导出Excel的url
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExportUrl: str
         :param _List: 成员企业信息列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type List: list of GroupOrganization
         :param _ActivatedTotal: 已加入的企业数量
 注意：此字段可能返回 null，表示取不到有效值。
@@ -11912,15 +11932,15 @@
         :type License: str
         :param _LicenseExpireTime: 企业许可证过期时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type LicenseExpireTime: int
         :param _JoinTime: 成员企业加入集团时间，时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type JoinTime: int
-        :param _FlowEngineEnable: 是否使用审批流引擎，true-是，false-否
+        :param _FlowEngineEnable: 是否使用自建审批流引擎（即不是企微审批流引擎），true-是，false-否
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowEngineEnable: bool
         """
         self._Name = None
         self._Alias = None
         self._OrganizationId = None
         self._UpdateTime = None
@@ -12441,17 +12461,17 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
-        :param _DeptId: 电子签部门ID
+        :param _DeptId: 电子签部门ID,通过DescribeIntegrationDepartments接口可以获取
         :type DeptId: str
-        :param _ParentDeptId: 电子签父部门ID
+        :param _ParentDeptId: 电子签父部门ID，通过DescribeIntegrationDepartments接口可以获取
         :type ParentDeptId: str
         :param _DeptName: 部门名称，不超过50个字符
         :type DeptName: str
         :param _DeptOpenId: 客户系统部门ID，不超过64个字符
         :type DeptOpenId: str
         :param _OrderNo: 排序号,1~30000范围内
         :type OrderNo: int
@@ -13188,20 +13208,22 @@
 
     def __init__(self):
         r"""
         :param _RecipientId: 参与方Id
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecipientId: str
         :param _RecipientFillStatus: 参与方填写状态
+0-未填写
+1-已填写
 注意：此字段可能返回 null，表示取不到有效值。
         :type RecipientFillStatus: str
-        :param _IsPromoter: 是否发起方
+        :param _IsPromoter: 是否为发起方
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsPromoter: bool
-        :param _Components: 填写控件内容
+        :param _Components: 填写控件列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type Components: list of FilledComponent
         """
         self._RecipientId = None
         self._RecipientFillStatus = None
         self._IsPromoter = None
         self._Components = None
@@ -14821,15 +14843,15 @@
 class UpdateIntegrationEmployeesRequest(AbstractModel):
     """UpdateIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Operator: 当前用户信息，OpenId与UserId二选一必填一个，OpenId是第三方客户ID，userId是用户实名后的电子签生成的ID,当传入客户系统openId，传入的openId需与电子签员工userId绑定，且参数Channel必填，Channel值为YUFU；
+        :param _Operator: 当前用户信息，UserId必填
         :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
         :param _Employees: 员工信息，不超过100个。
 根据UserId或OpenId更新员工，必填一个，优先UserId。
 可更新Mobile、DisplayName、Email和Department.DepartmentId字段，其他字段暂不支持
         :type Employees: list of Staff
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId需填充子企业Id
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.953/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.952/README.rst` & `tencentcloud-sdk-python-ess-3.0.953/README.rst`

 * *Files identical despite different names*


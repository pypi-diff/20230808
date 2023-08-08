# Comparing `tmp/tencentcloud-sdk-python-iss-3.0.951.tar.gz` & `tmp/tencentcloud-sdk-python-iss-3.0.952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iss-3.0.951.tar", last modified: Mon Aug  7 00:29:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iss-3.0.952.tar", last modified: Mon Aug  7 08:56:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iss-3.0.951.tar` & `tencentcloud-sdk-python-iss-3.0.952.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69487 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/iss_client.py
--rw-r--r--   0 root         (0) root         (0)    17413 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   355133 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 00:29:09.000000 tencentcloud-sdk-python-iss-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69487 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/iss_client.py
+-rw-r--r--   0 root         (0) root         (0)    17413 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   396571 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 08:56:18.000000 tencentcloud-sdk-python-iss-3.0.952/README.rst
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/setup.py` & `tencentcloud-sdk-python-iss-3.0.952/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-iss',
-    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Iss SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iss-3.0.952/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.951'
+__version__ = '3.0.952'
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/iss_client.py` & `tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/iss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/errorcodes.py` & `tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iss-3.0.951/tencentcloud/iss/v20230517/models.py` & `tencentcloud-sdk-python-iss-3.0.952/tencentcloud/iss/v20230517/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -210,14 +210,74 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AITaskResultData(AbstractModel):
+    """AI识别结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: AI 任务 ID
+        :type TaskId: str
+        :param _AIResultCount: 在 BeginTime 和 EndTime 时间之内，有识别结果的 AI 调用次数（分页依据此数值）
+        :type AIResultCount: int
+        :param _AIResults: AI 任务执行结果详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AIResults: :class:`tencentcloud.iss.v20230517.models.AITaskResultInfo`
+        """
+        self._TaskId = None
+        self._AIResultCount = None
+        self._AIResults = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
+    def AIResultCount(self):
+        return self._AIResultCount
+
+    @AIResultCount.setter
+    def AIResultCount(self, AIResultCount):
+        self._AIResultCount = AIResultCount
+
+    @property
+    def AIResults(self):
+        return self._AIResults
+
+    @AIResults.setter
+    def AIResults(self, AIResults):
+        self._AIResults = AIResults
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        self._AIResultCount = params.get("AIResultCount")
+        if params.get("AIResults") is not None:
+            self._AIResults = AITaskResultInfo()
+            self._AIResults._deserialize(params.get("AIResults"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AITaskResultInfo(AbstractModel):
     """AI分析结果详情
 
     """
 
     def __init__(self):
         r"""
@@ -375,74 +435,14 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AITaskResultResponse(AbstractModel):
-    """AI识别结果
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TaskId: AI 任务 ID
-        :type TaskId: str
-        :param _AIResultCount: 在 BeginTime 和 EndTime 时间之内，有识别结果的 AI 调用次数（分页依据此数值）
-        :type AIResultCount: int
-        :param _AIResults: AI 任务执行结果详情
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AIResults: :class:`tencentcloud.iss.v20230517.models.AITaskResultInfo`
-        """
-        self._TaskId = None
-        self._AIResultCount = None
-        self._AIResults = None
-
-    @property
-    def TaskId(self):
-        return self._TaskId
-
-    @TaskId.setter
-    def TaskId(self, TaskId):
-        self._TaskId = TaskId
-
-    @property
-    def AIResultCount(self):
-        return self._AIResultCount
-
-    @AIResultCount.setter
-    def AIResultCount(self, AIResultCount):
-        self._AIResultCount = AIResultCount
-
-    @property
-    def AIResults(self):
-        return self._AIResults
-
-    @AIResults.setter
-    def AIResults(self, AIResults):
-        self._AIResults = AIResults
-
-
-    def _deserialize(self, params):
-        self._TaskId = params.get("TaskId")
-        self._AIResultCount = params.get("AIResultCount")
-        if params.get("AIResults") is not None:
-            self._AIResults = AITaskResultInfo()
-            self._AIResults._deserialize(params.get("AIResults"))
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class AITemplates(AbstractModel):
     """AI模板信息
 
     """
 
     def __init__(self):
         r"""
@@ -634,15 +634,15 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = AITaskInfo()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class AddDeviceResponse(AbstractModel):
+class AddDeviceData(AbstractModel):
     """增加设备接口返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _DeviceId: 设备iD
@@ -890,15 +890,15 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AddOrgResponse(AbstractModel):
+class AddOrgData(AbstractModel):
     """增加组织接口返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _OrganizationId: 组织 ID
@@ -1068,15 +1068,15 @@
     """AddOrganization返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 增加组织接口返回数据
-        :type Data: :class:`tencentcloud.iss.v20230517.models.AddOrgResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddOrgData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -1094,120 +1094,20 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = AddOrgResponse()
+            self._Data = AddOrgData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class AddRecordBackupPlanRequest(AbstractModel):
-    """AddRecordBackupPlan请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TemplateId: 录制模板ID（录像计划关联的模板ID，从查询录像上云模板列表接口ListRecordBackupTemplates中获取）
-        :type TemplateId: str
-        :param _PlanName: 录像计划名称（仅支持中文、英文、数字、_、-，长度不超过32个字符，计划名称全局唯一，不能为空，不能重复）
-        :type PlanName: str
-        :param _Describe: 录像计划描述（仅支持中文、英文、数字、_、-，长度不超过128个字符）
-        :type Describe: str
-        :param _LifeCycle: 生命周期（录像文件生命周期设置，管理文件冷、热存储的时间）
-        :type LifeCycle: :class:`tencentcloud.iss.v20230517.models.LifeCycleData`
-        :param _Channels: 通道及通道所属设备（添加录像的设备的通道信息，一次添加通道总数不超过5000个，包括组织目录下的通道数量）
-        :type Channels: list of ChannelInfo
-        :param _OrganizationId: 添加组织目录下所有设备通道（Json数组，可以为空，通道总数量不超过5000个（包括Channel字段的数量））
-        :type OrganizationId: list of str
-        """
-        self._TemplateId = None
-        self._PlanName = None
-        self._Describe = None
-        self._LifeCycle = None
-        self._Channels = None
-        self._OrganizationId = None
-
-    @property
-    def TemplateId(self):
-        return self._TemplateId
-
-    @TemplateId.setter
-    def TemplateId(self, TemplateId):
-        self._TemplateId = TemplateId
-
-    @property
-    def PlanName(self):
-        return self._PlanName
-
-    @PlanName.setter
-    def PlanName(self, PlanName):
-        self._PlanName = PlanName
-
-    @property
-    def Describe(self):
-        return self._Describe
-
-    @Describe.setter
-    def Describe(self, Describe):
-        self._Describe = Describe
-
-    @property
-    def LifeCycle(self):
-        return self._LifeCycle
-
-    @LifeCycle.setter
-    def LifeCycle(self, LifeCycle):
-        self._LifeCycle = LifeCycle
-
-    @property
-    def Channels(self):
-        return self._Channels
-
-    @Channels.setter
-    def Channels(self, Channels):
-        self._Channels = Channels
-
-    @property
-    def OrganizationId(self):
-        return self._OrganizationId
-
-    @OrganizationId.setter
-    def OrganizationId(self, OrganizationId):
-        self._OrganizationId = OrganizationId
-
-
-    def _deserialize(self, params):
-        self._TemplateId = params.get("TemplateId")
-        self._PlanName = params.get("PlanName")
-        self._Describe = params.get("Describe")
-        if params.get("LifeCycle") is not None:
-            self._LifeCycle = LifeCycleData()
-            self._LifeCycle._deserialize(params.get("LifeCycle"))
-        if params.get("Channels") is not None:
-            self._Channels = []
-            for item in params.get("Channels"):
-                obj = ChannelInfo()
-                obj._deserialize(item)
-                self._Channels.append(obj)
-        self._OrganizationId = params.get("OrganizationId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class AddRecordBackupPlanResponse(AbstractModel):
+class AddRecordBackupPlanData(AbstractModel):
     """新增录像上云计划返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _PlanId: 录像上云计划ID
@@ -1320,96 +1220,164 @@
         if params.get("LifeCycle") is not None:
             self._LifeCycle = LifeCycleData()
             self._LifeCycle._deserialize(params.get("LifeCycle"))
         self._Status = params.get("Status")
         self._ChannelCount = params.get("ChannelCount")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class AddRecordBackupTemplateRequest(AbstractModel):
-    """AddRecordBackupTemplate请求参数结构体
+class AddRecordBackupPlanRequest(AbstractModel):
+    """AddRecordBackupPlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateName: 模板名称（仅支持中文、英文、数字、_、-，长度不超过32个字符，模板名称全局唯一，不能为空，不能重复）
-        :type TemplateName: str
-        :param _TimeSections: 上云时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
-        :type TimeSections: list of RecordTemplateTimeSections
-        :param _DevTimeSections: 录像时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
-        :type DevTimeSections: list of RecordTemplateTimeSections
-        :param _Scale: 上云倍速（支持1，2，4倍速）
-        :type Scale: int
+        :param _TemplateId: 录制模板ID（录像计划关联的模板ID，从查询录像上云模板列表接口ListRecordBackupTemplates中获取）
+        :type TemplateId: str
+        :param _PlanName: 录像计划名称（仅支持中文、英文、数字、_、-，长度不超过32个字符，计划名称全局唯一，不能为空，不能重复）
+        :type PlanName: str
+        :param _Describe: 录像计划描述（仅支持中文、英文、数字、_、-，长度不超过128个字符）
+        :type Describe: str
+        :param _LifeCycle: 生命周期（录像文件生命周期设置，管理文件冷、热存储的时间）
+        :type LifeCycle: :class:`tencentcloud.iss.v20230517.models.LifeCycleData`
+        :param _Channels: 通道及通道所属设备（添加录像的设备的通道信息，一次添加通道总数不超过5000个，包括组织目录下的通道数量）
+        :type Channels: list of ChannelInfo
+        :param _OrganizationId: 添加组织目录下所有设备通道（Json数组，可以为空，通道总数量不超过5000个（包括Channel字段的数量））
+        :type OrganizationId: list of str
         """
-        self._TemplateName = None
-        self._TimeSections = None
-        self._DevTimeSections = None
-        self._Scale = None
+        self._TemplateId = None
+        self._PlanName = None
+        self._Describe = None
+        self._LifeCycle = None
+        self._Channels = None
+        self._OrganizationId = None
 
     @property
-    def TemplateName(self):
-        return self._TemplateName
+    def TemplateId(self):
+        return self._TemplateId
 
-    @TemplateName.setter
-    def TemplateName(self, TemplateName):
-        self._TemplateName = TemplateName
+    @TemplateId.setter
+    def TemplateId(self, TemplateId):
+        self._TemplateId = TemplateId
 
     @property
-    def TimeSections(self):
-        return self._TimeSections
+    def PlanName(self):
+        return self._PlanName
 
-    @TimeSections.setter
-    def TimeSections(self, TimeSections):
-        self._TimeSections = TimeSections
+    @PlanName.setter
+    def PlanName(self, PlanName):
+        self._PlanName = PlanName
 
     @property
-    def DevTimeSections(self):
-        return self._DevTimeSections
+    def Describe(self):
+        return self._Describe
 
-    @DevTimeSections.setter
-    def DevTimeSections(self, DevTimeSections):
-        self._DevTimeSections = DevTimeSections
+    @Describe.setter
+    def Describe(self, Describe):
+        self._Describe = Describe
 
     @property
-    def Scale(self):
-        return self._Scale
+    def LifeCycle(self):
+        return self._LifeCycle
 
-    @Scale.setter
-    def Scale(self, Scale):
-        self._Scale = Scale
+    @LifeCycle.setter
+    def LifeCycle(self, LifeCycle):
+        self._LifeCycle = LifeCycle
+
+    @property
+    def Channels(self):
+        return self._Channels
+
+    @Channels.setter
+    def Channels(self, Channels):
+        self._Channels = Channels
+
+    @property
+    def OrganizationId(self):
+        return self._OrganizationId
+
+    @OrganizationId.setter
+    def OrganizationId(self, OrganizationId):
+        self._OrganizationId = OrganizationId
 
 
     def _deserialize(self, params):
-        self._TemplateName = params.get("TemplateName")
-        if params.get("TimeSections") is not None:
-            self._TimeSections = []
-            for item in params.get("TimeSections"):
-                obj = RecordTemplateTimeSections()
-                obj._deserialize(item)
-                self._TimeSections.append(obj)
-        if params.get("DevTimeSections") is not None:
-            self._DevTimeSections = []
-            for item in params.get("DevTimeSections"):
-                obj = RecordTemplateTimeSections()
+        self._TemplateId = params.get("TemplateId")
+        self._PlanName = params.get("PlanName")
+        self._Describe = params.get("Describe")
+        if params.get("LifeCycle") is not None:
+            self._LifeCycle = LifeCycleData()
+            self._LifeCycle._deserialize(params.get("LifeCycle"))
+        if params.get("Channels") is not None:
+            self._Channels = []
+            for item in params.get("Channels"):
+                obj = ChannelInfo()
                 obj._deserialize(item)
-                self._DevTimeSections.append(obj)
-        self._Scale = params.get("Scale")
+                self._Channels.append(obj)
+        self._OrganizationId = params.get("OrganizationId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AddRecordBackupTemplateResponse(AbstractModel):
+class AddRecordBackupPlanResponse(AbstractModel):
+    """AddRecordBackupPlan返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddRecordBackupPlanData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = AddRecordBackupPlanData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class AddRecordBackupTemplateData(AbstractModel):
     """新增录像上云模版返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _TemplateId: 模板ID
@@ -1513,14 +1481,140 @@
             for item in params.get("DevTimeSections"):
                 obj = RecordTemplateTimeSections()
                 obj._deserialize(item)
                 self._DevTimeSections.append(obj)
         self._Scale = params.get("Scale")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddRecordBackupTemplateRequest(AbstractModel):
+    """AddRecordBackupTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TemplateName: 模板名称（仅支持中文、英文、数字、_、-，长度不超过32个字符，模板名称全局唯一，不能为空，不能重复）
+        :type TemplateName: str
+        :param _TimeSections: 上云时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
+        :type TimeSections: list of RecordTemplateTimeSections
+        :param _DevTimeSections: 录像时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
+        :type DevTimeSections: list of RecordTemplateTimeSections
+        :param _Scale: 上云倍速（支持1，2，4倍速）
+        :type Scale: int
+        """
+        self._TemplateName = None
+        self._TimeSections = None
+        self._DevTimeSections = None
+        self._Scale = None
+
+    @property
+    def TemplateName(self):
+        return self._TemplateName
+
+    @TemplateName.setter
+    def TemplateName(self, TemplateName):
+        self._TemplateName = TemplateName
+
+    @property
+    def TimeSections(self):
+        return self._TimeSections
+
+    @TimeSections.setter
+    def TimeSections(self, TimeSections):
+        self._TimeSections = TimeSections
+
+    @property
+    def DevTimeSections(self):
+        return self._DevTimeSections
+
+    @DevTimeSections.setter
+    def DevTimeSections(self, DevTimeSections):
+        self._DevTimeSections = DevTimeSections
+
+    @property
+    def Scale(self):
+        return self._Scale
+
+    @Scale.setter
+    def Scale(self, Scale):
+        self._Scale = Scale
+
+
+    def _deserialize(self, params):
+        self._TemplateName = params.get("TemplateName")
+        if params.get("TimeSections") is not None:
+            self._TimeSections = []
+            for item in params.get("TimeSections"):
+                obj = RecordTemplateTimeSections()
+                obj._deserialize(item)
+                self._TimeSections.append(obj)
+        if params.get("DevTimeSections") is not None:
+            self._DevTimeSections = []
+            for item in params.get("DevTimeSections"):
+                obj = RecordTemplateTimeSections()
+                obj._deserialize(item)
+                self._DevTimeSections.append(obj)
+        self._Scale = params.get("Scale")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddRecordBackupTemplateResponse(AbstractModel):
+    """AddRecordBackupTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddRecordBackupTemplateData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = AddRecordBackupTemplateData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class AddRecordPlanRequest(AbstractModel):
     """AddRecordPlan请求参数结构体
 
     """
 
@@ -1635,15 +1729,15 @@
     """AddRecordPlan返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回结果
-        :type Data: :class:`tencentcloud.iss.v20230517.models.RecordPlanOptResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.RecordPlanOptData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -1661,50 +1755,65 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = RecordPlanOptResponse()
+            self._Data = RecordPlanOptData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class AddRecordRetrieveTaskRequest(AbstractModel):
-    """AddRecordRetrieveTask请求参数结构体
+class AddRecordRetrieveTaskData(AbstractModel):
+    """查询取回任务详情返回数据
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskName: 任务名称，仅支持中文、英文、数字、_、-，长度不超过32个字符，模板名称全局唯一，不能为空，不能重复
+        :param _TaskId: 任务ID
+        :type TaskId: str
+        :param _TaskName: 任务名称
         :type TaskName: str
-        :param _StartTime: 取回录像的开始时间，UTC秒数，例如：1662114146，开始和结束时间段最长为一天，且不能跨天
+        :param _StartTime: 取回录像的开始时间
         :type StartTime: int
-        :param _EndTime: 取回录像的结束时间，UTC秒数，例如：1662114146，开始和结束时间段最长为一天，且不能跨天
+        :param _EndTime: 取回录像的结束时间
         :type EndTime: int
-        :param _Mode: 取回模式， 1:极速模式，其他暂不支持
+        :param _Mode: 取回模式，1:极速模式，其他暂不支持
         :type Mode: int
-        :param _Expiration: 取回录像副本有效期，最小为1天，最大为365天
+        :param _Expiration: 副本有效期
         :type Expiration: int
-        :param _Channels: 设备通道，一个任务最多32个设备通道
-        :type Channels: list of ChannelInfo
-        :param _Describe: 取回任务描述
+        :param _Status: 任务状态，0:已取回，1:取回中，2:待取回
+        :type Status: int
+        :param _Capacity: 取回容量，单位MB
+        :type Capacity: float
+        :param _Describe: 任务描述
+注意：此字段可能返回 null，表示取不到有效值。
         :type Describe: str
         """
+        self._TaskId = None
         self._TaskName = None
         self._StartTime = None
         self._EndTime = None
         self._Mode = None
         self._Expiration = None
-        self._Channels = None
+        self._Status = None
+        self._Capacity = None
         self._Describe = None
 
     @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+    @property
     def TaskName(self):
         return self._TaskName
 
     @TaskName.setter
     def TaskName(self, TaskName):
         self._TaskName = TaskName
 
@@ -1737,99 +1846,89 @@
         return self._Expiration
 
     @Expiration.setter
     def Expiration(self, Expiration):
         self._Expiration = Expiration
 
     @property
-    def Channels(self):
-        return self._Channels
+    def Status(self):
+        return self._Status
 
-    @Channels.setter
-    def Channels(self, Channels):
-        self._Channels = Channels
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def Capacity(self):
+        return self._Capacity
+
+    @Capacity.setter
+    def Capacity(self, Capacity):
+        self._Capacity = Capacity
 
     @property
     def Describe(self):
         return self._Describe
 
     @Describe.setter
     def Describe(self, Describe):
         self._Describe = Describe
 
 
     def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Mode = params.get("Mode")
         self._Expiration = params.get("Expiration")
-        if params.get("Channels") is not None:
-            self._Channels = []
-            for item in params.get("Channels"):
-                obj = ChannelInfo()
-                obj._deserialize(item)
-                self._Channels.append(obj)
+        self._Status = params.get("Status")
+        self._Capacity = params.get("Capacity")
         self._Describe = params.get("Describe")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AddRecordRetrieveTaskResponse(AbstractModel):
-    """查询取回任务详情返回数据
+class AddRecordRetrieveTaskRequest(AbstractModel):
+    """AddRecordRetrieveTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 任务ID
-        :type TaskId: str
-        :param _TaskName: 任务名称
+        :param _TaskName: 任务名称，仅支持中文、英文、数字、_、-，长度不超过32个字符，模板名称全局唯一，不能为空，不能重复
         :type TaskName: str
-        :param _StartTime: 取回录像的开始时间
+        :param _StartTime: 取回录像的开始时间，UTC秒数，例如：1662114146，开始和结束时间段最长为一天，且不能跨天
         :type StartTime: int
-        :param _EndTime: 取回录像的结束时间
+        :param _EndTime: 取回录像的结束时间，UTC秒数，例如：1662114146，开始和结束时间段最长为一天，且不能跨天
         :type EndTime: int
-        :param _Mode: 取回模式，1:极速模式，其他暂不支持
+        :param _Mode: 取回模式， 1:极速模式，其他暂不支持
         :type Mode: int
-        :param _Expiration: 副本有效期
+        :param _Expiration: 取回录像副本有效期，最小为1天，最大为365天
         :type Expiration: int
-        :param _Status: 任务状态，0:已取回，1:取回中，2:待取回
-        :type Status: int
-        :param _Capacity: 取回容量，单位MB
-        :type Capacity: float
-        :param _Describe: 任务描述
-注意：此字段可能返回 null，表示取不到有效值。
+        :param _Channels: 设备通道，一个任务最多32个设备通道
+        :type Channels: list of ChannelInfo
+        :param _Describe: 取回任务描述
         :type Describe: str
         """
-        self._TaskId = None
         self._TaskName = None
         self._StartTime = None
         self._EndTime = None
         self._Mode = None
         self._Expiration = None
-        self._Status = None
-        self._Capacity = None
+        self._Channels = None
         self._Describe = None
 
     @property
-    def TaskId(self):
-        return self._TaskId
-
-    @TaskId.setter
-    def TaskId(self, TaskId):
-        self._TaskId = TaskId
-
-    @property
     def TaskName(self):
         return self._TaskName
 
     @TaskName.setter
     def TaskName(self, TaskName):
         self._TaskName = TaskName
 
@@ -1862,48 +1961,90 @@
         return self._Expiration
 
     @Expiration.setter
     def Expiration(self, Expiration):
         self._Expiration = Expiration
 
     @property
-    def Status(self):
-        return self._Status
-
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
-
-    @property
-    def Capacity(self):
-        return self._Capacity
+    def Channels(self):
+        return self._Channels
 
-    @Capacity.setter
-    def Capacity(self, Capacity):
-        self._Capacity = Capacity
+    @Channels.setter
+    def Channels(self, Channels):
+        self._Channels = Channels
 
     @property
     def Describe(self):
         return self._Describe
 
     @Describe.setter
     def Describe(self, Describe):
         self._Describe = Describe
 
 
     def _deserialize(self, params):
-        self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._StartTime = params.get("StartTime")
         self._EndTime = params.get("EndTime")
         self._Mode = params.get("Mode")
         self._Expiration = params.get("Expiration")
-        self._Status = params.get("Status")
-        self._Capacity = params.get("Capacity")
+        if params.get("Channels") is not None:
+            self._Channels = []
+            for item in params.get("Channels"):
+                obj = ChannelInfo()
+                obj._deserialize(item)
+                self._Channels.append(obj)
         self._Describe = params.get("Describe")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddRecordRetrieveTaskResponse(AbstractModel):
+    """AddRecordRetrieveTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddRecordRetrieveTaskData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = AddRecordRetrieveTaskData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class AddRecordTemplateRequest(AbstractModel):
     """AddRecordTemplate请求参数结构体
 
     """
 
@@ -1987,43 +2128,54 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = RecordTemplateInfo()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class AddStreamAuthRequest(AbstractModel):
-    """AddStreamAuth请求参数结构体
+class AddStreamAuthData(AbstractModel):
+    """设置推拉流鉴权返回数据结构
 
     """
 
     def __init__(self):
         r"""
         :param _Id: 鉴权配置ID（uuid）
+注意：此字段可能返回 null，表示取不到有效值。
         :type Id: str
         :param _PullState: 是否开播放鉴权（1:开启,0:关闭）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PullState: int
         :param _PullSecret: 播放密钥（仅支持字母数字，长度0-10位）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PullSecret: str
         :param _PullExpired: 播放过期时间（单位：分钟）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PullExpired: int
         :param _PushState: 是否开启推流鉴权（1:开启,0:关闭）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PushState: int
         :param _PushSecret: 推流密钥（仅支持字母数字，长度0-10位）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PushSecret: str
         :param _PushExpired: 推流过期时间（单位：分钟）
+注意：此字段可能返回 null，表示取不到有效值。
         :type PushExpired: int
+        :param _AppId: 用户ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
         """
         self._Id = None
         self._PullState = None
         self._PullSecret = None
         self._PullExpired = None
         self._PushState = None
         self._PushSecret = None
         self._PushExpired = None
+        self._AppId = None
 
     @property
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
@@ -2073,73 +2225,71 @@
     def PushExpired(self):
         return self._PushExpired
 
     @PushExpired.setter
     def PushExpired(self, PushExpired):
         self._PushExpired = PushExpired
 
+    @property
+    def AppId(self):
+        return self._AppId
+
+    @AppId.setter
+    def AppId(self, AppId):
+        self._AppId = AppId
+
 
     def _deserialize(self, params):
         self._Id = params.get("Id")
         self._PullState = params.get("PullState")
         self._PullSecret = params.get("PullSecret")
         self._PullExpired = params.get("PullExpired")
         self._PushState = params.get("PushState")
         self._PushSecret = params.get("PushSecret")
         self._PushExpired = params.get("PushExpired")
+        self._AppId = params.get("AppId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class AddStreamAuthResponse(AbstractModel):
-    """设置推拉流鉴权返回数据结构
+class AddStreamAuthRequest(AbstractModel):
+    """AddStreamAuth请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Id: 鉴权配置ID（uuid）
-注意：此字段可能返回 null，表示取不到有效值。
         :type Id: str
         :param _PullState: 是否开播放鉴权（1:开启,0:关闭）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PullState: int
         :param _PullSecret: 播放密钥（仅支持字母数字，长度0-10位）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PullSecret: str
         :param _PullExpired: 播放过期时间（单位：分钟）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PullExpired: int
         :param _PushState: 是否开启推流鉴权（1:开启,0:关闭）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PushState: int
         :param _PushSecret: 推流密钥（仅支持字母数字，长度0-10位）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PushSecret: str
         :param _PushExpired: 推流过期时间（单位：分钟）
-注意：此字段可能返回 null，表示取不到有效值。
         :type PushExpired: int
-        :param _AppId: 用户ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type AppId: int
         """
         self._Id = None
         self._PullState = None
         self._PullSecret = None
         self._PullExpired = None
         self._PushState = None
         self._PushSecret = None
         self._PushExpired = None
-        self._AppId = None
 
     @property
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
@@ -2189,32 +2339,70 @@
     def PushExpired(self):
         return self._PushExpired
 
     @PushExpired.setter
     def PushExpired(self, PushExpired):
         self._PushExpired = PushExpired
 
-    @property
-    def AppId(self):
-        return self._AppId
-
-    @AppId.setter
-    def AppId(self, AppId):
-        self._AppId = AppId
-
 
     def _deserialize(self, params):
         self._Id = params.get("Id")
         self._PullState = params.get("PullState")
         self._PullSecret = params.get("PullSecret")
         self._PullExpired = params.get("PullExpired")
         self._PushState = params.get("PushState")
         self._PushSecret = params.get("PushSecret")
         self._PushExpired = params.get("PushExpired")
-        self._AppId = params.get("AppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AddStreamAuthResponse(AbstractModel):
+    """AddStreamAuth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 设置推拉流鉴权返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddStreamAuthData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = AddStreamAuthData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class AddUserDeviceRequest(AbstractModel):
     """AddUserDevice请求参数结构体
 
     """
 
@@ -2394,15 +2582,15 @@
     """AddUserDevice返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 增加设备返回数据
-        :type Data: :class:`tencentcloud.iss.v20230517.models.AddDeviceResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AddDeviceData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -2420,15 +2608,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = AddDeviceResponse()
+            self._Data = AddDeviceData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
 class BaseAIResultInfo(AbstractModel):
     """通用AI识别结果信息
 
@@ -3088,14 +3276,74 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
+class ControlDeviceStreamData(AbstractModel):
+    """获取开流地址返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Flv: flv 流地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Flv: str
+        :param _Hls: hls 流地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Hls: str
+        :param _Rtmp: rtmp 流地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Rtmp: str
+        """
+        self._Flv = None
+        self._Hls = None
+        self._Rtmp = None
+
+    @property
+    def Flv(self):
+        return self._Flv
+
+    @Flv.setter
+    def Flv(self, Flv):
+        self._Flv = Flv
+
+    @property
+    def Hls(self):
+        return self._Hls
+
+    @Hls.setter
+    def Hls(self, Hls):
+        self._Hls = Hls
+
+    @property
+    def Rtmp(self):
+        return self._Rtmp
+
+    @Rtmp.setter
+    def Rtmp(self, Rtmp):
+        self._Rtmp = Rtmp
+
+
+    def _deserialize(self, params):
+        self._Flv = params.get("Flv")
+        self._Hls = params.get("Hls")
+        self._Rtmp = params.get("Rtmp")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ControlDeviceStreamRequest(AbstractModel):
     """ControlDeviceStream请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3153,63 +3401,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ControlDeviceStreamResponse(AbstractModel):
-    """获取开流地址返回数据
+    """ControlDeviceStream返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Flv: flv 流地址
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Flv: str
-        :param _Hls: hls 流地址
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Hls: str
-        :param _Rtmp: rtmp 流地址
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Rtmp: str
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ControlDeviceStreamData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._Flv = None
-        self._Hls = None
-        self._Rtmp = None
-
-    @property
-    def Flv(self):
-        return self._Flv
-
-    @Flv.setter
-    def Flv(self, Flv):
-        self._Flv = Flv
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def Hls(self):
-        return self._Hls
+    def Data(self):
+        return self._Data
 
-    @Hls.setter
-    def Hls(self, Hls):
-        self._Hls = Hls
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def Rtmp(self):
-        return self._Rtmp
+    def RequestId(self):
+        return self._RequestId
 
-    @Rtmp.setter
-    def Rtmp(self, Rtmp):
-        self._Rtmp = Rtmp
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._Flv = params.get("Flv")
-        self._Hls = params.get("Hls")
-        self._Rtmp = params.get("Rtmp")
+        if params.get("Data") is not None:
+            self._Data = ControlDeviceStreamData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class ControlRecordRequest(AbstractModel):
     """ControlRecord请求参数结构体
 
     """
 
@@ -4189,15 +4424,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Data: AI识别结果
 注意：此字段可能返回 null，表示取不到有效值。
-        :type Data: :class:`tencentcloud.iss.v20230517.models.AITaskResultResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.AITaskResultData`
         :param _TotalCount: AI识别结果数量
         :type TotalCount: int
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._TotalCount = None
@@ -4226,15 +4461,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = AITaskResultResponse()
+            self._Data = AITaskResultData()
             self._Data._deserialize(params.get("Data"))
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
 class DescribeCNAMERequest(AbstractModel):
     """DescribeCNAME请求参数结构体
@@ -4302,48 +4537,15 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
-class DescribeDeviceChannelRequest(AbstractModel):
-    """DescribeDeviceChannel请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _DeviceId: 设备ID（从获取设备列表接口ListDevices中获取）
-        :type DeviceId: str
-        """
-        self._DeviceId = None
-
-    @property
-    def DeviceId(self):
-        return self._DeviceId
-
-    @DeviceId.setter
-    def DeviceId(self, DeviceId):
-        self._DeviceId = DeviceId
-
-
-    def _deserialize(self, params):
-        self._DeviceId = params.get("DeviceId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeDeviceChannelResponse(AbstractModel):
+class DescribeDeviceChannelData(AbstractModel):
     """查询设备通道信息返回结果
 
     """
 
     def __init__(self):
         r"""
         :param _DeviceId: 设备 ID
@@ -4476,163 +4678,66 @@
         self._Name = params.get("Name")
         self._Status = params.get("Status")
         self._PTZType = params.get("PTZType")
         self._Manufacturer = params.get("Manufacturer")
         self._Resolution = params.get("Resolution")
         self._State = params.get("State")
         self._Region = params.get("Region")
-
-
-class DescribeDevicePresetRequest(AbstractModel):
-    """DescribeDevicePreset请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _ChannelId: 通道ID（从通道查询接口DescribeDeviceChannel中获取）
-        :type ChannelId: str
-        """
-        self._ChannelId = None
-
-    @property
-    def ChannelId(self):
-        return self._ChannelId
-
-    @ChannelId.setter
-    def ChannelId(self, ChannelId):
-        self._ChannelId = ChannelId
-
-
-    def _deserialize(self, params):
-        self._ChannelId = params.get("ChannelId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeDevicePresetResponse(AbstractModel):
-    """查询设备预置位返回数据
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _Index: 预置位索引    只支持1-10的索引
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Index: int
-        :param _Name: 预置位名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Name: str
-        """
-        self._Index = None
-        self._Name = None
-
-    @property
-    def Index(self):
-        return self._Index
-
-    @Index.setter
-    def Index(self, Index):
-        self._Index = Index
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-
-    def _deserialize(self, params):
-        self._Index = params.get("Index")
-        self._Name = params.get("Name")
-
-
-class DescribeDeviceRegion(AbstractModel):
-    """查询设备可接入集群信息
+class DescribeDeviceChannelRequest(AbstractModel):
+    """DescribeDeviceChannel请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Label: 服务节点描述
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Label: str
-        :param _Value: 服务节点 ID（对应为其他接口中所需的 ClusterId）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Value: str
-        :param _Region: 地域信息
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Region: str
+        :param _DeviceId: 设备ID（从获取设备列表接口ListDevices中获取）
+        :type DeviceId: str
         """
-        self._Label = None
-        self._Value = None
-        self._Region = None
-
-    @property
-    def Label(self):
-        return self._Label
-
-    @Label.setter
-    def Label(self, Label):
-        self._Label = Label
-
-    @property
-    def Value(self):
-        return self._Value
-
-    @Value.setter
-    def Value(self, Value):
-        self._Value = Value
+        self._DeviceId = None
 
     @property
-    def Region(self):
-        return self._Region
+    def DeviceId(self):
+        return self._DeviceId
 
-    @Region.setter
-    def Region(self, Region):
-        self._Region = Region
+    @DeviceId.setter
+    def DeviceId(self, DeviceId):
+        self._DeviceId = DeviceId
 
 
     def _deserialize(self, params):
-        self._Label = params.get("Label")
-        self._Value = params.get("Value")
-        self._Region = params.get("Region")
+        self._DeviceId = params.get("DeviceId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeDeviceRegionRequest(AbstractModel):
-    """DescribeDeviceRegion请求参数结构体
-
-    """
-
-
-class DescribeDeviceRegionResponse(AbstractModel):
-    """DescribeDeviceRegion返回参数结构体
+class DescribeDeviceChannelResponse(AbstractModel):
+    """DescribeDeviceChannel返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Data: 返回数据
-        :type Data: list of DescribeDeviceRegion
+        :param _Data: 返回结果
+        :type Data: list of DescribeDeviceChannelData
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -4652,21 +4757,21 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = []
             for item in params.get("Data"):
-                obj = DescribeDeviceRegion()
+                obj = DescribeDeviceChannelData()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class DescribeDeviceResponse(AbstractModel):
+class DescribeDeviceData(AbstractModel):
     """查询设备接口返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _DeviceId: 设备ID
@@ -5018,22 +5123,138 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeDomainRegionRequest(AbstractModel):
-    """DescribeDomainRegion请求参数结构体
+class DescribeDevicePresetData(AbstractModel):
+    """查询设备预置位返回数据
 
     """
 
+    def __init__(self):
+        r"""
+        :param _Index: 预置位索引    只支持1-10的索引
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Index: int
+        :param _Name: 预置位名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        """
+        self._Index = None
+        self._Name = None
 
-class DescribeDomainRegionResponse(AbstractModel):
-    """查询域名可绑定集群数据
+    @property
+    def Index(self):
+        return self._Index
+
+    @Index.setter
+    def Index(self, Index):
+        self._Index = Index
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+
+    def _deserialize(self, params):
+        self._Index = params.get("Index")
+        self._Name = params.get("Name")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDevicePresetRequest(AbstractModel):
+    """DescribeDevicePreset请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ChannelId: 通道ID（从通道查询接口DescribeDeviceChannel中获取）
+        :type ChannelId: str
+        """
+        self._ChannelId = None
+
+    @property
+    def ChannelId(self):
+        return self._ChannelId
+
+    @ChannelId.setter
+    def ChannelId(self, ChannelId):
+        self._ChannelId = ChannelId
+
+
+    def _deserialize(self, params):
+        self._ChannelId = params.get("ChannelId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDevicePresetResponse(AbstractModel):
+    """DescribeDevicePreset返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of DescribeDevicePresetData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeDevicePresetData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDeviceRegion(AbstractModel):
+    """查询设备可接入集群信息
 
     """
 
     def __init__(self):
         r"""
         :param _Label: 服务节点描述
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5074,23 +5295,73 @@
         self._Region = Region
 
 
     def _deserialize(self, params):
         self._Label = params.get("Label")
         self._Value = params.get("Value")
         self._Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class DescribeDomainRequest(AbstractModel):
-    """DescribeDomain请求参数结构体
+class DescribeDeviceRegionRequest(AbstractModel):
+    """DescribeDeviceRegion请求参数结构体
 
     """
 
 
-class DescribeDomainResponse(AbstractModel):
+class DescribeDeviceRegionResponse(AbstractModel):
+    """DescribeDeviceRegion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of DescribeDeviceRegion
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeDeviceRegion()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDomainData(AbstractModel):
     """查询域名详情数据
 
     """
 
     def __init__(self):
         r"""
         :param _Id: 域名ID
@@ -5184,14 +5455,347 @@
         self._Id = params.get("Id")
         self._PlayDomain = params.get("PlayDomain")
         self._InternalDomain = params.get("InternalDomain")
         self._HaveCert = params.get("HaveCert")
         self._ClusterId = params.get("ClusterId")
         self._ClusterName = params.get("ClusterName")
         self._AppId = params.get("AppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDomainRegionData(AbstractModel):
+    """查询域名可绑定集群数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Label: 服务节点描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Label: str
+        :param _Value: 服务节点 ID（对应为其他接口中所需的 ClusterId）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        :param _Region: 地域信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self._Label = None
+        self._Value = None
+        self._Region = None
+
+    @property
+    def Label(self):
+        return self._Label
+
+    @Label.setter
+    def Label(self, Label):
+        self._Label = Label
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+    @property
+    def Region(self):
+        return self._Region
+
+    @Region.setter
+    def Region(self, Region):
+        self._Region = Region
+
+
+    def _deserialize(self, params):
+        self._Label = params.get("Label")
+        self._Value = params.get("Value")
+        self._Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDomainRegionRequest(AbstractModel):
+    """DescribeDomainRegion请求参数结构体
+
+    """
+
+
+class DescribeDomainRegionResponse(AbstractModel):
+    """DescribeDomainRegion返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of DescribeDomainRegionData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeDomainRegionData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDomainRequest(AbstractModel):
+    """DescribeDomain请求参数结构体
+
+    """
+
+
+class DescribeDomainResponse(AbstractModel):
+    """DescribeDomain返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of DescribeDomainData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeDomainData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeGatewayData(AbstractModel):
+    """查询网关信息返回结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _GatewayId: 网关索引ID，用于网关查询，更新，删除操作
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GatewayId: str
+        :param _GwId: 网关编码，由网关设备生成的唯一编码
+注意：此字段可能返回 null，表示取不到有效值。
+        :type GwId: str
+        :param _Name: 网关名称，仅支持中文、英文、数字、_、-，长度不超过32个字符
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _Description: 网关描述，仅支持中文、英文、数字、_、-，长度不超过128个字符
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param _ClusterId: 服务节点id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param _ClusterName: 服务节点名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterName: str
+        :param _Status: 网关状态，0：离线，1:在线
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param _Version: 网关版本
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Version: list of GatewayVersion
+        :param _DeviceNum: 网关下挂设备数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeviceNum: int
+        :param _CreatedAt: 激活时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreatedAt: str
+        :param _Region: 所属地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self._GatewayId = None
+        self._GwId = None
+        self._Name = None
+        self._Description = None
+        self._ClusterId = None
+        self._ClusterName = None
+        self._Status = None
+        self._Version = None
+        self._DeviceNum = None
+        self._CreatedAt = None
+        self._Region = None
+
+    @property
+    def GatewayId(self):
+        return self._GatewayId
+
+    @GatewayId.setter
+    def GatewayId(self, GatewayId):
+        self._GatewayId = GatewayId
+
+    @property
+    def GwId(self):
+        return self._GwId
+
+    @GwId.setter
+    def GwId(self, GwId):
+        self._GwId = GwId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
+
+    @property
+    def ClusterName(self):
+        return self._ClusterName
+
+    @ClusterName.setter
+    def ClusterName(self, ClusterName):
+        self._ClusterName = ClusterName
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def Version(self):
+        return self._Version
+
+    @Version.setter
+    def Version(self, Version):
+        self._Version = Version
+
+    @property
+    def DeviceNum(self):
+        return self._DeviceNum
+
+    @DeviceNum.setter
+    def DeviceNum(self, DeviceNum):
+        self._DeviceNum = DeviceNum
+
+    @property
+    def CreatedAt(self):
+        return self._CreatedAt
+
+    @CreatedAt.setter
+    def CreatedAt(self, CreatedAt):
+        self._CreatedAt = CreatedAt
+
+    @property
+    def Region(self):
+        return self._Region
+
+    @Region.setter
+    def Region(self, Region):
+        self._Region = Region
+
+
+    def _deserialize(self, params):
+        self._GatewayId = params.get("GatewayId")
+        self._GwId = params.get("GwId")
+        self._Name = params.get("Name")
+        self._Description = params.get("Description")
+        self._ClusterId = params.get("ClusterId")
+        self._ClusterName = params.get("ClusterName")
+        self._Status = params.get("Status")
+        if params.get("Version") is not None:
+            self._Version = []
+            for item in params.get("Version"):
+                obj = GatewayVersion()
+                obj._deserialize(item)
+                self._Version.append(obj)
+        self._DeviceNum = params.get("DeviceNum")
+        self._CreatedAt = params.get("CreatedAt")
+        self._Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class DescribeGatewayMonitor(AbstractModel):
     """查询网关监控信息返回结果
 
     """
 
@@ -5396,21 +6000,15 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = DescribeGatewayMonitor()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class DescribeGatewayProtocolRequest(AbstractModel):
-    """DescribeGatewayProtocol请求参数结构体
-
-    """
-
-
-class DescribeGatewayProtocolResponse(AbstractModel):
+class DescribeGatewayProtocolData(AbstractModel):
     """查询网关所支持的接入协议
 
     """
 
     def __init__(self):
         r"""
         :param _TypeCode: 接入协议的字典码
@@ -5452,14 +6050,70 @@
         self._Label = Label
 
 
     def _deserialize(self, params):
         self._TypeCode = params.get("TypeCode")
         self._Value = params.get("Value")
         self._Label = params.get("Label")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeGatewayProtocolRequest(AbstractModel):
+    """DescribeGatewayProtocol请求参数结构体
+
+    """
+
+
+class DescribeGatewayProtocolResponse(AbstractModel):
+    """DescribeGatewayProtocol返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of DescribeGatewayProtocolData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeGatewayProtocolData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
 
 
 class DescribeGatewayRequest(AbstractModel):
     """DescribeGateway请求参数结构体
 
     """
 
@@ -5488,172 +6142,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DescribeGatewayResponse(AbstractModel):
-    """查询网关信息返回结果
+    """DescribeGateway返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _GatewayId: 网关索引ID，用于网关查询，更新，删除操作
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GatewayId: str
-        :param _GwId: 网关编码，由网关设备生成的唯一编码
-注意：此字段可能返回 null，表示取不到有效值。
-        :type GwId: str
-        :param _Name: 网关名称，仅支持中文、英文、数字、_、-，长度不超过32个字符
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Name: str
-        :param _Description: 网关描述，仅支持中文、英文、数字、_、-，长度不超过128个字符
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Description: str
-        :param _ClusterId: 服务节点id
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ClusterId: str
-        :param _ClusterName: 服务节点名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ClusterName: str
-        :param _Status: 网关状态，0：离线，1:在线
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Status: int
-        :param _Version: 网关版本
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Version: list of GatewayVersion
-        :param _DeviceNum: 网关下挂设备数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DeviceNum: int
-        :param _CreatedAt: 激活时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type CreatedAt: str
-        :param _Region: 所属地域
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Region: str
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeGatewayData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._GatewayId = None
-        self._GwId = None
-        self._Name = None
-        self._Description = None
-        self._ClusterId = None
-        self._ClusterName = None
-        self._Status = None
-        self._Version = None
-        self._DeviceNum = None
-        self._CreatedAt = None
-        self._Region = None
-
-    @property
-    def GatewayId(self):
-        return self._GatewayId
-
-    @GatewayId.setter
-    def GatewayId(self, GatewayId):
-        self._GatewayId = GatewayId
-
-    @property
-    def GwId(self):
-        return self._GwId
-
-    @GwId.setter
-    def GwId(self, GwId):
-        self._GwId = GwId
-
-    @property
-    def Name(self):
-        return self._Name
-
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
-
-    @property
-    def Description(self):
-        return self._Description
-
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
-
-    @property
-    def ClusterId(self):
-        return self._ClusterId
-
-    @ClusterId.setter
-    def ClusterId(self, ClusterId):
-        self._ClusterId = ClusterId
-
-    @property
-    def ClusterName(self):
-        return self._ClusterName
-
-    @ClusterName.setter
-    def ClusterName(self, ClusterName):
-        self._ClusterName = ClusterName
-
-    @property
-    def Status(self):
-        return self._Status
-
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
-
-    @property
-    def Version(self):
-        return self._Version
-
-    @Version.setter
-    def Version(self, Version):
-        self._Version = Version
-
-    @property
-    def DeviceNum(self):
-        return self._DeviceNum
-
-    @DeviceNum.setter
-    def DeviceNum(self, DeviceNum):
-        self._DeviceNum = DeviceNum
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def CreatedAt(self):
-        return self._CreatedAt
+    def Data(self):
+        return self._Data
 
-    @CreatedAt.setter
-    def CreatedAt(self, CreatedAt):
-        self._CreatedAt = CreatedAt
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def Region(self):
-        return self._Region
+    def RequestId(self):
+        return self._RequestId
 
-    @Region.setter
-    def Region(self, Region):
-        self._Region = Region
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._GatewayId = params.get("GatewayId")
-        self._GwId = params.get("GwId")
-        self._Name = params.get("Name")
-        self._Description = params.get("Description")
-        self._ClusterId = params.get("ClusterId")
-        self._ClusterName = params.get("ClusterName")
-        self._Status = params.get("Status")
-        if params.get("Version") is not None:
-            self._Version = []
-            for item in params.get("Version"):
-                obj = GatewayVersion()
-                obj._deserialize(item)
-                self._Version.append(obj)
-        self._DeviceNum = params.get("DeviceNum")
-        self._CreatedAt = params.get("CreatedAt")
-        self._Region = params.get("Region")
+        if params.get("Data") is not None:
+            self._Data = DescribeGatewayData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class DescribeGatewayVersion(AbstractModel):
     """查询网关服务版本信息返回数据
 
     """
 
@@ -5734,14 +6266,53 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeGatewayVersionData(AbstractModel):
+    """查询网关服务版本信息返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Services: 网关服务列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Services: list of DescribeGatewayVersion
+        """
+        self._Services = None
+
+    @property
+    def Services(self):
+        return self._Services
+
+    @Services.setter
+    def Services(self, Services):
+        self._Services = Services
+
+
+    def _deserialize(self, params):
+        if params.get("Services") is not None:
+            self._Services = []
+            for item in params.get("Services"):
+                obj = DescribeGatewayVersion()
+                obj._deserialize(item)
+                self._Services.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeGatewayVersionRequest(AbstractModel):
     """DescribeGatewayVersion请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5768,51 +6339,53 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DescribeGatewayVersionResponse(AbstractModel):
-    """查询网关服务版本信息返回数据
+    """DescribeGatewayVersion返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Services: 网关服务列表
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Services: list of DescribeGatewayVersion
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeGatewayVersionData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._Services = None
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def Services(self):
-        return self._Services
-
-    @Services.setter
-    def Services(self, Services):
-        self._Services = Services
+    def Data(self):
+        return self._Data
 
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
-    def _deserialize(self, params):
-        if params.get("Services") is not None:
-            self._Services = []
-            for item in params.get("Services"):
-                obj = DescribeGatewayVersion()
-                obj._deserialize(item)
-                self._Services.append(obj)
+    @property
+    def RequestId(self):
+        return self._RequestId
 
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
-class DescribeOrganizationRequest(AbstractModel):
-    """DescribeOrganization请求参数结构体
 
-    """
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DescribeGatewayVersionData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
-class DescribeOrganizationResponse(AbstractModel):
+class DescribeOrganizationData(AbstractModel):
     """查询组织数据返回结果
 
     """
 
     def __init__(self):
         r"""
         :param _OrganizationId: 组织 ID
@@ -5919,50 +6492,73 @@
         self._Name = params.get("Name")
         self._ParentId = params.get("ParentId")
         self._Level = params.get("Level")
         self._AppId = params.get("AppId")
         self._ParentIds = params.get("ParentIds")
         self._Total = params.get("Total")
         self._Online = params.get("Online")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class DescribeRecordBackupPlanRequest(AbstractModel):
-    """DescribeRecordBackupPlan请求参数结构体
+class DescribeOrganizationRequest(AbstractModel):
+    """DescribeOrganization请求参数结构体
+
+    """
+
+
+class DescribeOrganizationResponse(AbstractModel):
+    """DescribeOrganization返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlanId: 录像上云计划ID（从查询录像上云计划列表接口ListRecordBackupPlans中获取）
-        :type PlanId: str
+        :param _Data: 返回数据
+        :type Data: list of DescribeOrganizationData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._PlanId = None
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def PlanId(self):
-        return self._PlanId
+    def Data(self):
+        return self._Data
 
-    @PlanId.setter
-    def PlanId(self, PlanId):
-        self._PlanId = PlanId
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._PlanId = params.get("PlanId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = DescribeOrganizationData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
 
 
-class DescribeRecordBackupPlanResponse(AbstractModel):
+class DescribeRecordBackupPlanData(AbstractModel):
     """查询录像上云计划返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _PlanId: 录像上云计划ID
@@ -6075,50 +6671,97 @@
         if params.get("LifeCycle") is not None:
             self._LifeCycle = LifeCycleData()
             self._LifeCycle._deserialize(params.get("LifeCycle"))
         self._Status = params.get("Status")
         self._ChannelCount = params.get("ChannelCount")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class DescribeRecordBackupTemplateRequest(AbstractModel):
-    """DescribeRecordBackupTemplate请求参数结构体
+class DescribeRecordBackupPlanRequest(AbstractModel):
+    """DescribeRecordBackupPlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 模板ID（从查询录像上云模板列表接口ListRecordBackupTemplates中获取）
-        :type TemplateId: str
+        :param _PlanId: 录像上云计划ID（从查询录像上云计划列表接口ListRecordBackupPlans中获取）
+        :type PlanId: str
         """
-        self._TemplateId = None
+        self._PlanId = None
 
     @property
-    def TemplateId(self):
-        return self._TemplateId
+    def PlanId(self):
+        return self._PlanId
 
-    @TemplateId.setter
-    def TemplateId(self, TemplateId):
-        self._TemplateId = TemplateId
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
 
 
     def _deserialize(self, params):
-        self._TemplateId = params.get("TemplateId")
+        self._PlanId = params.get("PlanId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeRecordBackupTemplateResponse(AbstractModel):
+class DescribeRecordBackupPlanResponse(AbstractModel):
+    """DescribeRecordBackupPlan返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeRecordBackupPlanData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DescribeRecordBackupPlanData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeRecordBackupTemplateData(AbstractModel):
     """查询录像上云模版返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _TemplateId: 模板ID
@@ -6222,14 +6865,145 @@
             for item in params.get("DevTimeSections"):
                 obj = RecordTemplateTimeSections()
                 obj._deserialize(item)
                 self._DevTimeSections.append(obj)
         self._Scale = params.get("Scale")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRecordBackupTemplateRequest(AbstractModel):
+    """DescribeRecordBackupTemplate请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TemplateId: 模板ID（从查询录像上云模板列表接口ListRecordBackupTemplates中获取）
+        :type TemplateId: str
+        """
+        self._TemplateId = None
+
+    @property
+    def TemplateId(self):
+        return self._TemplateId
+
+    @TemplateId.setter
+    def TemplateId(self, TemplateId):
+        self._TemplateId = TemplateId
+
+
+    def _deserialize(self, params):
+        self._TemplateId = params.get("TemplateId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRecordBackupTemplateResponse(AbstractModel):
+    """DescribeRecordBackupTemplate返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeRecordBackupTemplateData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DescribeRecordBackupTemplateData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeRecordFileData(AbstractModel):
+    """用于查询设备云端录像时间轴信息返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Tips: 提示类型，0:时间段内无归档录像，1:时间段内有归档录像
+        :type Tips: int
+        :param _List: 存在为数组格式，不存在字段内容为空
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: list of RecordTimeLine
+        """
+        self._Tips = None
+        self._List = None
+
+    @property
+    def Tips(self):
+        return self._Tips
+
+    @Tips.setter
+    def Tips(self, Tips):
+        self._Tips = Tips
+
+    @property
+    def List(self):
+        return self._List
+
+    @List.setter
+    def List(self, List):
+        self._List = List
+
+
+    def _deserialize(self, params):
+        self._Tips = params.get("Tips")
+        if params.get("List") is not None:
+            self._List = []
+            for item in params.get("List"):
+                obj = RecordTimeLine()
+                obj._deserialize(item)
+                self._List.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class DescribeRecordFileRequest(AbstractModel):
     """DescribeRecordFile请求参数结构体
 
     """
 
@@ -6294,54 +7068,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DescribeRecordFileResponse(AbstractModel):
-    """用于查询设备云端录像时间轴信息返回数据
+    """DescribeRecordFile返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Tips: 提示类型，0:时间段内无归档录像，1:时间段内有归档录像
-        :type Tips: int
-        :param _List: 存在为数组格式，不存在字段内容为空
-注意：此字段可能返回 null，表示取不到有效值。
-        :type List: list of RecordTimeLine
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeRecordFileData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._Tips = None
-        self._List = None
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def Tips(self):
-        return self._Tips
+    def Data(self):
+        return self._Data
 
-    @Tips.setter
-    def Tips(self, Tips):
-        self._Tips = Tips
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def List(self):
-        return self._List
+    def RequestId(self):
+        return self._RequestId
 
-    @List.setter
-    def List(self, List):
-        self._List = List
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._Tips = params.get("Tips")
-        if params.get("List") is not None:
-            self._List = []
-            for item in params.get("List"):
-                obj = RecordTimeLine()
-                obj._deserialize(item)
-                self._List.append(obj)
+        if params.get("Data") is not None:
+            self._Data = DescribeRecordFileData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class DescribeRecordPlanRequest(AbstractModel):
     """DescribeRecordPlan请求参数结构体
 
     """
 
@@ -6504,48 +7274,15 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = RecordPlaybackUrl()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class DescribeRecordRetrieveTaskRequest(AbstractModel):
-    """DescribeRecordRetrieveTask请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _TaskId: 云录像取回任务ID
-        :type TaskId: str
-        """
-        self._TaskId = None
-
-    @property
-    def TaskId(self):
-        return self._TaskId
-
-    @TaskId.setter
-    def TaskId(self, TaskId):
-        self._TaskId = TaskId
-
-
-    def _deserialize(self, params):
-        self._TaskId = params.get("TaskId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeRecordRetrieveTaskResponse(AbstractModel):
+class DescribeRecordRetrieveTaskData(AbstractModel):
     """查询云录像取回任务详情返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _TaskId: 取回任务ID
@@ -6686,14 +7423,94 @@
             self._Channels = []
             for item in params.get("Channels"):
                 obj = RecordRetrieveTaskChannelInfo()
                 obj._deserialize(item)
                 self._Channels.append(obj)
         self._Describe = params.get("Describe")
         self._ChannelCount = params.get("ChannelCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRecordRetrieveTaskRequest(AbstractModel):
+    """DescribeRecordRetrieveTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TaskId: 云录像取回任务ID
+        :type TaskId: str
+        """
+        self._TaskId = None
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeRecordRetrieveTaskResponse(AbstractModel):
+    """DescribeRecordRetrieveTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeRecordRetrieveTaskData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DescribeRecordRetrieveTaskData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class DescribeRecordTemplateRequest(AbstractModel):
     """DescribeRecordTemplate请求参数结构体
 
     """
 
@@ -6760,21 +7577,15 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = RecordTemplateInfo()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
-class DescribeStreamAuthRequest(AbstractModel):
-    """DescribeStreamAuth请求参数结构体
-
-    """
-
-
-class DescribeStreamAuthResponse(AbstractModel):
+class DescribeStreamAuthData(AbstractModel):
     """查询推拉流鉴权返回数据结构
 
     """
 
     def __init__(self):
         r"""
         :param _Id: 鉴权配置ID（uuid）
@@ -6881,14 +7692,67 @@
         self._PullState = params.get("PullState")
         self._PullSecret = params.get("PullSecret")
         self._PullExpired = params.get("PullExpired")
         self._PushState = params.get("PushState")
         self._PushSecret = params.get("PushSecret")
         self._PushExpired = params.get("PushExpired")
         self._AppId = params.get("AppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeStreamAuthRequest(AbstractModel):
+    """DescribeStreamAuth请求参数结构体
+
+    """
+
+
+class DescribeStreamAuthResponse(AbstractModel):
+    """DescribeStreamAuth返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeStreamAuthData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = DescribeStreamAuthData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class DescribeUserDeviceRequest(AbstractModel):
     """DescribeUserDevice请求参数结构体
 
     """
 
@@ -6924,15 +7788,15 @@
     """DescribeUserDevice返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回结果
-        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeDeviceResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeDeviceData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -6950,19 +7814,82 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = DescribeDeviceResponse()
+            self._Data = DescribeDeviceData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
+class DescribeVideoDownloadUrlData(AbstractModel):
+    """获取云录像下载URL返回的数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Url: 录像文件下载 URL
+注意：
+URL 有效期是10分钟，过期后将拒绝访问，若需再用请重新获取 
+录像文件下载采用分块传输编码，响应头Transfer-Encoding:chunked 
+下载文件命名格式为{ChannelId}-{BeginTime}-{EndTime}.{FileType} 
+        :type Url: str
+        :param _ActualBeginTime: 实际下载录像的开始时间
+注意：当请求中指定IsRespActualTime参数为true时，才有该字段
+        :type ActualBeginTime: str
+        :param _ActualEndTime: 实际下载录像的结束时间
+注意：当请求中指定IsRespActualTime参数为true时，才有该字段
+        :type ActualEndTime: str
+        """
+        self._Url = None
+        self._ActualBeginTime = None
+        self._ActualEndTime = None
+
+    @property
+    def Url(self):
+        return self._Url
+
+    @Url.setter
+    def Url(self, Url):
+        self._Url = Url
+
+    @property
+    def ActualBeginTime(self):
+        return self._ActualBeginTime
+
+    @ActualBeginTime.setter
+    def ActualBeginTime(self, ActualBeginTime):
+        self._ActualBeginTime = ActualBeginTime
+
+    @property
+    def ActualEndTime(self):
+        return self._ActualEndTime
+
+    @ActualEndTime.setter
+    def ActualEndTime(self, ActualEndTime):
+        self._ActualEndTime = ActualEndTime
+
+
+    def _deserialize(self, params):
+        self._Url = params.get("Url")
+        self._ActualBeginTime = params.get("ActualBeginTime")
+        self._ActualEndTime = params.get("ActualEndTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeVideoDownloadUrlRequest(AbstractModel):
     """DescribeVideoDownloadUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7037,66 +7964,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class DescribeVideoDownloadUrlResponse(AbstractModel):
-    """获取云录像下载URL返回的数据
+    """DescribeVideoDownloadUrl返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Url: 录像文件下载 URL
-注意：
-URL 有效期是10分钟，过期后将拒绝访问，若需再用请重新获取 
-录像文件下载采用分块传输编码，响应头Transfer-Encoding:chunked 
-下载文件命名格式为{ChannelId}-{BeginTime}-{EndTime}.{FileType} 
-        :type Url: str
-        :param _ActualBeginTime: 实际下载录像的开始时间
-注意：当请求中指定IsRespActualTime参数为true时，才有该字段
-        :type ActualBeginTime: str
-        :param _ActualEndTime: 实际下载录像的结束时间
-注意：当请求中指定IsRespActualTime参数为true时，才有该字段
-        :type ActualEndTime: str
+        :param _Data: 返回的数据结构
+        :type Data: :class:`tencentcloud.iss.v20230517.models.DescribeVideoDownloadUrlData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._Url = None
-        self._ActualBeginTime = None
-        self._ActualEndTime = None
-
-    @property
-    def Url(self):
-        return self._Url
-
-    @Url.setter
-    def Url(self, Url):
-        self._Url = Url
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def ActualBeginTime(self):
-        return self._ActualBeginTime
+    def Data(self):
+        return self._Data
 
-    @ActualBeginTime.setter
-    def ActualBeginTime(self, ActualBeginTime):
-        self._ActualBeginTime = ActualBeginTime
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def ActualEndTime(self):
-        return self._ActualEndTime
+    def RequestId(self):
+        return self._RequestId
 
-    @ActualEndTime.setter
-    def ActualEndTime(self, ActualEndTime):
-        self._ActualEndTime = ActualEndTime
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._Url = params.get("Url")
-        self._ActualBeginTime = params.get("ActualBeginTime")
-        self._ActualEndTime = params.get("ActualEndTime")
+        if params.get("Data") is not None:
+            self._Data = DescribeVideoDownloadUrlData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class FaceMaskAIResultInfo(AbstractModel):
     """口罩识别结果详情
 
     """
 
@@ -7929,14 +8840,66 @@
                 obj = ListDeviceInfo()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._TotalCount = params.get("TotalCount")
         self._RequestId = params.get("RequestId")
 
 
+class ListGatewaysData(AbstractModel):
+    """查询网关列表返回结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _List: 网关列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: list of GatewaysData
+        :param _TotalCount: 网关数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        """
+        self._List = None
+        self._TotalCount = None
+
+    @property
+    def List(self):
+        return self._List
+
+    @List.setter
+    def List(self, List):
+        self._List = List
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+
+    def _deserialize(self, params):
+        if params.get("List") is not None:
+            self._List = []
+            for item in params.get("List"):
+                obj = GatewaysData()
+                obj._deserialize(item)
+                self._List.append(obj)
+        self._TotalCount = params.get("TotalCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ListGatewaysRequest(AbstractModel):
     """ListGateways请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8011,91 +8974,53 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ListGatewaysResponse(AbstractModel):
-    """查询网关列表返回结果
+    """ListGateways返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _List: 网关列表
-注意：此字段可能返回 null，表示取不到有效值。
-        :type List: list of GatewaysData
-        :param _TotalCount: 网关数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TotalCount: int
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListGatewaysData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._List = None
-        self._TotalCount = None
-
-    @property
-    def List(self):
-        return self._List
-
-    @List.setter
-    def List(self, List):
-        self._List = List
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def TotalCount(self):
-        return self._TotalCount
-
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
-
-
-    def _deserialize(self, params):
-        if params.get("List") is not None:
-            self._List = []
-            for item in params.get("List"):
-                obj = GatewaysData()
-                obj._deserialize(item)
-                self._List.append(obj)
-        self._TotalCount = params.get("TotalCount")
-
-
-class ListOrganizationChannelNumbersRequest(AbstractModel):
-    """ListOrganizationChannelNumbers请求参数结构体
-
-    """
+    def Data(self):
+        return self._Data
 
-    def __init__(self):
-        r"""
-        :param _OrganizationId: 组织ID，json数组格式，最多一次支持10个组织
-        :type OrganizationId: list of str
-        """
-        self._OrganizationId = None
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def OrganizationId(self):
-        return self._OrganizationId
+    def RequestId(self):
+        return self._RequestId
 
-    @OrganizationId.setter
-    def OrganizationId(self, OrganizationId):
-        self._OrganizationId = OrganizationId
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._OrganizationId = params.get("OrganizationId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+        if params.get("Data") is not None:
+            self._Data = ListGatewaysData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
-class ListOrganizationChannelNumbersResponse(AbstractModel):
+class ListOrganizationChannelNumbersData(AbstractModel):
     """组织目录下的未添加到实时上云计划中的通道数量返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _TotalCount: 组织下通道总数
@@ -8122,100 +9047,97 @@
     def NotInPlanCount(self, NotInPlanCount):
         self._NotInPlanCount = NotInPlanCount
 
 
     def _deserialize(self, params):
         self._TotalCount = params.get("TotalCount")
         self._NotInPlanCount = params.get("NotInPlanCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class ListOrganizationChannelsRequest(AbstractModel):
-    """ListOrganizationChannels请求参数结构体
+class ListOrganizationChannelNumbersRequest(AbstractModel):
+    """ListOrganizationChannelNumbers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _OrganizationId: 组织ID
-        :type OrganizationId: str
-        :param _PageSize: 每页最大数量
-        :type PageSize: int
-        :param _PageNumber: 第几页 
-        :type PageNumber: int
-        :param _DeviceName: 查询条件，则按照设备名称查询
-查询条件同时只有一个生效。长度不超过32字节
-        :type DeviceName: str
-        :param _ChannelName: 查询条件，则按照通道名称查询
-查询条件同时只有一个生效。长度不超过32字节
-        :type ChannelName: str
+        :param _OrganizationId: 组织ID，json数组格式，最多一次支持10个组织
+        :type OrganizationId: list of str
         """
         self._OrganizationId = None
-        self._PageSize = None
-        self._PageNumber = None
-        self._DeviceName = None
-        self._ChannelName = None
 
     @property
     def OrganizationId(self):
         return self._OrganizationId
 
     @OrganizationId.setter
     def OrganizationId(self, OrganizationId):
         self._OrganizationId = OrganizationId
 
-    @property
-    def PageSize(self):
-        return self._PageSize
 
-    @PageSize.setter
-    def PageSize(self, PageSize):
-        self._PageSize = PageSize
+    def _deserialize(self, params):
+        self._OrganizationId = params.get("OrganizationId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
-    @property
-    def PageNumber(self):
-        return self._PageNumber
 
-    @PageNumber.setter
-    def PageNumber(self, PageNumber):
-        self._PageNumber = PageNumber
+class ListOrganizationChannelNumbersResponse(AbstractModel):
+    """ListOrganizationChannelNumbers返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListOrganizationChannelNumbersData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def DeviceName(self):
-        return self._DeviceName
+    def Data(self):
+        return self._Data
 
-    @DeviceName.setter
-    def DeviceName(self, DeviceName):
-        self._DeviceName = DeviceName
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def ChannelName(self):
-        return self._ChannelName
+    def RequestId(self):
+        return self._RequestId
 
-    @ChannelName.setter
-    def ChannelName(self, ChannelName):
-        self._ChannelName = ChannelName
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._OrganizationId = params.get("OrganizationId")
-        self._PageSize = params.get("PageSize")
-        self._PageNumber = params.get("PageNumber")
-        self._DeviceName = params.get("DeviceName")
-        self._ChannelName = params.get("ChannelName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+        if params.get("Data") is not None:
+            self._Data = ListOrganizationChannelNumbersData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
-class ListOrganizationChannelsResponse(AbstractModel):
+class ListOrganizationChannelsData(AbstractModel):
     """查询组织目录下的通道列表返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _PageNumber: 第几页
@@ -8272,74 +9194,57 @@
         self._TotalCount = params.get("TotalCount")
         if params.get("List") is not None:
             self._List = []
             for item in params.get("List"):
                 obj = OrganizationChannelInfo()
                 obj._deserialize(item)
                 self._List.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class ListRecordBackupPlanDevicesRequest(AbstractModel):
-    """ListRecordBackupPlanDevices请求参数结构体
+class ListOrganizationChannelsRequest(AbstractModel):
+    """ListOrganizationChannels请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlanId: 录像计划ID（从查询录像上云计划列表接口ListRecordBackupPlans中获取）
-        :type PlanId: str
-        :param _DeviceName: 按照设备名称查询（为空时，不参考该参数）
+        :param _OrganizationId: 组织ID
+        :type OrganizationId: str
+        :param _PageSize: 每页最大数量
+        :type PageSize: int
+        :param _PageNumber: 第几页 
+        :type PageNumber: int
+        :param _DeviceName: 查询条件，则按照设备名称查询
+查询条件同时只有一个生效。长度不超过32字节
         :type DeviceName: str
-        :param _ChannelName: 按照通道名称查询（为空时，不参考该参数）
+        :param _ChannelName: 查询条件，则按照通道名称查询
+查询条件同时只有一个生效。长度不超过32字节
         :type ChannelName: str
-        :param _OrganizationName: 按照组织名称查询（为空时，不参考该参数）
-        :type OrganizationName: str
-        :param _PageSize: 每页最大数量
-        :type PageSize: str
-        :param _PageNumber: 第几页
-        :type PageNumber: str
         """
-        self._PlanId = None
-        self._DeviceName = None
-        self._ChannelName = None
-        self._OrganizationName = None
+        self._OrganizationId = None
         self._PageSize = None
         self._PageNumber = None
+        self._DeviceName = None
+        self._ChannelName = None
 
     @property
-    def PlanId(self):
-        return self._PlanId
-
-    @PlanId.setter
-    def PlanId(self, PlanId):
-        self._PlanId = PlanId
-
-    @property
-    def DeviceName(self):
-        return self._DeviceName
-
-    @DeviceName.setter
-    def DeviceName(self, DeviceName):
-        self._DeviceName = DeviceName
-
-    @property
-    def ChannelName(self):
-        return self._ChannelName
-
-    @ChannelName.setter
-    def ChannelName(self, ChannelName):
-        self._ChannelName = ChannelName
-
-    @property
-    def OrganizationName(self):
-        return self._OrganizationName
+    def OrganizationId(self):
+        return self._OrganizationId
 
-    @OrganizationName.setter
-    def OrganizationName(self, OrganizationName):
-        self._OrganizationName = OrganizationName
+    @OrganizationId.setter
+    def OrganizationId(self, OrganizationId):
+        self._OrganizationId = OrganizationId
 
     @property
     def PageSize(self):
         return self._PageSize
 
     @PageSize.setter
     def PageSize(self, PageSize):
@@ -8349,100 +9254,87 @@
     def PageNumber(self):
         return self._PageNumber
 
     @PageNumber.setter
     def PageNumber(self, PageNumber):
         self._PageNumber = PageNumber
 
+    @property
+    def DeviceName(self):
+        return self._DeviceName
+
+    @DeviceName.setter
+    def DeviceName(self, DeviceName):
+        self._DeviceName = DeviceName
+
+    @property
+    def ChannelName(self):
+        return self._ChannelName
+
+    @ChannelName.setter
+    def ChannelName(self, ChannelName):
+        self._ChannelName = ChannelName
+
 
     def _deserialize(self, params):
-        self._PlanId = params.get("PlanId")
-        self._DeviceName = params.get("DeviceName")
-        self._ChannelName = params.get("ChannelName")
-        self._OrganizationName = params.get("OrganizationName")
+        self._OrganizationId = params.get("OrganizationId")
         self._PageSize = params.get("PageSize")
         self._PageNumber = params.get("PageNumber")
+        self._DeviceName = params.get("DeviceName")
+        self._ChannelName = params.get("ChannelName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ListRecordBackupPlanDevicesResponse(AbstractModel):
-    """查询录像上云计划关联通道的返回数据
+class ListOrganizationChannelsResponse(AbstractModel):
+    """ListOrganizationChannels返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PageNumber: 第几页
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PageNumber: int
-        :param _PageSize: 当前页的设备数量
-注意：此字段可能返回 null，表示取不到有效值。
-        :type PageSize: int
-        :param _TotalCount: 本次查询的设备通道总数
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TotalCount: int
-        :param _List: 设备通道信息列表
-注意：此字段可能返回 null，表示取不到有效值。
-        :type List: :class:`tencentcloud.iss.v20230517.models.RecordPlanChannelInfo`
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListOrganizationChannelsData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._PageNumber = None
-        self._PageSize = None
-        self._TotalCount = None
-        self._List = None
-
-    @property
-    def PageNumber(self):
-        return self._PageNumber
-
-    @PageNumber.setter
-    def PageNumber(self, PageNumber):
-        self._PageNumber = PageNumber
-
-    @property
-    def PageSize(self):
-        return self._PageSize
-
-    @PageSize.setter
-    def PageSize(self, PageSize):
-        self._PageSize = PageSize
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def TotalCount(self):
-        return self._TotalCount
+    def Data(self):
+        return self._Data
 
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def List(self):
-        return self._List
+    def RequestId(self):
+        return self._RequestId
 
-    @List.setter
-    def List(self, List):
-        self._List = List
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._PageNumber = params.get("PageNumber")
-        self._PageSize = params.get("PageSize")
-        self._TotalCount = params.get("TotalCount")
-        if params.get("List") is not None:
-            self._List = RecordPlanChannelInfo()
-            self._List._deserialize(params.get("List"))
+        if params.get("Data") is not None:
+            self._Data = ListOrganizationChannelsData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
-class ListRecordBackupPlanResponse(AbstractModel):
+class ListRecordBackupPlanData(AbstractModel):
     """查询录像上云计划列表返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _PlanId: 录像上云计划ID
@@ -8565,29 +9457,236 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ListRecordBackupPlanDevicesData(AbstractModel):
+    """查询录像上云计划关联通道的返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PageNumber: 第几页
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PageNumber: int
+        :param _PageSize: 当前页的设备数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PageSize: int
+        :param _TotalCount: 本次查询的设备通道总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalCount: int
+        :param _List: 设备通道信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: :class:`tencentcloud.iss.v20230517.models.RecordPlanChannelInfo`
+        """
+        self._PageNumber = None
+        self._PageSize = None
+        self._TotalCount = None
+        self._List = None
+
+    @property
+    def PageNumber(self):
+        return self._PageNumber
+
+    @PageNumber.setter
+    def PageNumber(self, PageNumber):
+        self._PageNumber = PageNumber
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def List(self):
+        return self._List
+
+    @List.setter
+    def List(self, List):
+        self._List = List
+
+
+    def _deserialize(self, params):
+        self._PageNumber = params.get("PageNumber")
+        self._PageSize = params.get("PageSize")
+        self._TotalCount = params.get("TotalCount")
+        if params.get("List") is not None:
+            self._List = RecordPlanChannelInfo()
+            self._List._deserialize(params.get("List"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ListRecordBackupPlanDevicesRequest(AbstractModel):
+    """ListRecordBackupPlanDevices请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 录像计划ID（从查询录像上云计划列表接口ListRecordBackupPlans中获取）
+        :type PlanId: str
+        :param _DeviceName: 按照设备名称查询（为空时，不参考该参数）
+        :type DeviceName: str
+        :param _ChannelName: 按照通道名称查询（为空时，不参考该参数）
+        :type ChannelName: str
+        :param _OrganizationName: 按照组织名称查询（为空时，不参考该参数）
+        :type OrganizationName: str
+        :param _PageSize: 每页最大数量
+        :type PageSize: str
+        :param _PageNumber: 第几页
+        :type PageNumber: str
+        """
+        self._PlanId = None
+        self._DeviceName = None
+        self._ChannelName = None
+        self._OrganizationName = None
+        self._PageSize = None
+        self._PageNumber = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+    @property
+    def DeviceName(self):
+        return self._DeviceName
+
+    @DeviceName.setter
+    def DeviceName(self, DeviceName):
+        self._DeviceName = DeviceName
+
+    @property
+    def ChannelName(self):
+        return self._ChannelName
+
+    @ChannelName.setter
+    def ChannelName(self, ChannelName):
+        self._ChannelName = ChannelName
+
+    @property
+    def OrganizationName(self):
+        return self._OrganizationName
+
+    @OrganizationName.setter
+    def OrganizationName(self, OrganizationName):
+        self._OrganizationName = OrganizationName
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def PageNumber(self):
+        return self._PageNumber
+
+    @PageNumber.setter
+    def PageNumber(self, PageNumber):
+        self._PageNumber = PageNumber
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        self._DeviceName = params.get("DeviceName")
+        self._ChannelName = params.get("ChannelName")
+        self._OrganizationName = params.get("OrganizationName")
+        self._PageSize = params.get("PageSize")
+        self._PageNumber = params.get("PageNumber")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ListRecordBackupPlanDevicesResponse(AbstractModel):
+    """ListRecordBackupPlanDevices返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListRecordBackupPlanDevicesData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = ListRecordBackupPlanDevicesData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
 class ListRecordBackupPlansRequest(AbstractModel):
     """ListRecordBackupPlans请求参数结构体
 
     """
 
 
 class ListRecordBackupPlansResponse(AbstractModel):
     """ListRecordBackupPlans返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回数据
-        :type Data: list of ListRecordBackupPlanResponse
+        :type Data: list of ListRecordBackupPlanData
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -8607,27 +9706,21 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = []
             for item in params.get("Data"):
-                obj = ListRecordBackupPlanResponse()
+                obj = ListRecordBackupPlanData()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
-class ListRecordBackupTemplatesRequest(AbstractModel):
-    """ListRecordBackupTemplates请求参数结构体
-
-    """
-
-
-class ListRecordBackupTemplatesResponse(AbstractModel):
+class ListRecordBackupTemplatesData(AbstractModel):
     """查询录像上云模板列表返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _TemplateId: 模板ID
@@ -8731,23 +9824,73 @@
             for item in params.get("DevTimeSections"):
                 obj = RecordTemplateTimeSections()
                 obj._deserialize(item)
                 self._DevTimeSections.append(obj)
         self._Scale = params.get("Scale")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
-class ListRecordPlanChannelsRequest(AbstractModel):
-    """ListRecordPlanChannels请求参数结构体
+class ListRecordBackupTemplatesRequest(AbstractModel):
+    """ListRecordBackupTemplates请求参数结构体
 
     """
 
 
-class ListRecordPlanChannelsResponse(AbstractModel):
+class ListRecordBackupTemplatesResponse(AbstractModel):
+    """ListRecordBackupTemplates返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: list of ListRecordBackupTemplatesData
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = ListRecordBackupTemplatesData()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class ListRecordPlanChannelsData(AbstractModel):
     """用户下所有实时上云计划中的通道id列表返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _List: 用户所有计划下通道id，存在通道是为数组格式，不存在时，字段数据为空 
@@ -8763,14 +9906,142 @@
     @List.setter
     def List(self, List):
         self._List = List
 
 
     def _deserialize(self, params):
         self._List = params.get("List")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ListRecordPlanChannelsRequest(AbstractModel):
+    """ListRecordPlanChannels请求参数结构体
+
+    """
+
+
+class ListRecordPlanChannelsResponse(AbstractModel):
+    """ListRecordPlanChannels返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListRecordPlanChannelsData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = ListRecordPlanChannelsData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class ListRecordPlanDevicesData(AbstractModel):
+    """云计划下的设备通道列表返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PageNumber: 第几页
+        :type PageNumber: int
+        :param _PageSize: 当前页的设备数量
+        :type PageSize: int
+        :param _TotalCount: 本次查询的设备通道总数
+        :type TotalCount: int
+        :param _List: 设备通道信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type List: list of RecordPlanChannelInfo
+        """
+        self._PageNumber = None
+        self._PageSize = None
+        self._TotalCount = None
+        self._List = None
+
+    @property
+    def PageNumber(self):
+        return self._PageNumber
+
+    @PageNumber.setter
+    def PageNumber(self, PageNumber):
+        self._PageNumber = PageNumber
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def List(self):
+        return self._List
+
+    @List.setter
+    def List(self, List):
+        self._List = List
+
+
+    def _deserialize(self, params):
+        self._PageNumber = params.get("PageNumber")
+        self._PageSize = params.get("PageSize")
+        self._TotalCount = params.get("TotalCount")
+        if params.get("List") is not None:
+            self._List = []
+            for item in params.get("List"):
+                obj = RecordPlanChannelInfo()
+                obj._deserialize(item)
+                self._List.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class ListRecordPlanDevicesRequest(AbstractModel):
     """ListRecordPlanDevices请求参数结构体
 
     """
 
@@ -8862,78 +10133,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ListRecordPlanDevicesResponse(AbstractModel):
-    """云计划下的设备通道列表返回数据
+    """ListRecordPlanDevices返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PageNumber: 第几页
-        :type PageNumber: int
-        :param _PageSize: 当前页的设备数量
-        :type PageSize: int
-        :param _TotalCount: 本次查询的设备通道总数
-        :type TotalCount: int
-        :param _List: 设备通道信息列表
-注意：此字段可能返回 null，表示取不到有效值。
-        :type List: list of RecordPlanChannelInfo
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.ListRecordPlanDevicesData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._PageNumber = None
-        self._PageSize = None
-        self._TotalCount = None
-        self._List = None
-
-    @property
-    def PageNumber(self):
-        return self._PageNumber
-
-    @PageNumber.setter
-    def PageNumber(self, PageNumber):
-        self._PageNumber = PageNumber
-
-    @property
-    def PageSize(self):
-        return self._PageSize
-
-    @PageSize.setter
-    def PageSize(self, PageSize):
-        self._PageSize = PageSize
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def TotalCount(self):
-        return self._TotalCount
+    def Data(self):
+        return self._Data
 
-    @TotalCount.setter
-    def TotalCount(self, TotalCount):
-        self._TotalCount = TotalCount
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def List(self):
-        return self._List
+    def RequestId(self):
+        return self._RequestId
 
-    @List.setter
-    def List(self, List):
-        self._List = List
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._PageNumber = params.get("PageNumber")
-        self._PageSize = params.get("PageSize")
-        self._TotalCount = params.get("TotalCount")
-        if params.get("List") is not None:
-            self._List = []
-            for item in params.get("List"):
-                obj = RecordPlanChannelInfo()
-                obj._deserialize(item)
-                self._List.append(obj)
+        if params.get("Data") is not None:
+            self._Data = ListRecordPlanDevicesData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class ListRecordPlansRequest(AbstractModel):
     """ListRecordPlans请求参数结构体
 
     """
 
@@ -9467,14 +10710,48 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PlayRecordData(AbstractModel):
+    """本地录像播放url数据结构
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Flv: 录像播放地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Flv: str
+        """
+        self._Flv = None
+
+    @property
+    def Flv(self):
+        return self._Flv
+
+    @Flv.setter
+    def Flv(self, Flv):
+        self._Flv = Flv
+
+
+    def _deserialize(self, params):
+        self._Flv = params.get("Flv")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PlayRecordRequest(AbstractModel):
     """PlayRecord请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9549,37 +10826,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class PlayRecordResponse(AbstractModel):
-    """本地录像播放url数据结构
+    """PlayRecord返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Flv: 录像播放地址
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Flv: str
+        :param _Data: 返回结果
+        :type Data: :class:`tencentcloud.iss.v20230517.models.PlayRecordData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._Flv = None
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def Flv(self):
-        return self._Flv
+    def Data(self):
+        return self._Data
 
-    @Flv.setter
-    def Flv(self, Flv):
-        self._Flv = Flv
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._Flv = params.get("Flv")
+        if params.get("Data") is not None:
+            self._Data = PlayRecordData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class RecordPlanBaseInfo(AbstractModel):
     """实时上云计划基础信息
 
     """
 
@@ -9779,15 +11069,15 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class RecordPlanOptResponse(AbstractModel):
+class RecordPlanOptData(AbstractModel):
     """实时上云计划添加和修改的返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _PlanId: 上云计划ID
@@ -10733,85 +12023,15 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class UpdateDeviceOrganizationRequest(AbstractModel):
-    """UpdateDeviceOrganization请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _DeviceIds: 设备 ID 数组（从获取设备列表接口ListDevices中获取）
-        :type DeviceIds: list of str
-        :param _OrganizationId: 组织 ID（从查询组织接口DescribeOrganization中获取）
-        :type OrganizationId: str
-        """
-        self._DeviceIds = None
-        self._OrganizationId = None
-
-    @property
-    def DeviceIds(self):
-        return self._DeviceIds
-
-    @DeviceIds.setter
-    def DeviceIds(self, DeviceIds):
-        self._DeviceIds = DeviceIds
-
-    @property
-    def OrganizationId(self):
-        return self._OrganizationId
-
-    @OrganizationId.setter
-    def OrganizationId(self, OrganizationId):
-        self._OrganizationId = OrganizationId
-
-
-    def _deserialize(self, params):
-        self._DeviceIds = params.get("DeviceIds")
-        self._OrganizationId = params.get("OrganizationId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            property_name = name[1:]
-            if property_name in memeber_set:
-                memeber_set.remove(property_name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class UpdateDeviceOrganizationResponse(AbstractModel):
-    """UpdateDeviceOrganization返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self._RequestId = None
-
-    @property
-    def RequestId(self):
-        return self._RequestId
-
-    @RequestId.setter
-    def RequestId(self, RequestId):
-        self._RequestId = RequestId
-
-
-    def _deserialize(self, params):
-        self._RequestId = params.get("RequestId")
-
-
-class UpdateDeviceResponse(AbstractModel):
+class UpdateDeviceData(AbstractModel):
     """修改设备接口返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _DeviceId: 设备ID
@@ -11059,61 +12279,61 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class UpdateDeviceStatusRequest(AbstractModel):
-    """UpdateDeviceStatus请求参数结构体
+class UpdateDeviceOrganizationRequest(AbstractModel):
+    """UpdateDeviceOrganization请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _DeviceId: 设备 ID（从获取设备列表接口ListDevices中获取）
-        :type DeviceId: str
-        :param _Status: 禁用启用状态码（2：启用，3:禁用）
-        :type Status: int
+        :param _DeviceIds: 设备 ID 数组（从获取设备列表接口ListDevices中获取）
+        :type DeviceIds: list of str
+        :param _OrganizationId: 组织 ID（从查询组织接口DescribeOrganization中获取）
+        :type OrganizationId: str
         """
-        self._DeviceId = None
-        self._Status = None
+        self._DeviceIds = None
+        self._OrganizationId = None
 
     @property
-    def DeviceId(self):
-        return self._DeviceId
+    def DeviceIds(self):
+        return self._DeviceIds
 
-    @DeviceId.setter
-    def DeviceId(self, DeviceId):
-        self._DeviceId = DeviceId
+    @DeviceIds.setter
+    def DeviceIds(self, DeviceIds):
+        self._DeviceIds = DeviceIds
 
     @property
-    def Status(self):
-        return self._Status
+    def OrganizationId(self):
+        return self._OrganizationId
 
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
+    @OrganizationId.setter
+    def OrganizationId(self, OrganizationId):
+        self._OrganizationId = OrganizationId
 
 
     def _deserialize(self, params):
-        self._DeviceId = params.get("DeviceId")
-        self._Status = params.get("Status")
+        self._DeviceIds = params.get("DeviceIds")
+        self._OrganizationId = params.get("OrganizationId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class UpdateDeviceStatusResponse(AbstractModel):
-    """UpdateDeviceStatus返回参数结构体
+class UpdateDeviceOrganizationResponse(AbstractModel):
+    """UpdateDeviceOrganization返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -11129,72 +12349,85 @@
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._RequestId = params.get("RequestId")
 
 
-class UpdateGatewayRequest(AbstractModel):
-    """UpdateGateway请求参数结构体
+class UpdateDeviceStatusRequest(AbstractModel):
+    """UpdateDeviceStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _GatewayId: 网关索引ID（从获取网关列表ListGateways接口中获取）	
-        :type GatewayId: str
-        :param _Name: 仅支持中文、英文、数网关名称，字、_、-，长度不超过32个字符
-        :type Name: str
-        :param _Description: 网关描述，仅支持中文、英文、数字、_、-，长度不超过128个字符
-        :type Description: str
+        :param _DeviceId: 设备 ID（从获取设备列表接口ListDevices中获取）
+        :type DeviceId: str
+        :param _Status: 禁用启用状态码（2：启用，3:禁用）
+        :type Status: int
         """
-        self._GatewayId = None
-        self._Name = None
-        self._Description = None
-
-    @property
-    def GatewayId(self):
-        return self._GatewayId
-
-    @GatewayId.setter
-    def GatewayId(self, GatewayId):
-        self._GatewayId = GatewayId
+        self._DeviceId = None
+        self._Status = None
 
     @property
-    def Name(self):
-        return self._Name
+    def DeviceId(self):
+        return self._DeviceId
 
-    @Name.setter
-    def Name(self, Name):
-        self._Name = Name
+    @DeviceId.setter
+    def DeviceId(self, DeviceId):
+        self._DeviceId = DeviceId
 
     @property
-    def Description(self):
-        return self._Description
+    def Status(self):
+        return self._Status
 
-    @Description.setter
-    def Description(self, Description):
-        self._Description = Description
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
 
 
     def _deserialize(self, params):
-        self._GatewayId = params.get("GatewayId")
-        self._Name = params.get("Name")
-        self._Description = params.get("Description")
+        self._DeviceId = params.get("DeviceId")
+        self._Status = params.get("Status")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class UpdateGatewayResponse(AbstractModel):
+class UpdateDeviceStatusResponse(AbstractModel):
+    """UpdateDeviceStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
+class UpdateGatewayData(AbstractModel):
     """修改网关信息返回结果
 
     """
 
     def __init__(self):
         r"""
         :param _GatewayId: 网关索引ID
@@ -11327,17 +12560,121 @@
         self._Description = params.get("Description")
         self._ClusterId = params.get("ClusterId")
         self._ClusterName = params.get("ClusterName")
         self._Status = params.get("Status")
         self._CreatedAt = params.get("CreatedAt")
         self._Secret = params.get("Secret")
         self._Version = params.get("Version")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateGatewayRequest(AbstractModel):
+    """UpdateGateway请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _GatewayId: 网关索引ID（从获取网关列表ListGateways接口中获取）	
+        :type GatewayId: str
+        :param _Name: 仅支持中文、英文、数网关名称，字、_、-，长度不超过32个字符
+        :type Name: str
+        :param _Description: 网关描述，仅支持中文、英文、数字、_、-，长度不超过128个字符
+        :type Description: str
+        """
+        self._GatewayId = None
+        self._Name = None
+        self._Description = None
+
+    @property
+    def GatewayId(self):
+        return self._GatewayId
+
+    @GatewayId.setter
+    def GatewayId(self, GatewayId):
+        self._GatewayId = GatewayId
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+
+    def _deserialize(self, params):
+        self._GatewayId = params.get("GatewayId")
+        self._Name = params.get("Name")
+        self._Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateGatewayResponse(AbstractModel):
+    """UpdateGateway返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateGatewayData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = UpdateGatewayData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
-class UpdateOrgResponse(AbstractModel):
+class UpdateOrgData(AbstractModel):
     """修改组织接口返回数据
 
     """
 
     def __init__(self):
         r"""
         :param _OrganizationId: 组织 ID
@@ -11507,15 +12844,15 @@
     """UpdateOrganization返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回结果
-        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateOrgResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateOrgData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -11533,19 +12870,150 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = UpdateOrgResponse()
+            self._Data = UpdateOrgData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
+class UpdateRecordBackupPlanData(AbstractModel):
+    """修改录像上云计划返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _PlanId: 录像上云计划ID
+        :type PlanId: str
+        :param _PlanName: 录像上云计划名称
+        :type PlanName: str
+        :param _TemplateId: 录像上云模板ID
+        :type TemplateId: str
+        :param _Describe: 录像上云计划描述
+        :type Describe: str
+        :param _LifeCycle: 云文件生命周期
+        :type LifeCycle: :class:`tencentcloud.iss.v20230517.models.LifeCycleData`
+        :param _Status: 录像上云计划状态，1:正常使用中，0:删除中，无法使用
+        :type Status: int
+        :param _ChannelCount: 通道数量
+        :type ChannelCount: int
+        :param _CreateAt: 创建时间
+        :type CreateAt: str
+        :param _UpdateAt: 修改时间
+        :type UpdateAt: str
+        """
+        self._PlanId = None
+        self._PlanName = None
+        self._TemplateId = None
+        self._Describe = None
+        self._LifeCycle = None
+        self._Status = None
+        self._ChannelCount = None
+        self._CreateAt = None
+        self._UpdateAt = None
+
+    @property
+    def PlanId(self):
+        return self._PlanId
+
+    @PlanId.setter
+    def PlanId(self, PlanId):
+        self._PlanId = PlanId
+
+    @property
+    def PlanName(self):
+        return self._PlanName
+
+    @PlanName.setter
+    def PlanName(self, PlanName):
+        self._PlanName = PlanName
+
+    @property
+    def TemplateId(self):
+        return self._TemplateId
+
+    @TemplateId.setter
+    def TemplateId(self, TemplateId):
+        self._TemplateId = TemplateId
+
+    @property
+    def Describe(self):
+        return self._Describe
+
+    @Describe.setter
+    def Describe(self, Describe):
+        self._Describe = Describe
+
+    @property
+    def LifeCycle(self):
+        return self._LifeCycle
+
+    @LifeCycle.setter
+    def LifeCycle(self, LifeCycle):
+        self._LifeCycle = LifeCycle
+
+    @property
+    def Status(self):
+        return self._Status
+
+    @Status.setter
+    def Status(self, Status):
+        self._Status = Status
+
+    @property
+    def ChannelCount(self):
+        return self._ChannelCount
+
+    @ChannelCount.setter
+    def ChannelCount(self, ChannelCount):
+        self._ChannelCount = ChannelCount
+
+    @property
+    def CreateAt(self):
+        return self._CreateAt
+
+    @CreateAt.setter
+    def CreateAt(self, CreateAt):
+        self._CreateAt = CreateAt
+
+    @property
+    def UpdateAt(self):
+        return self._UpdateAt
+
+    @UpdateAt.setter
+    def UpdateAt(self, UpdateAt):
+        self._UpdateAt = UpdateAt
+
+
+    def _deserialize(self, params):
+        self._PlanId = params.get("PlanId")
+        self._PlanName = params.get("PlanName")
+        self._TemplateId = params.get("TemplateId")
+        self._Describe = params.get("Describe")
+        if params.get("LifeCycle") is not None:
+            self._LifeCycle = LifeCycleData()
+            self._LifeCycle._deserialize(params.get("LifeCycle"))
+        self._Status = params.get("Status")
+        self._ChannelCount = params.get("ChannelCount")
+        self._CreateAt = params.get("CreateAt")
+        self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class UpdateRecordBackupPlanModify(AbstractModel):
     """修改录像上云计划数据结构
 
     """
 
     def __init__(self):
         r"""
@@ -11693,104 +13161,128 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class UpdateRecordBackupPlanResponse(AbstractModel):
-    """修改录像上云计划返回数据
+    """UpdateRecordBackupPlan返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _PlanId: 录像上云计划ID
-        :type PlanId: str
-        :param _PlanName: 录像上云计划名称
-        :type PlanName: str
-        :param _TemplateId: 录像上云模板ID
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateRecordBackupPlanData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = UpdateRecordBackupPlanData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class UpdateRecordBackupTemplateData(AbstractModel):
+    """修改录像上云模版返回数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TemplateId: 模板ID
+注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateId: str
-        :param _Describe: 录像上云计划描述
-        :type Describe: str
-        :param _LifeCycle: 云文件生命周期
-        :type LifeCycle: :class:`tencentcloud.iss.v20230517.models.LifeCycleData`
-        :param _Status: 录像上云计划状态，1:正常使用中，0:删除中，无法使用
-        :type Status: int
-        :param _ChannelCount: 通道数量
-        :type ChannelCount: int
+        :param _TemplateName: 模板名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TemplateName: str
+        :param _TimeSections: 上云时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeSections: list of RecordTemplateTimeSections
+        :param _DevTimeSections: 录像时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DevTimeSections: list of RecordTemplateTimeSections
+        :param _Scale: 上云倍速（支持1，2，4倍速）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Scale: int
         :param _CreateAt: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
         :type CreateAt: str
-        :param _UpdateAt: 修改时间
+        :param _UpdateAt: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateAt: str
         """
-        self._PlanId = None
-        self._PlanName = None
         self._TemplateId = None
-        self._Describe = None
-        self._LifeCycle = None
-        self._Status = None
-        self._ChannelCount = None
+        self._TemplateName = None
+        self._TimeSections = None
+        self._DevTimeSections = None
+        self._Scale = None
         self._CreateAt = None
         self._UpdateAt = None
 
     @property
-    def PlanId(self):
-        return self._PlanId
-
-    @PlanId.setter
-    def PlanId(self, PlanId):
-        self._PlanId = PlanId
-
-    @property
-    def PlanName(self):
-        return self._PlanName
-
-    @PlanName.setter
-    def PlanName(self, PlanName):
-        self._PlanName = PlanName
-
-    @property
     def TemplateId(self):
         return self._TemplateId
 
     @TemplateId.setter
     def TemplateId(self, TemplateId):
         self._TemplateId = TemplateId
 
     @property
-    def Describe(self):
-        return self._Describe
+    def TemplateName(self):
+        return self._TemplateName
 
-    @Describe.setter
-    def Describe(self, Describe):
-        self._Describe = Describe
+    @TemplateName.setter
+    def TemplateName(self, TemplateName):
+        self._TemplateName = TemplateName
 
     @property
-    def LifeCycle(self):
-        return self._LifeCycle
+    def TimeSections(self):
+        return self._TimeSections
 
-    @LifeCycle.setter
-    def LifeCycle(self, LifeCycle):
-        self._LifeCycle = LifeCycle
+    @TimeSections.setter
+    def TimeSections(self, TimeSections):
+        self._TimeSections = TimeSections
 
     @property
-    def Status(self):
-        return self._Status
+    def DevTimeSections(self):
+        return self._DevTimeSections
 
-    @Status.setter
-    def Status(self, Status):
-        self._Status = Status
+    @DevTimeSections.setter
+    def DevTimeSections(self, DevTimeSections):
+        self._DevTimeSections = DevTimeSections
 
     @property
-    def ChannelCount(self):
-        return self._ChannelCount
+    def Scale(self):
+        return self._Scale
 
-    @ChannelCount.setter
-    def ChannelCount(self, ChannelCount):
-        self._ChannelCount = ChannelCount
+    @Scale.setter
+    def Scale(self, Scale):
+        self._Scale = Scale
 
     @property
     def CreateAt(self):
         return self._CreateAt
 
     @CreateAt.setter
     def CreateAt(self, CreateAt):
@@ -11802,25 +13294,39 @@
 
     @UpdateAt.setter
     def UpdateAt(self, UpdateAt):
         self._UpdateAt = UpdateAt
 
 
     def _deserialize(self, params):
-        self._PlanId = params.get("PlanId")
-        self._PlanName = params.get("PlanName")
         self._TemplateId = params.get("TemplateId")
-        self._Describe = params.get("Describe")
-        if params.get("LifeCycle") is not None:
-            self._LifeCycle = LifeCycleData()
-            self._LifeCycle._deserialize(params.get("LifeCycle"))
-        self._Status = params.get("Status")
-        self._ChannelCount = params.get("ChannelCount")
+        self._TemplateName = params.get("TemplateName")
+        if params.get("TimeSections") is not None:
+            self._TimeSections = []
+            for item in params.get("TimeSections"):
+                obj = RecordTemplateTimeSections()
+                obj._deserialize(item)
+                self._TimeSections.append(obj)
+        if params.get("DevTimeSections") is not None:
+            self._DevTimeSections = []
+            for item in params.get("DevTimeSections"):
+                obj = RecordTemplateTimeSections()
+                obj._deserialize(item)
+                self._DevTimeSections.append(obj)
+        self._Scale = params.get("Scale")
         self._CreateAt = params.get("CreateAt")
         self._UpdateAt = params.get("UpdateAt")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class UpdateRecordBackupTemplateModify(AbstractModel):
     """修改录像上云模板数据结构
 
     """
 
@@ -11942,125 +13448,50 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class UpdateRecordBackupTemplateResponse(AbstractModel):
-    """修改录像上云模版返回数据
+    """UpdateRecordBackupTemplate返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TemplateId: 模板ID
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TemplateId: str
-        :param _TemplateName: 模板名称
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TemplateName: str
-        :param _TimeSections: 上云时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type TimeSections: list of RecordTemplateTimeSections
-        :param _DevTimeSections: 录像时间段（按周进行设置，支持一天设置多个时间段，每个时间段不小于10分钟）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type DevTimeSections: list of RecordTemplateTimeSections
-        :param _Scale: 上云倍速（支持1，2，4倍速）
-注意：此字段可能返回 null，表示取不到有效值。
-        :type Scale: int
-        :param _CreateAt: 创建时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type CreateAt: str
-        :param _UpdateAt: 更新时间
-注意：此字段可能返回 null，表示取不到有效值。
-        :type UpdateAt: str
+        :param _Data: 返回数据
+        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateRecordBackupTemplateData`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
-        self._TemplateId = None
-        self._TemplateName = None
-        self._TimeSections = None
-        self._DevTimeSections = None
-        self._Scale = None
-        self._CreateAt = None
-        self._UpdateAt = None
-
-    @property
-    def TemplateId(self):
-        return self._TemplateId
-
-    @TemplateId.setter
-    def TemplateId(self, TemplateId):
-        self._TemplateId = TemplateId
-
-    @property
-    def TemplateName(self):
-        return self._TemplateName
-
-    @TemplateName.setter
-    def TemplateName(self, TemplateName):
-        self._TemplateName = TemplateName
-
-    @property
-    def TimeSections(self):
-        return self._TimeSections
-
-    @TimeSections.setter
-    def TimeSections(self, TimeSections):
-        self._TimeSections = TimeSections
-
-    @property
-    def DevTimeSections(self):
-        return self._DevTimeSections
-
-    @DevTimeSections.setter
-    def DevTimeSections(self, DevTimeSections):
-        self._DevTimeSections = DevTimeSections
-
-    @property
-    def Scale(self):
-        return self._Scale
-
-    @Scale.setter
-    def Scale(self, Scale):
-        self._Scale = Scale
+        self._Data = None
+        self._RequestId = None
 
     @property
-    def CreateAt(self):
-        return self._CreateAt
+    def Data(self):
+        return self._Data
 
-    @CreateAt.setter
-    def CreateAt(self, CreateAt):
-        self._CreateAt = CreateAt
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
 
     @property
-    def UpdateAt(self):
-        return self._UpdateAt
+    def RequestId(self):
+        return self._RequestId
 
-    @UpdateAt.setter
-    def UpdateAt(self, UpdateAt):
-        self._UpdateAt = UpdateAt
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
 
 
     def _deserialize(self, params):
-        self._TemplateId = params.get("TemplateId")
-        self._TemplateName = params.get("TemplateName")
-        if params.get("TimeSections") is not None:
-            self._TimeSections = []
-            for item in params.get("TimeSections"):
-                obj = RecordTemplateTimeSections()
-                obj._deserialize(item)
-                self._TimeSections.append(obj)
-        if params.get("DevTimeSections") is not None:
-            self._DevTimeSections = []
-            for item in params.get("DevTimeSections"):
-                obj = RecordTemplateTimeSections()
-                obj._deserialize(item)
-                self._DevTimeSections.append(obj)
-        self._Scale = params.get("Scale")
-        self._CreateAt = params.get("CreateAt")
-        self._UpdateAt = params.get("UpdateAt")
+        if params.get("Data") is not None:
+            self._Data = UpdateRecordBackupTemplateData()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
 
 
 class UpdateRecordPlanData(AbstractModel):
     """修改实时上云录像计划的数据
 
     """
 
@@ -12234,15 +13665,15 @@
     """UpdateRecordPlan返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回结果
-        :type Data: :class:`tencentcloud.iss.v20230517.models.RecordPlanOptResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.RecordPlanOptData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -12260,15 +13691,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = RecordPlanOptResponse()
+            self._Data = RecordPlanOptData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
 class UpdateRecordTemplateData(AbstractModel):
     """修改实时上云模板的请求数据结构
 
@@ -12526,15 +13957,15 @@
     """UpdateUserDevice返回参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 返回数据
-        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateDeviceResponse`
+        :type Data: :class:`tencentcloud.iss.v20230517.models.UpdateDeviceData`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
         self._RequestId = None
 
     @property
@@ -12552,15 +13983,15 @@
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         if params.get("Data") is not None:
-            self._Data = UpdateDeviceResponse()
+            self._Data = UpdateDeviceData()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
 class UpgradeGatewayRequest(AbstractModel):
     """UpgradeGateway请求参数结构体
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/tencentcloud_sdk_python_iss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iss-3.0.952/tencentcloud_sdk_python_iss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iss
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Iss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/PKG-INFO` & `tencentcloud-sdk-python-iss-3.0.952/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iss
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Iss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iss-3.0.951/README.rst` & `tencentcloud-sdk-python-iss-3.0.952/README.rst`

 * *Files identical despite different names*


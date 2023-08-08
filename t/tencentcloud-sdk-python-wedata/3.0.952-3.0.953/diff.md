# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.952.tar", last modified: Mon Aug  7 09:07:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.953.tar", last modified: Tue Aug  8 00:36:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.952.tar` & `tencentcloud-sdk-python-wedata-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      528 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1965400 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)   276930 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-08-07 09:07:25.000000 tencentcloud-sdk-python-wedata-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1968638 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)   276930 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-08 00:36:28.000000 tencentcloud-sdk-python-wedata-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/setup.py` & `tencentcloud-sdk-python-wedata-3.0.953/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-wedata',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Wedata SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -15574,14 +15574,26 @@
         :type DataEngine: str
         :param _UpdateTime: 更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
         :param _CreateTime: 创造时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateTime: str
+        :param _CycleUnit: 周期类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CycleUnit: str
+        :param _ScheduleDesc: 调度计划
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScheduleDesc: str
+        :param _DatasourceId: 数据源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatasourceId: str
+        :param _DatasourceType: 数据源类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatasourceType: str
         """
         self._TaskId = None
         self._TaskName = None
         self._WorkflowId = None
         self._WorkflowName = None
         self._Status = None
         self._TaskTypeId = None
@@ -15589,14 +15601,18 @@
         self._FolderName = None
         self._FolderId = None
         self._InCharge = None
         self._Submit = None
         self._DataEngine = None
         self._UpdateTime = None
         self._CreateTime = None
+        self._CycleUnit = None
+        self._ScheduleDesc = None
+        self._DatasourceId = None
+        self._DatasourceType = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -15702,14 +15718,46 @@
     def CreateTime(self):
         return self._CreateTime
 
     @CreateTime.setter
     def CreateTime(self, CreateTime):
         self._CreateTime = CreateTime
 
+    @property
+    def CycleUnit(self):
+        return self._CycleUnit
+
+    @CycleUnit.setter
+    def CycleUnit(self, CycleUnit):
+        self._CycleUnit = CycleUnit
+
+    @property
+    def ScheduleDesc(self):
+        return self._ScheduleDesc
+
+    @ScheduleDesc.setter
+    def ScheduleDesc(self, ScheduleDesc):
+        self._ScheduleDesc = ScheduleDesc
+
+    @property
+    def DatasourceId(self):
+        return self._DatasourceId
+
+    @DatasourceId.setter
+    def DatasourceId(self, DatasourceId):
+        self._DatasourceId = DatasourceId
+
+    @property
+    def DatasourceType(self):
+        return self._DatasourceType
+
+    @DatasourceType.setter
+    def DatasourceType(self, DatasourceType):
+        self._DatasourceType = DatasourceType
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
         self._WorkflowName = params.get("WorkflowName")
         self._Status = params.get("Status")
@@ -15718,14 +15766,18 @@
         self._FolderName = params.get("FolderName")
         self._FolderId = params.get("FolderId")
         self._InCharge = params.get("InCharge")
         self._Submit = params.get("Submit")
         self._DataEngine = params.get("DataEngine")
         self._UpdateTime = params.get("UpdateTime")
         self._CreateTime = params.get("CreateTime")
+        self._CycleUnit = params.get("CycleUnit")
+        self._ScheduleDesc = params.get("ScheduleDesc")
+        self._DatasourceId = params.get("DatasourceId")
+        self._DatasourceType = params.get("DatasourceType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -15845,14 +15897,22 @@
         :type DataEngineList: list of str
         :param _UserId: 操作人名
         :type UserId: str
         :param _OwnerId: 1
         :type OwnerId: str
         :param _TenantId: 1
         :type TenantId: str
+        :param _DatasourceIdList: 数据源ID列表
+        :type DatasourceIdList: list of str
+        :param _DatasourceTypeList: 数据源类型列表
+        :type DatasourceTypeList: list of str
+        :param _CycleUnitList: 调度单位类型列表
+        :type CycleUnitList: list of str
+        :param _CanSubmit: 是否筛选出可提交的任务
+        :type CanSubmit: bool
         """
         self._ProjectId = None
         self._Page = None
         self._Size = None
         self._StatusList = None
         self._OwnerNameList = None
         self._WorkflowIdList = None
@@ -15863,14 +15923,18 @@
         self._OwnerNameFilter = None
         self._SortItem = None
         self._SortType = None
         self._DataEngineList = None
         self._UserId = None
         self._OwnerId = None
         self._TenantId = None
+        self._DatasourceIdList = None
+        self._DatasourceTypeList = None
+        self._CycleUnitList = None
+        self._CanSubmit = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -16000,14 +16064,46 @@
     def TenantId(self):
         return self._TenantId
 
     @TenantId.setter
     def TenantId(self, TenantId):
         self._TenantId = TenantId
 
+    @property
+    def DatasourceIdList(self):
+        return self._DatasourceIdList
+
+    @DatasourceIdList.setter
+    def DatasourceIdList(self, DatasourceIdList):
+        self._DatasourceIdList = DatasourceIdList
+
+    @property
+    def DatasourceTypeList(self):
+        return self._DatasourceTypeList
+
+    @DatasourceTypeList.setter
+    def DatasourceTypeList(self, DatasourceTypeList):
+        self._DatasourceTypeList = DatasourceTypeList
+
+    @property
+    def CycleUnitList(self):
+        return self._CycleUnitList
+
+    @CycleUnitList.setter
+    def CycleUnitList(self, CycleUnitList):
+        self._CycleUnitList = CycleUnitList
+
+    @property
+    def CanSubmit(self):
+        return self._CanSubmit
+
+    @CanSubmit.setter
+    def CanSubmit(self, CanSubmit):
+        self._CanSubmit = CanSubmit
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._Page = params.get("Page")
         self._Size = params.get("Size")
         self._StatusList = params.get("StatusList")
         self._OwnerNameList = params.get("OwnerNameList")
@@ -16019,14 +16115,18 @@
         self._OwnerNameFilter = params.get("OwnerNameFilter")
         self._SortItem = params.get("SortItem")
         self._SortType = params.get("SortType")
         self._DataEngineList = params.get("DataEngineList")
         self._UserId = params.get("UserId")
         self._OwnerId = params.get("OwnerId")
         self._TenantId = params.get("TenantId")
+        self._DatasourceIdList = params.get("DatasourceIdList")
+        self._DatasourceTypeList = params.get("DatasourceTypeList")
+        self._CycleUnitList = params.get("CycleUnitList")
+        self._CanSubmit = params.get("CanSubmit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.953/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.953/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.952/README.rst` & `tencentcloud-sdk-python-wedata-3.0.953/README.rst`

 * *Files identical despite different names*


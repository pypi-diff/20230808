# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.952.tar", last modified: Mon Aug  7 08:51:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.953.tar", last modified: Tue Aug  8 00:22:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.952.tar` & `tencentcloud-sdk-python-dasb-3.0.953.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    45781 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   260513 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-07 08:51:19.000000 tencentcloud-sdk-python-dasb-3.0.952/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    45781 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   260936 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-08 00:22:59.000000 tencentcloud-sdk-python-dasb-3.0.953/README.rst
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/setup.py` & `tencentcloud-sdk-python-dasb-3.0.953/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-dasb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Dasb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/dasb/v20191018/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3846,14 +3846,16 @@
         :type Limit: int
         :param _AuthorizedUserIdSet: 有该资产访问权限的用户ID集合
         :type AuthorizedUserIdSet: list of int non-negative
         :param _ResourceIdSet: 过滤条件，资产绑定的堡垒机服务ID集合
         :type ResourceIdSet: list of str
         :param _KindSet: 可提供按照多种类型过滤, 1 - Linux, 2 - Windows, 3 - MySQL, 4 - SQLServer
         :type KindSet: list of int non-negative
+        :param _ManagedAccount: 资产是否包含托管账号。1，包含；0，不包含
+        :type ManagedAccount: str
         :param _DepartmentId: 过滤条件，可按照部门ID进行过滤
         :type DepartmentId: str
         :param _TagFilters: 过滤条件，可按照标签键、标签进行过滤。如果同时指定标签键和标签过滤条件，它们之间为“AND”的关系
         :type TagFilters: list of TagFilter
         :param _Filters: 过滤数组。支持的Name：
 BindingStatus 绑定状态
         :type Filters: list of Filter
@@ -3864,14 +3866,15 @@
         self._ApCodeSet = None
         self._Kind = None
         self._Offset = None
         self._Limit = None
         self._AuthorizedUserIdSet = None
         self._ResourceIdSet = None
         self._KindSet = None
+        self._ManagedAccount = None
         self._DepartmentId = None
         self._TagFilters = None
         self._Filters = None
 
     @property
     def IdSet(self):
         return self._IdSet
@@ -3949,14 +3952,22 @@
         return self._KindSet
 
     @KindSet.setter
     def KindSet(self, KindSet):
         self._KindSet = KindSet
 
     @property
+    def ManagedAccount(self):
+        return self._ManagedAccount
+
+    @ManagedAccount.setter
+    def ManagedAccount(self, ManagedAccount):
+        self._ManagedAccount = ManagedAccount
+
+    @property
     def DepartmentId(self):
         return self._DepartmentId
 
     @DepartmentId.setter
     def DepartmentId(self, DepartmentId):
         self._DepartmentId = DepartmentId
 
@@ -3984,14 +3995,15 @@
         self._ApCodeSet = params.get("ApCodeSet")
         self._Kind = params.get("Kind")
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._AuthorizedUserIdSet = params.get("AuthorizedUserIdSet")
         self._ResourceIdSet = params.get("ResourceIdSet")
         self._KindSet = params.get("KindSet")
+        self._ManagedAccount = params.get("ManagedAccount")
         self._DepartmentId = params.get("DepartmentId")
         if params.get("TagFilters") is not None:
             self._TagFilters = []
             for item in params.get("TagFilters"):
                 obj = TagFilter()
                 obj._deserialize(item)
                 self._TagFilters.append(obj)
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.953/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.953/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.952/README.rst` & `tencentcloud-sdk-python-dasb-3.0.953/README.rst`

 * *Files identical despite different names*


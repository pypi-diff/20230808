# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.952.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.952.tar", last modified: Mon Aug  7 09:03:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.953.tar", last modified: Tue Aug  8 00:33:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.952.tar` & `tencentcloud-sdk-python-teo-3.0.953.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60588 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)    24008 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   606776 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5399 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 09:03:56.000000 tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60588 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)    24556 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   606776 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:33:51.000000 tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-teo-3.0.952/setup.py` & `tencentcloud-sdk-python-teo-3.0.953/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-teo',
-    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Teo SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,17 @@
 
 # 不支持智能路由
 INVALIDPARAMETER_MULTIPLYLAYERNOTSUPPORTSMARTROUTING = 'InvalidParameter.MultiplyLayerNotSupportSmartRouting'
 
 # 操作配置存在不支持的预设变量。
 INVALIDPARAMETER_NOTSUPPORTTHISPRESET = 'InvalidParameter.NotSupportThisPreset'
 
+# 域名处于直接回源架构，需要保持智能加速功能的开启。
+INVALIDPARAMETER_OCDIRECTORIGINREQUIRESSMARTROUTING = 'InvalidParameter.OCDirectOriginRequiresSmartRouting'
+
 # 源站是内网IP。
 INVALIDPARAMETER_ORIGINISINNERIP = 'InvalidParameter.OriginIsInnerIp'
 
 # 修改源站操作中源站组Id必填。
 INVALIDPARAMETER_ORIGINORIGINGROUPIDISREQUIRED = 'InvalidParameter.OriginOriginGroupIdIsRequired'
 
 # 参数错误: 无效 "结束时间", 不在允许的查询范围内: [开始时间, 开始+ 7天]
@@ -418,14 +421,17 @@
 
 # DNS 记录内容错误。
 INVALIDPARAMETERVALUE_INVALIDDNSCONTENT = 'InvalidParameterValue.InvalidDNSContent'
 
 # DNS 记录名称错误。
 INVALIDPARAMETERVALUE_INVALIDDNSNAME = 'InvalidParameterValue.InvalidDNSName'
 
+# 加速域名名称不合法，加速域名应该由数字、英文字母、连词符组成，且连词符不能位于开头和结尾处。
+INVALIDPARAMETERVALUE_INVALIDDOMAINNAME = 'InvalidParameterValue.InvalidDomainName'
+
 # 加速域名状态不符合要求。
 INVALIDPARAMETERVALUE_INVALIDDOMAINSTATUS = 'InvalidParameterValue.InvalidDomainStatus'
 
 # 该同名站点标识已被占用，请重新输入。
 INVALIDPARAMETERVALUE_ZONESAMEASNAME = 'InvalidParameterValue.ZoneSameAsName'
 
 # 超过配额限制。
@@ -463,14 +469,17 @@
 
 # 域名被封禁，暂时无法操作。
 OPERATIONDENIED_DOMAINISBLOCKED = 'OperationDenied.DomainIsBlocked'
 
 # 域名尚未备案。
 OPERATIONDENIED_DOMAINNOICP = 'OperationDenied.DomainNoICP'
 
+# 站点下有域名时不允许修改服务区域。
+OPERATIONDENIED_DOMAINNUMBERISNOTZERO = 'OperationDenied.DomainNumberIsNotZero'
+
 # 站点处于停用状态，请开启后重试。
 OPERATIONDENIED_ERRZONEISALREADYPAUSED = 'OperationDenied.ErrZoneIsAlreadyPaused'
 
 # 开启高防时必须保证安全是开启状态。
 OPERATIONDENIED_INVALIDADVANCEDDEFENSESECURITYTYPE = 'OperationDenied.InvalidAdvancedDefenseSecurityType'
 
 # 开启高防必须保证站点加速区域是国内。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.953/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.952/README.rst` & `tencentcloud-sdk-python-teo-3.0.953/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.952/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.953/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.952
+Version: 3.0.953
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```


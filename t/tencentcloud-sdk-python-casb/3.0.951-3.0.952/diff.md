# Comparing `tmp/tencentcloud-sdk-python-casb-3.0.951.tar.gz` & `tmp/tencentcloud-sdk-python-casb-3.0.952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-casb-3.0.951.tar", last modified: Mon Aug  7 00:21:08 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-casb-3.0.952.tar", last modified: Mon Aug  7 08:47:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-casb-3.0.951.tar` & `tencentcloud-sdk-python-casb-3.0.952.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/casb_client.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5624 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-07 00:21:08.000000 tencentcloud-sdk-python-casb-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/casb_client.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-07 08:47:52.000000 tencentcloud-sdk-python-casb-3.0.952/README.rst
```

### Comparing `tencentcloud-sdk-python-casb-3.0.951/setup.py` & `tencentcloud-sdk-python-casb-3.0.952/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-casb',
-    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Casb SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-casb-3.0.951/tencentcloud_sdk_python_casb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-casb-3.0.952/tencentcloud_sdk_python_casb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-casb
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Casb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/casb_client.py` & `tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/casb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/errorcodes.py` & `tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.951/tencentcloud/casb/v20200507/models.py` & `tencentcloud-sdk-python-casb-3.0.952/tencentcloud/casb/v20200507/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-casb-3.0.951/tencentcloud/__init__.py` & `tencentcloud-sdk-python-casb-3.0.952/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-casb-3.0.951/PKG-INFO` & `tencentcloud-sdk-python-casb-3.0.952/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-casb
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Casb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-casb-3.0.951/README.rst` & `tencentcloud-sdk-python-casb-3.0.952/README.rst`

 * *Files identical despite different names*


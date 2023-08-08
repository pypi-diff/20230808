# Comparing `tmp/tencentcloud-sdk-python-faceid-3.0.951.tar.gz` & `tmp/tencentcloud-sdk-python-faceid-3.0.952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.951.tar", last modified: Mon Aug  7 00:26:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-faceid-3.0.952.tar", last modified: Mon Aug  7 08:53:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-faceid-3.0.951.tar` & `tencentcloud-sdk-python-faceid-3.0.952.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      528 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34162 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/faceid_client.py
--rw-r--r--   0 root         (0) root         (0)   212767 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-08-07 00:26:53.000000 tencentcloud-sdk-python-faceid-3.0.951/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      528 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/faceid_client.py
+-rw-r--r--   0 root         (0) root         (0)   212767 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-07 08:53:57.000000 tencentcloud-sdk-python-faceid-3.0.952/README.rst
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud_sdk_python_faceid.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/setup.py` & `tencentcloud-sdk-python-faceid-3.0.952/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-faceid',
-    install_requires=["tencentcloud-sdk-python-common==3.0.951"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.952"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Faceid SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/__init__.py` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-faceid-3.0.952/tencentcloud/faceid/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/PKG-INFO` & `tencentcloud-sdk-python-faceid-3.0.952/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-faceid
-Version: 3.0.951
+Version: 3.0.952
 Summary: Tencent Cloud Faceid SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-faceid-3.0.951/README.rst` & `tencentcloud-sdk-python-faceid-3.0.952/README.rst`

 * *Files identical despite different names*


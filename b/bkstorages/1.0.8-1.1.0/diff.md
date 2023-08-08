# Comparing `tmp/bkstorages-1.0.8.tar.gz` & `tmp/bkstorages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkstorages-1.0.8.tar", max compression
+gzip compressed data, was "bkstorages-1.1.0.tar", max compression
```

## Comparing `bkstorages-1.0.8.tar` & `bkstorages-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      782 2022-04-01 08:59:57.259976 bkstorages-1.0.8/bkstorages/__init__.py
--rw-r--r--   0        0        0      760 2021-09-06 02:19:29.666439 bkstorages-1.0.8/bkstorages/backends/__init__.py
--rw-r--r--   0        0        0    16651 2022-03-23 04:00:58.350506 bkstorages-1.0.8/bkstorages/backends/bkrepo.py
--rw-r--r--   0        0        0    25222 2022-03-23 04:00:58.351040 bkstorages-1.0.8/bkstorages/backends/rgw.py
--rw-r--r--   0        0        0     1859 2022-01-18 06:41:44.833102 bkstorages-1.0.8/bkstorages/exceptions.py
--rw-r--r--   0        0        0     5413 2022-04-01 08:01:31.866670 bkstorages-1.0.8/bkstorages/utils.py
--rw-r--r--   0        0        0     1537 2022-04-02 08:45:49.625512 bkstorages-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      710 2022-04-02 09:00:43.567099 bkstorages-1.0.8/setup.py
--rw-r--r--   0        0        0      662 2022-04-02 09:00:43.567520 bkstorages-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      782 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/__init__.py
+-rw-r--r--   0        0        0      760 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/__init__.py
+-rw-r--r--   0        0        0    18027 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/bkrepo.py
+-rw-r--r--   0        0        0    25222 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/backends/rgw.py
+-rw-r--r--   0        0        0     1859 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/exceptions.py
+-rw-r--r--   0        0        0     5413 2023-08-08 10:34:10.480000 bkstorages-1.1.0/bkstorages/utils.py
+-rw-r--r--   0        0        0     1521 2023-08-08 10:34:10.480000 bkstorages-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      696 2023-08-08 11:04:10.890000 bkstorages-1.1.0/setup.py
+-rw-r--r--   0        0        0      633 2023-08-08 11:04:10.890000 bkstorages-1.1.0/PKG-INFO
```

### Comparing `bkstorages-1.0.8/bkstorages/__init__.py` & `bkstorages-1.1.0/bkstorages/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,8 @@
  * Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
  * Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
  * You may obtain a copy of the License at http://opensource.org/licenses/MIT
  * Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
-__version__ = "1.0.8"
+__version__ = "1.1.0"
```

### Comparing `bkstorages-1.0.8/bkstorages/backends/__init__.py` & `bkstorages-1.1.0/bkstorages/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.0.8/bkstorages/backends/bkrepo.py` & `bkstorages-1.1.0/bkstorages/backends/bkrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
  * an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
  * specific language governing permissions and limitations under the License.
 """
 import datetime
 import logging
 from os import PathLike
 from tempfile import SpooledTemporaryFile
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import curlify
 import requests
 from django.core.exceptions import ImproperlyConfigured
 from django.core.files.base import File
 from django.core.files.storage import Storage
 from django.utils.deconstruct import deconstructible
+from django.utils.functional import cached_property
 from django.utils.timezone import localtime
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 from six.moves.urllib_parse import urljoin
 
 from bkstorages.exceptions import DownloadFailedError, ObjectAlreadyExists, RequestError, UploadFailedError
 from bkstorages.utils import clean_name, get_available_overwrite_name, get_setting, safe_join, setting
@@ -53,22 +54,30 @@
         self.bucket = bucket
         self.project = project
         # endpoint can not endswith '/'
         self.endpoint_url = endpoint_url.rstrip("/")
         self.username = username
         self.password = password
         self._max_retries = kwargs.get("max_retries", MAX_RETRIES)
+        self._session: Optional[requests.Session] = None
 
     def get_client(self) -> requests.Session:
-        session = requests.session()
+        if self._session is not None:
+            return self._session
+        self._session = session = requests.session()
         session.auth = HTTPBasicAuth(username=self.username, password=self.password)
         session.mount("http://", HTTPAdapter(max_retries=self._max_retries))
         session.mount("https://", HTTPAdapter(max_retries=self._max_retries))
         return session
 
+    @cached_property
+    def is_public(self) -> bool:
+        """当前仓库是否公开"""
+        return self.get_bucket_metadata().get("public", False)
+
     def upload_file(self, filepath: PathLike, key: str, allow_overwrite: bool = True, **kwargs):
         """上传通用制品文件
 
         :param PathLike filepath: 需要上传文件的路径
         :param str key: 文件完整路径
         :param bool allow_overwrite: 是否覆盖已存在文件
         """
@@ -156,14 +165,26 @@
         client = self.get_client()
         url = urljoin(self.endpoint_url, f'/generic/{self.project}/{self.bucket}/{key}')
         resp = client.head(url, timeout=TIMEOUT_THRESHOLD)
         if resp.status_code == 200:
             return dict(resp.headers)
         raise RequestError("Can't get file head info", code=str(resp.status_code), response=resp)
 
+    def build_download_url(self, key: str, force_download: bool = False) -> str:
+        """构造下载url
+
+        :param str key: 文件完整路径
+        :param bool force_download: 如果为true，响应体会添加Content-Disposition，强制浏览器进行下载；不加此参数，浏览器将根据情况展示文件预览
+        """
+        while key.startswith("/"):
+            key = key[1:]
+        download = "true" if force_download else "false"
+        url = urljoin(self.endpoint_url, f'/generic/{self.project}/{self.bucket}/{key}?download={download}')
+        return url
+
     def generate_presigned_url(self, key: str, expires_in: int, token_type: str = "DOWNLOAD", *args, **kwargs) -> str:
         """创建临时访问url
 
         :param str key: 授权路径
         :param int expires_in: token 有效时间，单位秒，小于等于 0 则永久有效
         :param str token_type: token类型。UPLOAD:允许上传, DOWNLOAD: 允许下载, ALL: 同时允许上传和下载。
         """
@@ -222,14 +243,22 @@
         for record in data["records"]:
             if record["folder"]:
                 directories.append(record["name"])
             else:
                 files.append(record["name"])
         return directories, files, (cur_page < total_pages)
 
+    def get_bucket_metadata(self) -> Dict:
+        """查询仓库信息"""
+        client = self.get_client()
+        url = urljoin(self.endpoint_url, f"/repository/api/repo/info/{self.project}/{self.bucket}/GENERIC")
+        resp = client.get(url)
+        data = self._validate_resp(resp)
+        return data
+
     @staticmethod
     def _validate_resp(response: requests.Response) -> Dict:
         """校验响应体"""
         try:
             logger.info("Equivalent curl command: %s", curlify.to_curl(response.request))
         except Exception:  # pylint: disable=broad-except
             pass
@@ -359,14 +388,16 @@
             return False
 
     def size(self, name):
         metadata = self.client.get_file_metadata(self._full_path(name))
         return metadata.get("Content-Length", 0)
 
     def url(self, name):
+        if self.client.is_public:
+            return self.client.build_download_url(self._full_path(name))
         # expires_in 小于等于 0 则永久有效
         return self.client.generate_presigned_url(self._full_path(name), expires_in=0)
 
     def listdir(self, path):
         return self.client.list_dir(self._full_path(name=path))
 
     # 上传文件相关
```

### Comparing `bkstorages-1.0.8/bkstorages/backends/rgw.py` & `bkstorages-1.1.0/bkstorages/backends/rgw.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.0.8/bkstorages/exceptions.py` & `bkstorages-1.1.0/bkstorages/exceptions.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.0.8/bkstorages/utils.py` & `bkstorages-1.1.0/bkstorages/utils.py`

 * *Files identical despite different names*

### Comparing `bkstorages-1.0.8/pyproject.toml` & `bkstorages-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "bkstorages"
-version = "1.0.8"
+version = "1.1.0"
 description = "File storage backends for blueking PaaS platform"
 classifiers = ["Programming Language :: Python", "Programming Language :: Python :: 3", "Framework :: Django"]
 authors = ["blueking <blueking@tencent.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<3.11"
 boto3 = ">=1.4.1"
 six = "*"
 requests = "*"
 curlify = "^2.2.1"
-pyyaml = "<6.0"
 
 [tool.poetry.dev-dependencies]
 django = ">=1.7,<3.0.0"
 six = ">=1.14"
 # For flake8 support pyproject.toml
 toml = "0.10.1"
 pyproject-flake8 = "^0.0.1-alpha.2"
```

### Comparing `bkstorages-1.0.8/setup.py` & `bkstorages-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['bkstorages', 'bkstorages.backends']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.4.1', 'curlify>=2.2.1,<3.0.0', 'pyyaml<6.0', 'requests', 'six']
+['boto3>=1.4.1', 'curlify>=2.2.1,<3.0.0', 'requests', 'six']
 
 setup_kwargs = {
     'name': 'bkstorages',
-    'version': '1.0.8',
+    'version': '1.1.0',
     'description': 'File storage backends for blueking PaaS platform',
     'long_description': None,
     'author': 'blueking',
     'author_email': 'blueking@tencent.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bkstorages-1.0.8/PKG-INFO` & `bkstorages-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: bkstorages
-Version: 1.0.8
+Version: 1.1.0
 Summary: File storage backends for blueking PaaS platform
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.6.2,<3.11
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.4.1)
 Requires-Dist: curlify (>=2.2.1,<3.0.0)
-Requires-Dist: pyyaml (<6.0)
 Requires-Dist: requests
 Requires-Dist: six
```


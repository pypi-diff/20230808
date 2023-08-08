# Comparing `tmp/pysnc-1.1.5a1.tar.gz` & `tmp/pysnc-1.1.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnc-1.1.5a1.tar", max compression
+gzip compressed data, was "pysnc-1.1.5a2.tar", max compression
```

## Comparing `pysnc-1.1.5a1.tar` & `pysnc-1.1.5a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1052 2023-05-24 22:01:02.490748 pysnc-1.1.5a1/LICENSE
--rw-r--r--   0        0        0     1590 2023-05-24 22:01:02.490748 pysnc-1.1.5a1/README.md
--rw-r--r--   0        0        0     1058 2023-05-24 22:01:27.514738 pysnc-1.1.5a1/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/__init__.py
--rw-r--r--   0        0        0       98 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/__version__.py
--rw-r--r--   0        0        0     9386 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/attachment.py
--rw-r--r--   0        0        0     3757 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/auth.py
--rw-r--r--   0        0        0    15673 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/client.py
--rw-r--r--   0        0        0     1002 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/exceptions.py
--rw-r--r--   0        0        0     3867 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/query.py
--rw-r--r--   0        0        0    38858 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/record.py
--rw-r--r--   0        0        0      846 2023-05-24 22:01:02.494748 pysnc-1.1.5a1/pysnc/utils.py
--rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 pysnc-1.1.5a1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-08-08 20:31:29.719025 pysnc-1.1.5a2/LICENSE
+-rw-r--r--   0        0        0     1590 2023-08-08 20:31:29.719025 pysnc-1.1.5a2/README.md
+-rw-r--r--   0        0        0     1079 2023-08-08 20:31:51.011492 pysnc-1.1.5a2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/__init__.py
+-rw-r--r--   0        0        0       98 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/__version__.py
+-rw-r--r--   0        0        0     9386 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/attachment.py
+-rw-r--r--   0        0        0     3757 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/auth.py
+-rw-r--r--   0        0        0    16051 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/client.py
+-rw-r--r--   0        0        0     1002 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/query.py
+-rw-r--r--   0        0        0    38858 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/record.py
+-rw-r--r--   0        0        0      846 2023-08-08 20:31:29.723024 pysnc-1.1.5a2/pysnc/utils.py
+-rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 pysnc-1.1.5a2/PKG-INFO
```

### Comparing `pysnc-1.1.5a1/LICENSE` & `pysnc-1.1.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/README.md` & `pysnc-1.1.5a2/README.md`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pyproject.toml` & `pysnc-1.1.5a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnc"
-version = "1.1.5a1"
+version = "1.1.5a2"
 description = "Python SNC (REST) API"
 authors = ["Matthew Gill <matthew.gill@servicenow.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ServiceNow/PySNC"
 documentation = "https://servicenow.github.io/PySNC/"
 keywords = ["servicenow", "snc"]
@@ -14,16 +14,17 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Operating System :: OS Independent',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = ">=2.8.1"
+requests = "2.31.0"
 requests-oauthlib = { version = ">=1.2.0", optional = true}
+certifi = "2023.7.22"
 
 [tool.poetry.extras]
 oauth = ["requests-oauthlib"]
 
 [tool.poetry.group.dev.dependencies]
 requests-oauthlib = ">=1.2.0"
 pytest = "^7.3.1"
```

### Comparing `pysnc-1.1.5a1/pysnc/attachment.py` & `pysnc-1.1.5a2/pysnc/attachment.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pysnc/auth.py` & `pysnc-1.1.5a2/pysnc/auth.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pysnc/client.py` & `pysnc-1.1.5a2/pysnc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import base64
 from typing import Callable, no_type_check
 
 from requests.cookies import MockRequest, MockResponse
 from requests.structures import CaseInsensitiveDict
 from requests.utils import get_encoding_from_headers
+from requests.adapters import HTTPAdapter, Retry
 
 from .exceptions import *
 from .record import GlideRecord
 from .attachment import Attachment
 from .utils import get_instance, MockHeaders
 from .auth import ServiceNowFlow
 
@@ -24,15 +25,15 @@
 
     :param str instance: The instance to connect to e.g. ``https://dev00000.service-now.com`` or ``dev000000``
     :param auth: Username password combination ``(name,pass)`` or :class:`pysnc.ServiceNowOAuth2` or ``requests.sessions.Session`` or ``requests.auth.AuthBase`` object
     :param proxy: HTTP(s) proxy to use as a str ``'http://proxy:8080`` or dict ``{'http':'http://proxy:8080'}``
     :param bool verify: Verify the SSL/TLS certificate OR the certificate to use. Useful if you're using a self-signed HTTPS proxy.
     :param cert: if String, path to ssl client cert file (.pem). If Tuple, (‘cert’, ‘key’) pair.
     """
-    def __init__(self, instance, auth, proxy=None, verify=None, cert=None):
+    def __init__(self, instance, auth, proxy=None, verify=None, cert=None, auto_retry=True):
         self._log = logging.getLogger(__name__)
         self.__instance = get_instance(instance)
 
         if auth is not None and cert is not None:
             raise AuthenticationException('Cannot specify both auth and cert')
         elif isinstance(auth, (list, tuple)) and len(auth) == 2:
             self.__user = auth[0]
@@ -62,14 +63,19 @@
             if verify is None:
                 verify = True  # default to verify with proxy
         if verify is not None:
             self.__session.verify = verify
 
         self.__session.headers.update(dict(Accept="application/json"))
 
+        if auto_retry is True:
+            # https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
+            retry = Retry(total=4, backoff_factor=0.2, status_forcelist=[429, 500, 503])
+            self.__session.mount(self.__instance, HTTPAdapter(max_retries=retry))
+
         self.table_api = TableAPI(self)
         self.attachment_api = AttachmentAPI(self)
         self.batch_api = BatchAPI(self)
 
     def GlideRecord(self, table, batch_size=100) -> GlideRecord:
         """
         Create a :class:`pysnc.GlideRecord` for a given table against the current client
```

### Comparing `pysnc-1.1.5a1/pysnc/exceptions.py` & `pysnc-1.1.5a2/pysnc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pysnc/query.py` & `pysnc-1.1.5a2/pysnc/query.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pysnc/record.py` & `pysnc-1.1.5a2/pysnc/record.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/pysnc/utils.py` & `pysnc-1.1.5a2/pysnc/utils.py`

 * *Files identical despite different names*

### Comparing `pysnc-1.1.5a1/PKG-INFO` & `pysnc-1.1.5a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnc
-Version: 1.1.5a1
+Version: 1.1.5a2
 Summary: Python SNC (REST) API
 Home-page: https://github.com/ServiceNow/PySNC
 License: MIT
 Keywords: servicenow,snc
 Author: Matthew Gill
 Author-email: matthew.gill@servicenow.com
 Requires-Python: >=3.8,<4.0
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: oauth
-Requires-Dist: requests (>=2.8.1)
+Requires-Dist: certifi (==2023.7.22)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: requests-oauthlib (>=1.2.0) ; extra == "oauth"
 Project-URL: Documentation, https://servicenow.github.io/PySNC/
 Project-URL: Repository, https://github.com/ServiceNow/PySNC
 Description-Content-Type: text/markdown
 
 # ServiceNow Python API
```


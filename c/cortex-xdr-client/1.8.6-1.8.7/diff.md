# Comparing `tmp/cortex_xdr_client-1.8.6.tar.gz` & `tmp/cortex_xdr_client-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_xdr_client-1.8.6.tar", max compression
+gzip compressed data, was "cortex_xdr_client-1.8.7.tar", max compression
```

## Comparing `cortex_xdr_client-1.8.6.tar` & `cortex_xdr_client-1.8.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1067 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/LICENSE
--rw-r--r--   0        0        0     3059 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/README.rst
--rw-r--r--   0        0        0       61 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/__init__.py
--rw-r--r--   0        0        0     2059 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/actions_api.py
--rw-r--r--   0        0        0     3387 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/alerts_api.py
--rw-r--r--   0        0        0     1544 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/authentication.py
--rw-r--r--   0        0        0     2376 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/base_api.py
--rw-r--r--   0        0        0     1037 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/download_api.py
--rw-r--r--   0        0        0    15639 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/endpoints_api.py
--rw-r--r--   0        0        0     5261 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/incidents_api.py
--rw-r--r--   0        0        0     1175 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/ioc_api.py
--rw-r--r--   0        0        0        0 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/__init__.py
--rw-r--r--   0        0        0      390 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/action_status.py
--rw-r--r--   0        0        0     5902 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/alerts.py
--rw-r--r--   0        0        0     2721 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/endpoints.py
--rw-r--r--   0        0        0      692 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/exceptions.py
--rw-r--r--   0        0        0     2835 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/filters.py
--rw-r--r--   0        0        0     7770 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/incidents.py
--rw-r--r--   0        0        0     2617 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/ioc.py
--rw-r--r--   0        0        0     2392 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/scripts.py
--rw-r--r--   0        0        0    12326 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/scripts_api.py
--rw-r--r--   0        0        0     5414 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/api/xql_api.py
--rw-r--r--   0        0        0     2547 2023-08-03 17:44:35.927349 cortex_xdr_client-1.8.6/cortex_xdr_client/client.py
--rw-r--r--   0        0        0      646 2023-08-03 17:44:59.971677 cortex_xdr_client-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-08 18:00:11.998844 cortex_xdr_client-1.8.7/LICENSE
+-rw-r--r--   0        0        0     3059 2023-08-08 18:00:11.998844 cortex_xdr_client-1.8.7/README.rst
+-rw-r--r--   0        0        0       61 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/__init__.py
+-rw-r--r--   0        0        0     2059 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/actions_api.py
+-rw-r--r--   0        0        0     3387 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/alerts_api.py
+-rw-r--r--   0        0        0     1544 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/authentication.py
+-rw-r--r--   0        0        0     2376 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/base_api.py
+-rw-r--r--   0        0        0      890 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/download_api.py
+-rw-r--r--   0        0        0    15782 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/endpoints_api.py
+-rw-r--r--   0        0        0     5261 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/incidents_api.py
+-rw-r--r--   0        0        0     1175 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/ioc_api.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/__init__.py
+-rw-r--r--   0        0        0      390 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/action_status.py
+-rw-r--r--   0        0        0     5902 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/alerts.py
+-rw-r--r--   0        0        0     2716 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/endpoints.py
+-rw-r--r--   0        0        0      692 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/exceptions.py
+-rw-r--r--   0        0        0     2835 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/filters.py
+-rw-r--r--   0        0        0     7770 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/incidents.py
+-rw-r--r--   0        0        0     2617 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/ioc.py
+-rw-r--r--   0        0        0     2392 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/scripts.py
+-rw-r--r--   0        0        0    12326 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/scripts_api.py
+-rw-r--r--   0        0        0     5414 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/xql_api.py
+-rw-r--r--   0        0        0     2497 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/client.py
+-rw-r--r--   0        0        0      646 2023-08-08 18:00:34.863235 cortex_xdr_client-1.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.7/PKG-INFO
```

### Comparing `cortex_xdr_client-1.8.6/LICENSE` & `cortex_xdr_client-1.8.7/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Eloi Barti
+Copyright (c) 2022-2023 Eloi Barti
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cortex_xdr_client-1.8.6/README.rst` & `cortex_xdr_client-1.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/actions_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/alerts_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/authentication.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/authentication.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/base_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/base_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/download_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/download_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from typing import Optional, Tuple
+from typing import Tuple
 
 from cortex_xdr_client.api.authentication import Authentication
 from cortex_xdr_client.api.base_api import BaseAPI
-from cortex_xdr_client.api.models.action_status import GetActionStatus
-from cortex_xdr_client.api.models.filters import new_request_data
 
 
 class DownloadAPI(BaseAPI):
     def __init__(self, auth: Authentication, fqdn: str, timeout: Tuple[int, int]) -> None:
         super(DownloadAPI, self).__init__(auth, fqdn, "download", timeout)
 
     # https://docs-cortex.paloaltonetworks.com/r/Cortex-XDR/Cortex-XDR-API-Reference/File-Retrieval-Details
```

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/endpoints_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/endpoints_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
                         ) -> Optional[ResponseActionResponse]:
         """
         Quarantine file on selected endpoints. You can select up to 1000 endpoints.
 
         :param endpoint_id_list: List of endpoint IDs.
         :param file_path: String that represents the path of the file you want to quarantine. You must enter a proper path and not symbolic links.
         :param file_hash: String that represents the file’s hash. Hash must be a valid SHA256.
+        :param incident_id: When included in the request, the Quarantine File action will appear in the Cortex XDR Incident View Timeline tab.
         :return: A ResponseActionResponse object if successful.
         """
 
         filters = [request_filter("endpoint_id_list", "in", endpoint_id_list)]
 
         request_data = new_request_data(filters=filters, other={"file_path": file_path, "file_hash": file_hash})
         if incident_id is not None:
```

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/incidents_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/ioc_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/ioc_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/alerts.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/endpoints.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Optional, Union, Any
+from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
 
 class EndpointStatus(Enum):
     """
     Enum for endpoint status
```

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/exceptions.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/filters.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/filters.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/incidents.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/ioc.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/ioc.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,20 +68,20 @@
 
 
 class IoCSeverity(str, Enum):
     """
     IoC Severity Enum
     Represents the indicator's severity. Valid values are: informational, low, medium, high, critical, or unknown
     """
-    informational: str = 'informational'
-    low: str = 'low'
-    medium: str = 'medium'
-    high: str = 'high'
-    critical: str = 'critical'
-    unknown: str = 'unknown'
+    informational: str = 'INFORMATIONAL'
+    low: str = 'LOW'
+    medium: str = 'MEDIUM'
+    high: str = 'HIGH'
+    critical: str = 'CRITICAL'
+    unknown: str = 'UNKNOWN'
 
 
 class IoCType(str, Enum):
     """
     IoC Type Enum
     Represents the type of indicator. Allowed values:HASH, IP, DOMAIN_NAME, FILENAME
     """
```

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/models/scripts.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/scripts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/scripts_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/scripts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/api/xql_api.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/api/xql_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.6/cortex_xdr_client/client.py` & `cortex_xdr_client-1.8.7/cortex_xdr_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     download_api: DownloadAPI
     ioc_api: IocAPI
 
     def __init__(self, auth: Authentication, fqdn: str, default_timeout: Tuple[int, int] = (10, 60)) -> None:
         """
         Constructor of the CortexXDRClient class. This class is used to interact with the Cortex XDR API.
         :param auth: The Authentication object containing type
-        :param api_key: The API key value to use.
         :param fqdn: The fully qualified domain name of the Cortex XDR server.
         :param default_timeout: The default timeout for API calls.
         """
         self.incidents_api = IncidentsAPI(auth=auth,
                                           fqdn=fqdn,
                                           timeout=default_timeout)
         self.alerts_api = AlertsAPI(auth=auth,
```

### Comparing `cortex_xdr_client-1.8.6/pyproject.toml` & `cortex_xdr_client-1.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cortex-xdr-client"
 packages= [
     { include = "cortex_xdr_client", from="." },
 ]
-version = "v1.8.6"
+version = "v1.8.7"
 description = "API client for Cortex XDR Prevent"
 authors = ["ebarti"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ebarti/cortex-xdr-client"
 repository = "https://github.com/ebarti/cortex-xdr-client"
```

### Comparing `cortex_xdr_client-1.8.6/PKG-INFO` & `cortex_xdr_client-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortex-xdr-client
-Version: 1.8.6
+Version: 1.8.7
 Summary: API client for Cortex XDR Prevent
 Home-page: https://github.com/ebarti/cortex-xdr-client
 License: MIT
 Author: ebarti
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


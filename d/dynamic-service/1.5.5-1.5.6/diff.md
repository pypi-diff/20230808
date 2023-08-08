# Comparing `tmp/dynamic-service-1.5.5.tar.gz` & `tmp/dynamic-service-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-service-1.5.5.tar", last modified: Mon Aug  7 17:58:55 2023, max compression
+gzip compressed data, was "dynamic-service-1.5.6.tar", last modified: Tue Aug  8 07:47:26 2023, max compression
```

## Comparing `dynamic-service-1.5.5.tar` & `dynamic-service-1.5.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.220658 dynamic-service-1.5.5/
--rw-rw-rw-   0        0        0      236 2023-08-07 17:58:54.000000 dynamic-service-1.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2023 2023-08-07 17:58:55.220658 dynamic-service-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/README.md
--rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/build.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.196658 dynamic-service-1.5.5/dynamic_service/
--rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/dynamic_service/base.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.216658 dynamic-service-1.5.5/dynamic_service/endpoints/
--rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/dynamic_service/endpoints/__init__.py
--rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.5/dynamic_service/endpoints/data.py
--rw-rw-rw-   0        0        0     9485 2023-07-25 09:26:13.000000 dynamic-service-1.5.5/dynamic_service/endpoints/engine.py
--rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.5/dynamic_service/endpoints/exceptions.py
--rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.5/dynamic_service/endpoints/process.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.218658 dynamic-service-1.5.5/dynamic_service/service/
--rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/dynamic_service/service/__init__.py
--rw-rw-rw-   0        0        0    21281 2023-08-07 17:58:36.000000 dynamic-service-1.5.5/dynamic_service/service/rest.py
--rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.5/dynamic_service/service/sockets.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.189906 dynamic-service-1.5.5/dynamic_service/source/
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.189906 dynamic-service-1.5.5/dynamic_service/source/assets/
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.219658 dynamic-service-1.5.5/dynamic_service/source/assets/icon/
--rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/dynamic_service/source/assets/icon/icon.ico
--rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.5/dynamic_service/source/assets/icon/icon.png
-drwxrwxrwx   0        0        0        0 2023-08-07 17:58:55.212689 dynamic-service-1.5.5/dynamic_service.egg-info/
--rw-rw-rw-   0        0        0     2023 2023-08-07 17:58:55.000000 dynamic-service-1.5.5/dynamic_service.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-08-07 17:58:55.000000 dynamic-service-1.5.5/dynamic_service.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 17:58:55.000000 dynamic-service-1.5.5/dynamic_service.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-08-07 17:58:55.000000 dynamic-service-1.5.5/dynamic_service.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 17:58:55.000000 dynamic-service-1.5.5/dynamic_service.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      627 2023-08-07 17:58:54.000000 dynamic-service-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.5/requirements-dev.txt
--rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 17:58:55.220658 dynamic-service-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-08-07 17:58:49.000000 dynamic-service-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.921649 dynamic-service-1.5.6/
+-rw-rw-rw-   0        0        0      236 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2023 2023-08-08 07:47:26.921649 dynamic-service-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1226 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/README.md
+-rw-rw-rw-   0        0        0    12920 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/build.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.859024 dynamic-service-1.5.6/dynamic_service/
+-rw-rw-rw-   0        0        0     1439 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/dynamic_service/base.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.897787 dynamic-service-1.5.6/dynamic_service/endpoints/
+-rw-rw-rw-   0        0        0      210 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/dynamic_service/endpoints/__init__.py
+-rw-rw-rw-   0        0        0     2539 2023-07-03 14:24:04.000000 dynamic-service-1.5.6/dynamic_service/endpoints/data.py
+-rw-rw-rw-   0        0        0    10271 2023-08-08 07:47:19.000000 dynamic-service-1.5.6/dynamic_service/endpoints/engine.py
+-rw-rw-rw-   0        0        0     1569 2023-07-03 06:52:10.000000 dynamic-service-1.5.6/dynamic_service/endpoints/exceptions.py
+-rw-rw-rw-   0        0        0     1608 2023-07-03 06:51:55.000000 dynamic-service-1.5.6/dynamic_service/endpoints/process.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.915430 dynamic-service-1.5.6/dynamic_service/service/
+-rw-rw-rw-   0        0        0      106 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/dynamic_service/service/__init__.py
+-rw-rw-rw-   0        0        0    21281 2023-08-07 17:58:36.000000 dynamic-service-1.5.6/dynamic_service/service/rest.py
+-rw-rw-rw-   0        0        0     3419 2023-07-08 16:21:14.000000 dynamic-service-1.5.6/dynamic_service/service/sockets.py
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.847513 dynamic-service-1.5.6/dynamic_service/source/
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.847513 dynamic-service-1.5.6/dynamic_service/source/assets/
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.920619 dynamic-service-1.5.6/dynamic_service/source/assets/icon/
+-rw-rw-rw-   0        0        0     2834 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/dynamic_service/source/assets/icon/icon.ico
+-rw-rw-rw-   0        0        0    27619 2023-07-01 09:47:05.000000 dynamic-service-1.5.6/dynamic_service/source/assets/icon/icon.png
+drwxrwxrwx   0        0        0        0 2023-08-08 07:47:26.874606 dynamic-service-1.5.6/dynamic_service.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/dynamic_service.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/dynamic_service.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/dynamic_service.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/dynamic_service.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/dynamic_service.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      627 2023-08-08 07:47:26.000000 dynamic-service-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2023-07-08 15:54:50.000000 dynamic-service-1.5.6/requirements-dev.txt
+-rw-rw-rw-   0        0        0       76 2023-07-08 15:54:50.000000 dynamic-service-1.5.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 07:47:26.921649 dynamic-service-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-08-08 07:47:08.000000 dynamic-service-1.5.6/setup.py
```

### Comparing `dynamic-service-1.5.5/PKG-INFO` & `dynamic-service-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.5
+Version: 1.5.6
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.5/README.md` & `dynamic-service-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/build.py` & `dynamic-service-1.5.6/build.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/base.py` & `dynamic-service-1.5.6/dynamic_service/base.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/endpoints/data.py` & `dynamic-service-1.5.6/dynamic_service/endpoints/data.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/endpoints/engine.py` & `dynamic-service-1.5.6/dynamic_service/endpoints/engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # engine.py
 
 from functools import wraps
 from typing import (
-    List, Any, Dict, Optional,
+    List, Any, Dict, Optional, Union, Type,
     Tuple, Callable, Iterable, TypeVar, Generic
 )
 
 from attrs import define, field
 
 from fastapi.openapi.docs import get_swagger_ui_html, HTMLResponse
 
@@ -14,15 +14,16 @@
 
 from dynamic_service.endpoints.data import DOCS
 
 __all__ = [
     "BaseEndpoint",
     "DocsEndpoint",
     "Record",
-    "valid_endpoints"
+    "valid_endpoints",
+    "build_endpoints"
 ]
 
 @define(repr=False)
 @represent
 class Record:
     """A class to represent a result object for commands and conditions calls."""
 
@@ -330,8 +331,33 @@
                 f"paths as values, or an iterable object with endpoint objects, "
                 f"not: {endpoints}"
             )
         # end try
     # end if
 
     return endpoints
-# end valid_endpoints
+# end valid_endpoints
+
+def build_endpoints(
+    endpoints: Iterable[Union[BaseEndpoint, Type[BaseEndpoint]]],
+    service: Optional[_ServiceType] = None
+) -> List[BaseEndpoint[_ServiceType, ..., ...]]:
+    """
+    Builds the endpoints for the service.
+
+    :param service: The service for the endpoints.
+    :param endpoints: The bases of endpoints for the service.
+
+    :return: The built endpoints.
+    """
+
+    return [
+        (
+            endpoint(
+                path=endpoint.PATH,
+                methods=endpoint.METHODS,
+                service=service,
+                options=dict(response_model=None)
+            ) if issubclass(endpoint, BaseEndpoint) else endpoint
+        ) for endpoint in endpoints
+    ]
+# end build_endpoints
```

### Comparing `dynamic-service-1.5.5/dynamic_service/endpoints/exceptions.py` & `dynamic-service-1.5.6/dynamic_service/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/endpoints/process.py` & `dynamic-service-1.5.6/dynamic_service/endpoints/process.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/service/rest.py` & `dynamic-service-1.5.6/dynamic_service/service/rest.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/service/sockets.py` & `dynamic-service-1.5.6/dynamic_service/service/sockets.py`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/source/assets/icon/icon.ico` & `dynamic-service-1.5.6/dynamic_service/source/assets/icon/icon.ico`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service/source/assets/icon/icon.png` & `dynamic-service-1.5.6/dynamic_service/source/assets/icon/icon.png`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/dynamic_service.egg-info/PKG-INFO` & `dynamic-service-1.5.6/dynamic_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-service
-Version: 1.5.5
+Version: 1.5.6
 Summary: A framework for developing responsive, live and dynamic REST APIs with python.
 Home-page: https://github.com/Shahaf-F-S/dynamic-service
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dynamic-service-1.5.5/dynamic_service.egg-info/SOURCES.txt` & `dynamic-service-1.5.6/dynamic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-service-1.5.5/pyproject.toml` & `dynamic-service-1.5.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'dynamic-service'
-version = '1.5.5'
+version = '1.5.6'
 description = 'A framework for developing responsive, live and dynamic REST APIs with python.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `dynamic-service-1.5.5/setup.py` & `dynamic-service-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "dynamic_service/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='dynamic-service',
-        version='1.5.5',
+        version='1.5.6',
         description=(
             "A framework for developing responsive, "
             "live and dynamic REST APIs with python."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```


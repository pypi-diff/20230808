# Comparing `tmp/cumplo_common-0.1.0.tar.gz` & `tmp/cumplo_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumplo_common-0.1.0.tar", max compression
+gzip compressed data, was "cumplo_common-0.1.1.tar", max compression
```

## Comparing `cumplo_common-0.1.0.tar` & `cumplo_common-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    34523 2023-08-04 22:48:00.735339 cumplo_common-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133087 cumplo_common-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133037 cumplo_common-0.1.0/cumplo_common/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 21:08:12.823188 cumplo_common-0.1.0/cumplo_common/database/__init__.py
--rw-r--r--   0        0        0     5389 2023-08-05 21:18:50.983861 cumplo_common-0.1.0/cumplo_common/database/firestore.py
--rw-r--r--   0        0        0     1504 2023-08-05 21:24:45.780295 cumplo_common-0.1.0/cumplo_common/integrations/cloud_tasks.py
--rw-r--r--   0        0        0      696 2023-08-05 21:26:45.358044 cumplo_common-0.1.0/cumplo_common/middlewares/authentication.py
--rw-r--r--   0        0        0      372 2023-08-05 21:26:47.630268 cumplo_common-0.1.0/cumplo_common/middlewares/authorization.py
--rw-r--r--   0        0        0        0 2023-08-05 21:08:18.258596 cumplo_common-0.1.0/cumplo_common/models/__init__.py
--rw-r--r--   0        0        0     1669 2023-08-04 23:07:25.517655 cumplo_common-0.1.0/cumplo_common/models/configuration.py
--rw-r--r--   0        0        0      402 2023-08-04 23:11:28.896994 cumplo_common-0.1.0/cumplo_common/models/notification.py
--rw-r--r--   0        0        0      517 2023-08-04 23:09:27.965311 cumplo_common-0.1.0/cumplo_common/models/user.py
--rw-r--r--   0        0        0        0 2023-08-05 21:08:31.777792 cumplo_common-0.1.0/cumplo_common/utils/__init__.py
--rw-r--r--   0        0        0      369 2023-08-05 21:24:15.107625 cumplo_common-0.1.0/cumplo_common/utils/constants.py
--rw-r--r--   0        0        0      189 2023-08-05 20:59:13.277955 cumplo_common-0.1.0/cumplo_common/utils/currency.py
--rw-r--r--   0        0        0      701 2023-08-05 20:58:12.453196 cumplo_common-0.1.0/cumplo_common/utils/text.py
--rw-r--r--   0        0        0      677 2023-08-05 21:25:53.692242 cumplo_common-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 cumplo_common-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-04 22:48:00.735339 cumplo_common-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133087 cumplo_common-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 22:49:44.133037 cumplo_common-0.1.1/cumplo_common/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:12.823188 cumplo_common-0.1.1/cumplo_common/database/__init__.py
+-rw-r--r--   0        0        0     5389 2023-08-05 21:18:50.983861 cumplo_common-0.1.1/cumplo_common/database/firestore.py
+-rw-r--r--   0        0        0     1504 2023-08-05 21:24:45.780295 cumplo_common-0.1.1/cumplo_common/integrations/cloud_tasks.py
+-rw-r--r--   0        0        0      694 2023-08-07 22:56:57.754118 cumplo_common-0.1.1/cumplo_common/middlewares/authentication.py
+-rw-r--r--   0        0        0      372 2023-08-05 21:26:47.630268 cumplo_common-0.1.1/cumplo_common/middlewares/authorization.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:18.258596 cumplo_common-0.1.1/cumplo_common/models/__init__.py
+-rw-r--r--   0        0        0     1669 2023-08-04 23:07:25.517655 cumplo_common-0.1.1/cumplo_common/models/configuration.py
+-rw-r--r--   0        0        0      402 2023-08-04 23:11:28.896994 cumplo_common-0.1.1/cumplo_common/models/notification.py
+-rw-r--r--   0        0        0      517 2023-08-04 23:09:27.965311 cumplo_common-0.1.1/cumplo_common/models/user.py
+-rw-r--r--   0        0        0        0 2023-08-05 21:08:31.777792 cumplo_common-0.1.1/cumplo_common/utils/__init__.py
+-rw-r--r--   0        0        0      369 2023-08-05 21:24:15.107625 cumplo_common-0.1.1/cumplo_common/utils/constants.py
+-rw-r--r--   0        0        0      189 2023-08-05 20:59:13.277955 cumplo_common-0.1.1/cumplo_common/utils/currency.py
+-rw-r--r--   0        0        0      701 2023-08-05 20:58:12.453196 cumplo_common-0.1.1/cumplo_common/utils/text.py
+-rw-r--r--   0        0        0      677 2023-08-07 23:08:18.809244 cumplo_common-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 cumplo_common-0.1.1/PKG-INFO
```

### Comparing `cumplo_common-0.1.0/LICENSE` & `cumplo_common-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/cumplo_common/database/firestore.py` & `cumplo_common-0.1.1/cumplo_common/database/firestore.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/cumplo_common/integrations/cloud_tasks.py` & `cumplo_common-0.1.1/cumplo_common/integrations/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/cumplo_common/middlewares/authentication.py` & `cumplo_common-0.1.1/cumplo_common/middlewares/authentication.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fastapi import Header
 from fastapi.exceptions import HTTPException
 from fastapi.requests import Request
 
 from cumplo_common.database.firestore import firestore_client
 
 
-async def authenticate(request: Request, x_api_key: Annotated[str | None, Header()] = None) -> None:
+async def authenticate(request: Request, x_api_key: Annotated[str | None, Header] = None) -> None:
     """
     Authenticates a request.
     """
     if not x_api_key:
         raise HTTPException(status_code=HTTPStatus.UNAUTHORIZED)
 
     try:
```

### Comparing `cumplo_common-0.1.0/cumplo_common/models/configuration.py` & `cumplo_common-0.1.1/cumplo_common/models/configuration.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/cumplo_common/models/user.py` & `cumplo_common-0.1.1/cumplo_common/models/user.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/cumplo_common/utils/text.py` & `cumplo_common-0.1.1/cumplo_common/utils/text.py`

 * *Files identical despite different names*

### Comparing `cumplo_common-0.1.0/pyproject.toml` & `cumplo_common-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cumplo-common"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python library that contains all common logic throughout Cumplo API project"
 authors = ["Cristobal Sfeir <cnsfeir@uc.cl>"]
 readme = "README.md"
 packages = [{ include = "cumplo_common" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cumplo_common-0.1.0/PKG-INFO` & `cumplo_common-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumplo-common
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library that contains all common logic throughout Cumplo API project
 Author: Cristobal Sfeir
 Author-email: cnsfeir@uc.cl
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
```


# Comparing `tmp/fastapi_authtools-0.4.tar.gz` & `tmp/fastapi_authtools-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_authtools-0.4.tar", last modified: Mon Jul 17 06:23:49 2023, max compression
+gzip compressed data, was "fastapi_authtools-0.5.tar", last modified: Tue Aug  8 09:39:20 2023, max compression
```

## Comparing `fastapi_authtools-0.4.tar` & `fastapi_authtools-0.5.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.4/LICENSE
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4351 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3678 2023-07-17 06:19:38.000000 fastapi_authtools-0.4/README.md
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.827398 fastapi_authtools-0.4/fastapi_authtools/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3162 2023-07-16 19:19:10.000000 fastapi_authtools-0.4/fastapi_authtools/__init__.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2126 2023-07-16 18:52:36.000000 fastapi_authtools-0.4/fastapi_authtools/backend.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1015 2023-07-16 18:52:36.000000 fastapi_authtools-0.4/fastapi_authtools/exceptions.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1048 2023-07-16 18:35:50.000000 fastapi_authtools-0.4/fastapi_authtools/middleware.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.4/fastapi_authtools/models.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      912 2023-07-15 16:18:33.000000 fastapi_authtools-0.4/fastapi_authtools/token.py
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.4/fastapi_authtools/user.py
-drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/fastapi_authtools.egg-info/
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4351 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/PKG-INFO
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      489 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/SOURCES.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/dependency_links.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/not-zip-safe
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       20 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/requires.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       18 2023-07-17 06:23:49.000000 fastapi_authtools-0.4/fastapi_authtools.egg-info/top_level.txt
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      639 2023-07-17 06:22:42.000000 fastapi_authtools-0.4/pyproject.toml
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-07-17 06:23:49.831397 fastapi_authtools-0.4/setup.cfg
--rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      538 2023-07-17 06:23:22.000000 fastapi_authtools-0.4/setup.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1073 2023-07-13 17:55:37.000000 fastapi_authtools-0.5/LICENSE
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4023 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3678 2023-07-17 06:19:38.000000 fastapi_authtools-0.5/README.md
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/fastapi_authtools/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3177 2023-08-08 08:52:53.000000 fastapi_authtools-0.5/fastapi_authtools/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2107 2023-08-08 08:40:13.000000 fastapi_authtools-0.5/fastapi_authtools/backend.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1005 2023-08-08 08:41:22.000000 fastapi_authtools-0.5/fastapi_authtools/exceptions.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1048 2023-07-16 18:35:50.000000 fastapi_authtools-0.5/fastapi_authtools/middleware.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      681 2023-07-14 05:43:40.000000 fastapi_authtools-0.5/fastapi_authtools/models.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1052 2023-08-08 08:52:53.000000 fastapi_authtools-0.5/fastapi_authtools/token.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      988 2023-07-13 17:55:37.000000 fastapi_authtools-0.5/fastapi_authtools/user.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/fastapi_authtools.egg-info/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     4023 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/PKG-INFO
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      854 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        1 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/not-zip-safe
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       45 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/requires.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       24 2023-08-08 09:39:20.000000 fastapi_authtools-0.5/fastapi_authtools.egg-info/top_level.txt
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      639 2023-08-08 09:31:09.000000 fastapi_authtools-0.5/pyproject.toml
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)       38 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/setup.cfg
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      607 2023-08-08 09:38:27.000000 fastapi_authtools-0.5/setup.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.880467 fastapi_authtools-0.5/tests/
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/tests/test_api/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 07:27:39.000000 fastapi_authtools-0.5/tests/test_api/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2358 2023-08-08 08:30:55.000000 fastapi_authtools-0.5/tests/test_api/app.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      937 2023-08-08 08:36:16.000000 fastapi_authtools-0.5/tests/test_api/conftest.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     3121 2023-08-08 08:44:03.000000 fastapi_authtools-0.5/tests/test_api/test_auth.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/tests/test_classes/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 08:44:57.000000 fastapi_authtools-0.5/tests/test_classes/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      491 2023-08-08 08:47:24.000000 fastapi_authtools-0.5/tests/test_classes/conftest.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      387 2023-07-14 17:17:26.000000 fastapi_authtools-0.5/tests/test_classes/test_middleware.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     1018 2023-08-08 08:57:20.000000 fastapi_authtools-0.5/tests/test_classes/test_token.py
+drwxrwxr-x   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 09:39:20.884467 fastapi_authtools-0.5/tests/test_fullstack/
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)        0 2023-08-08 08:57:40.000000 fastapi_authtools-0.5/tests/test_fullstack/__init__.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2731 2023-08-08 09:10:57.000000 fastapi_authtools-0.5/tests/test_fullstack/app.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)      899 2023-08-08 09:29:55.000000 fastapi_authtools-0.5/tests/test_fullstack/conftest.py
+-rw-rw-r--   0 michael7nightingale  (1000) michael7nightingale  (1000)     2136 2023-08-08 09:28:40.000000 fastapi_authtools-0.5/tests/test_fullstack/test_auth.py
```

### Comparing `fastapi_authtools-0.4/LICENSE` & `fastapi_authtools-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.4/PKG-INFO` & `fastapi_authtools-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi_authtools
-Version: 0.4
-Summary: FastAPI authentication package.
-Home-page: https://github.com/michael7nightinglae/fastapi_authtools
+Version: 0.5
+Summary: Simple and comfortable FastAPI JWT authentication.
+Home-page: https://github.com/michael7nightingale/fastapi_authtools
 Author: Michael Nightingale
-Author-email: Michael Nightingale <suslanchikmopl@gmail.com>
+Author-email: suslanchikmopl@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/michael7nightinglae/fastapi_authtools
-Project-URL: Bug Tracker, https://github.com/michael7nightinglae/fastapi_authtools/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+Platform: UNKNOWN
+Description-Content-Type: Markdown
 License-File: LICENSE
 
 # FastAPI auth library.
 
 It`s simple to connect to your project. Just make user_data verification, and library will manage JWT-tokens.
 
 ## Installation
@@ -144,7 +139,9 @@
     app.state.auth_manager.login(response, user)
     return response
 ```
 
 
 Auth manager adds authentication middleware to your application instance and uses authentication backends to treat token and
 request user instance. 
+
+
```

### Comparing `fastapi_authtools-0.4/README.md` & `fastapi_authtools-0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.4/fastapi_authtools/__init__.py` & `fastapi_authtools-0.5/fastapi_authtools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from starlette.responses import JSONResponse
 from pydantic import BaseModel
 from typing import Awaitable, List, Callable, Type
 from functools import wraps
 
 from .middleware import AuthenticationMiddleware
 from .token import encode_jwt_token
-from .exceptions import raise_credentials_error, raise_data_model_exception
+from .exceptions import raise_credentials_not_provided, raise_data_model_exception
 from .models import UserModel
 
 
 class JWTConfig(BaseModel):
     """JWT-tokens "configuration model."""
     secret_key: str
     algorithm: str
@@ -69,29 +69,29 @@
             jwt_config=self.jwt_config,
             excluded_urls=self.excluded_urls,
             use_cookies=self.use_cookies,
             user_model=self.user_model,
             auth_error_handler=self.auth_error_handler
         )
 
-    def create_token(self, data: Type[BaseModel]) -> str:
+    def create_token(self, data: dict | BaseModel) -> str:
         """Create token function to user in token get endpoint."""
         return encode_jwt_token(
             user_data=data,
             secret_key=self.jwt_config.secret_key,
             expire_minutes=self.jwt_config.expire_minutes,
             algorithm=self.jwt_config.algorithm
         )
 
 
 def login_required(func):
     """Decorator with makes view allowed only for authenticated users."""
     @wraps(func)
     async def inner_view(request: Request, *args, **kwargs):
         if request.user is None:
-            raise_credentials_error()
+            raise_credentials_not_provided()
         response = func(request, *args, **kwargs)
         if isinstance(response, Awaitable):
             response = await response
         return response
 
     return inner_view
```

### Comparing `fastapi_authtools-0.4/fastapi_authtools/backend.py` & `fastapi_authtools-0.5/fastapi_authtools/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from starlette import authentication
 from starlette.requests import HTTPConnection
 from pydantic import typing, BaseModel
 from typing import Type
 
-from .exceptions import invalid_credentials_message
+from .exceptions import Responses
 from .token import decode_jwt_token
 
 
 class AuthenticationBackend(authentication.AuthenticationBackend):
     def __init__(
             self,
             jwt_config: Type[BaseModel],
@@ -30,19 +30,18 @@
         user_data = decode_jwt_token(
             token=token,
             secret_key=self.jwt_config.secret_key,
             algorithm=self.jwt_config.algorithm
         )
         if user_data is None:
             return scopes, None
-
         try:
             user = self.user_model(**user_data)
         except:
-            raise authentication.AuthenticationError(invalid_credentials_message())
+            raise authentication.AuthenticationError(Responses.invalid_credentials)
         else:
             return scopes, user
 
     def get_token(self, conn: HTTPConnection) -> str:
         if self.use_cookies:
             token = conn.cookies.get("access-token")
             return token
```

### Comparing `fastapi_authtools-0.4/fastapi_authtools/exceptions.py` & `fastapi_authtools-0.5/fastapi_authtools/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 from fastapi import HTTPException
+from enum import Enum
 
 
-def credentials_error_message() -> str:
-    return "Auth credentials are not provided."
-
-
-def permissions_error_message() -> str:
-    return "You don`t have permissions."
+class Responses(str, Enum):
+    credentials_not_provided = "Auth credentials are not provided."
+    permission_required = "You don`t have permissions."
+    invalid_credentials = "Invalid credentials provided."
 
 
 def data_model_exception_message(expected, got) -> str:
     return f"""Invalid data model got: {got}. Expected: {expected}."""
 
 
-def invalid_credentials_message() -> str:
-    return "Invalid credentials provided."
-
-
-def raise_credentials_error() -> str:
+def raise_credentials_not_provided() -> str:
     raise HTTPException(
         status_code=401,
-        detail=credentials_error_message()
+        detail=Responses.credentials_not_provided
     )
 
 
 def raise_permissions_error() -> str:
     raise HTTPException(
         status_code=403,
-        detail=permissions_error_message()
+        detail=Responses.permission_required
     )
 
 
 def raise_data_model_exception(expected, got) -> str:
     raise HTTPException(
         status_code=400,
         detail=data_model_exception_message(expected, got)
     )
 
 
 def raise_invalid_credentials() -> str:
     raise HTTPException(
         status_code=400,
-        detail=invalid_credentials_message()
+        detail=Responses.invalid_credentials
     )
```

### Comparing `fastapi_authtools-0.4/fastapi_authtools/middleware.py` & `fastapi_authtools-0.5/fastapi_authtools/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.4/fastapi_authtools/models.py` & `fastapi_authtools-0.5/fastapi_authtools/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.4/fastapi_authtools/token.py` & `fastapi_authtools-0.5/fastapi_authtools/token.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from datetime import datetime, timedelta
 from typing import Type
 from jose import JWTError, jwt
 from pydantic import BaseModel, ValidationError
 
 
 def encode_jwt_token(
-        user_data: dict | Type[BaseModel],
+        user_data: dict | BaseModel,
         secret_key: str,
         algorithm: str,
         expire_minutes: int
 ) -> str:
     if isinstance(user_data, BaseModel):
-        user_data = user_data.dict()
+        user_data = user_data.model_dump()
+    elif isinstance(user_data, dict):
+        pass
+    else:
+        raise TypeError("Data to encode must be either `dict` ot `BaseModel`")
     user_data.update(exp=datetime.now() + timedelta(minutes=expire_minutes))
     token = jwt.encode(
         user_data,
         key=secret_key,
         algorithm=algorithm
     )
     return token
```

### Comparing `fastapi_authtools-0.4/fastapi_authtools/user.py` & `fastapi_authtools-0.5/fastapi_authtools/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_authtools-0.4/fastapi_authtools.egg-info/PKG-INFO` & `fastapi_authtools-0.5/fastapi_authtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: fastapi-authtools
-Version: 0.4
-Summary: FastAPI authentication package.
-Home-page: https://github.com/michael7nightinglae/fastapi_authtools
+Version: 0.5
+Summary: Simple and comfortable FastAPI JWT authentication.
+Home-page: https://github.com/michael7nightingale/fastapi_authtools
 Author: Michael Nightingale
-Author-email: Michael Nightingale <suslanchikmopl@gmail.com>
+Author-email: suslanchikmopl@gmail.com
 License: MIT
-Project-URL: Homepage, https://github.com/michael7nightinglae/fastapi_authtools
-Project-URL: Bug Tracker, https://github.com/michael7nightinglae/fastapi_authtools/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
+Platform: UNKNOWN
+Description-Content-Type: Markdown
 License-File: LICENSE
 
 # FastAPI auth library.
 
 It`s simple to connect to your project. Just make user_data verification, and library will manage JWT-tokens.
 
 ## Installation
@@ -144,7 +139,9 @@
     app.state.auth_manager.login(response, user)
     return response
 ```
 
 
 Auth manager adds authentication middleware to your application instance and uses authentication backends to treat token and
 request user instance. 
+
+
```

### Comparing `fastapi_authtools-0.4/pyproject.toml` & `fastapi_authtools-0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fastapi_authtools"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Michael Nightingale", email="suslanchikmopl@gmail.com" },
 ]
 description = "FastAPI authentication package."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/michael7nightinglae/fastapi_authtools"
-"Bug Tracker" = "https://github.com/michael7nightinglae/fastapi_authtools/issues"
+"Homepage" = "https://github.com/michael7nightingale/fastapi_authtools"
+"Bug Tracker" = "https://github.com/michael7nightingale/fastapi_authtools/issues"
```


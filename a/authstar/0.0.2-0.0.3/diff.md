# Comparing `tmp/authstar-0.0.2.tar.gz` & `tmp/authstar-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authstar-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "authstar-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `authstar-0.0.2.tar` & `authstar-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      778 2023-08-05 15:16:43.000000 authstar-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       34 2023-08-06 03:32:08.997521 authstar-0.0.2/.gitignore
--rw-r--r--   0        0        0      543 2023-08-05 15:16:43.000000 authstar-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-08-05 15:16:43.000000 authstar-0.0.2/LICENSE
--rw-r--r--   0        0        0     7094 2023-08-06 03:00:09.664650 authstar-0.0.2/README.md
--rw-r--r--   0        0        0      582 2023-08-08 15:33:59.162343 authstar-0.0.2/authstar/__init__.py
--rw-r--r--   0        0        0    16397 2023-08-08 15:54:20.627491 authstar-0.0.2/authstar/fastapi.py
--rw-r--r--   0        0        0     5823 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/middleware.py
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/py.typed
--rw-r--r--   0        0        0     3182 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/types.py
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/example/__init__.py
--rw-r--r--   0        0        0     1436 2023-08-08 15:50:56.034881 authstar-0.0.2/example/app.py
--rw-r--r--   0        0        0     2045 2023-08-06 03:36:03.295649 authstar-0.0.2/example/routes.py
--rw-r--r--   0        0        0     2613 2023-08-05 15:16:43.000000 authstar-0.0.2/example/security.py
--rw-r--r--   0        0        0     1023 2023-08-06 03:36:03.285560 authstar-0.0.2/example/settings.py
--rw-r--r--   0        0        0     1597 2023-08-06 03:44:36.493776 authstar-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      225 2023-08-08 15:12:15.511600 authstar-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      149 2023-08-05 15:16:43.000000 authstar-0.0.2/run_checks.sh
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-05 15:16:43.000000 authstar-0.0.2/tests/test_middleware.py
--rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 authstar-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      778 2023-08-05 15:16:43.000000 authstar-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       34 2023-08-06 03:32:08.997521 authstar-0.0.3/.gitignore
+-rw-r--r--   0        0        0      543 2023-08-05 15:16:43.000000 authstar-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-08-05 15:16:43.000000 authstar-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7095 2023-08-08 19:50:11.460253 authstar-0.0.3/README.md
+-rw-r--r--   0        0        0      582 2023-08-08 19:52:50.295162 authstar-0.0.3/authstar/__init__.py
+-rw-r--r--   0        0        0    16570 2023-08-08 19:58:00.282961 authstar-0.0.3/authstar/fastapi.py
+-rw-r--r--   0        0        0     5823 2023-08-05 15:16:43.000000 authstar-0.0.3/authstar/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.3/authstar/py.typed
+-rw-r--r--   0        0        0     3182 2023-08-05 15:16:43.000000 authstar-0.0.3/authstar/types.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.3/example/__init__.py
+-rw-r--r--   0        0        0     1436 2023-08-08 15:50:56.034881 authstar-0.0.3/example/app.py
+-rw-r--r--   0        0        0     2045 2023-08-06 03:36:03.295649 authstar-0.0.3/example/routes.py
+-rw-r--r--   0        0        0     2613 2023-08-05 15:16:43.000000 authstar-0.0.3/example/security.py
+-rw-r--r--   0        0        0     1023 2023-08-06 03:36:03.285560 authstar-0.0.3/example/settings.py
+-rw-r--r--   0        0        0     1597 2023-08-06 03:44:36.493776 authstar-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-08-08 15:12:15.511600 authstar-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      149 2023-08-05 15:16:43.000000 authstar-0.0.3/run_checks.sh
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-05 15:16:43.000000 authstar-0.0.3/tests/test_middleware.py
+-rw-r--r--   0        0        0     7629 1970-01-01 00:00:00.000000 authstar-0.0.3/PKG-INFO
```

### Comparing `authstar-0.0.2/.github/workflows/ci.yml` & `authstar-0.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/.pre-commit-config.yaml` & `authstar-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/LICENSE` & `authstar-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/README.md` & `authstar-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     on_auth_basic=on_auth_basic,
     on_auth_header=HeaderAuth.x_api_key(on_auth_api_key),
     on_auth_scope=on_auth_scope_session,
 )
 ```
 
 The `scope_key` parameter defines the dict key in the ASGI Scope where the
-client information will be stored. The default is `autstar.client`. For
+client information will be stored. The default is `authstar.client`. For
 example, using `scope_key="users"` would match what the **Starlette**
 Authentication Middleware uses and allow for using `request.user` if using
 that framework or a framework built on **Starlette**.
 
 The `AuthstarClient` model can be subclassed to allow for additional
 attributes or methods to be added. If subclassing is not desired, any object
 that implements the `authstar.Client` protocol can be used.
```

### Comparing `authstar-0.0.2/authstar/__init__.py` & `authstar-0.0.3/authstar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Client,
     HeaderAuth,
     Scope,
     ScopeAuthenticator,
     TokenAuthenticator,
 )
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __all__ = [
     "AuthstarClient",
     "AuthstarMiddleware",
     "BasicAuthenticator",
     "Client",
     "HeaderAuth",
```

### Comparing `authstar-0.0.2/authstar/fastapi.py` & `authstar-0.0.3/authstar/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 Authstar FastAPI extension
 
 Provides route security and an OAuth2 token endpoint.
 """
 import collections.abc
 import dataclasses
 import ipaddress
+import logging
 import typing
 
 import fastapi
 import fastapi.openapi.models
 import fastapi.responses
 import fastapi.security
 
 from .middleware import AuthstarMiddleware
 from .types import BasicAuthenticator, Client
 
+logger = logging.getLogger(__name__)
+
 
 class UnauthorizedError(fastapi.HTTPException):
     """HTTP 401 Unauthorized Error."""
 
     def __init__(
         self,
         client: Client,
@@ -416,24 +419,27 @@
                             f"The grant_type '{grant_type}' is not supported, "
                             "only 'client_credentials' is allowed."
                         ),
                     },
                     status_code=400,
                 )
 
-            auth_client: Client | None
+            auth_client = self.client(request)
             if (
-                not (auth_client := self.client(request))
+                not auth_client.is_authenticated
                 and on_auth_basic is not None
                 and client_id is not None
                 and client_secret is not None
             ):
-                auth_client = await on_auth_basic(client_id, client_secret)
+                try:
+                    auth_client = await on_auth_basic(client_id, client_secret)
+                except Exception:
+                    logger.exception("auth from client_id/client_secret failed")
 
-            if not auth_client or not auth_client.is_authenticated:
+            if not auth_client.is_authenticated:
                 return fastapi.responses.JSONResponse(
                     content={"error": "invalid_client"},
                     status_code=401,
                 )
 
             if scope:
                 requested_scopes = set(scope.split())
```

### Comparing `authstar-0.0.2/authstar/middleware.py` & `authstar-0.0.3/authstar/middleware.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/authstar/types.py` & `authstar-0.0.3/authstar/types.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/example/app.py` & `authstar-0.0.3/example/app.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/example/routes.py` & `authstar-0.0.3/example/routes.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/example/security.py` & `authstar-0.0.3/example/security.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/example/settings.py` & `authstar-0.0.3/example/settings.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/pyproject.toml` & `authstar-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/tests/test_middleware.py` & `authstar-0.0.3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.2/PKG-INFO` & `authstar-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authstar
-Version: 0.0.2
+Version: 0.0.3
 Summary: Authstar ASGI Middleware for client authentication
 Keywords: Authentication,ASGI
 Author-email: John Wagenleitner <johnwa@mail.fresnostate.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -62,15 +62,15 @@
     on_auth_basic=on_auth_basic,
     on_auth_header=HeaderAuth.x_api_key(on_auth_api_key),
     on_auth_scope=on_auth_scope_session,
 )
 ```
 
 The `scope_key` parameter defines the dict key in the ASGI Scope where the
-client information will be stored. The default is `autstar.client`. For
+client information will be stored. The default is `authstar.client`. For
 example, using `scope_key="users"` would match what the **Starlette**
 Authentication Middleware uses and allow for using `request.user` if using
 that framework or a framework built on **Starlette**.
 
 The `AuthstarClient` model can be subclassed to allow for additional
 attributes or methods to be added. If subclassing is not desired, any object
 that implements the `authstar.Client` protocol can be used.
```


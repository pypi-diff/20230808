# Comparing `tmp/authstar-0.0.1.tar.gz` & `tmp/authstar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authstar-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "authstar-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `authstar-0.0.1.tar` & `authstar-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      778 2023-08-05 15:16:43.000000 authstar-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       34 2023-08-06 03:32:08.997521 authstar-0.0.1/.gitignore
--rw-r--r--   0        0        0      543 2023-08-05 15:16:43.000000 authstar-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-08-05 15:16:43.000000 authstar-0.0.1/LICENSE
--rw-r--r--   0        0        0     7094 2023-08-06 03:00:09.664650 authstar-0.0.1/README.md
--rw-r--r--   0        0        0      582 2023-08-05 15:16:43.000000 authstar-0.0.1/authstar/__init__.py
--rw-r--r--   0        0        0    15581 2023-08-05 15:16:43.000000 authstar-0.0.1/authstar/fastapi.py
--rw-r--r--   0        0        0     5823 2023-08-05 15:16:43.000000 authstar-0.0.1/authstar/middleware.py
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.1/authstar/py.typed
--rw-r--r--   0        0        0     3182 2023-08-05 15:16:43.000000 authstar-0.0.1/authstar/types.py
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.1/example/__init__.py
--rw-r--r--   0        0        0     1043 2023-08-06 03:10:11.792999 authstar-0.0.1/example/app.py
--rw-r--r--   0        0        0     2045 2023-08-06 03:36:03.295649 authstar-0.0.1/example/routes.py
--rw-r--r--   0        0        0     2613 2023-08-05 15:16:43.000000 authstar-0.0.1/example/security.py
--rw-r--r--   0        0        0     1023 2023-08-06 03:36:03.285560 authstar-0.0.1/example/settings.py
--rw-r--r--   0        0        0     1597 2023-08-06 03:44:36.493776 authstar-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      225 2023-08-06 03:10:11.803437 authstar-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0      149 2023-08-05 15:16:43.000000 authstar-0.0.1/run_checks.sh
--rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-05 15:16:43.000000 authstar-0.0.1/tests/test_middleware.py
--rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 authstar-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      778 2023-08-05 15:16:43.000000 authstar-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       34 2023-08-06 03:32:08.997521 authstar-0.0.2/.gitignore
+-rw-r--r--   0        0        0      543 2023-08-05 15:16:43.000000 authstar-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-08-05 15:16:43.000000 authstar-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7094 2023-08-06 03:00:09.664650 authstar-0.0.2/README.md
+-rw-r--r--   0        0        0      582 2023-08-08 15:33:59.162343 authstar-0.0.2/authstar/__init__.py
+-rw-r--r--   0        0        0    16397 2023-08-08 15:54:20.627491 authstar-0.0.2/authstar/fastapi.py
+-rw-r--r--   0        0        0     5823 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/py.typed
+-rw-r--r--   0        0        0     3182 2023-08-05 15:16:43.000000 authstar-0.0.2/authstar/types.py
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/example/__init__.py
+-rw-r--r--   0        0        0     1436 2023-08-08 15:50:56.034881 authstar-0.0.2/example/app.py
+-rw-r--r--   0        0        0     2045 2023-08-06 03:36:03.295649 authstar-0.0.2/example/routes.py
+-rw-r--r--   0        0        0     2613 2023-08-05 15:16:43.000000 authstar-0.0.2/example/security.py
+-rw-r--r--   0        0        0     1023 2023-08-06 03:36:03.285560 authstar-0.0.2/example/settings.py
+-rw-r--r--   0        0        0     1597 2023-08-06 03:44:36.493776 authstar-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-08-08 15:12:15.511600 authstar-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      149 2023-08-05 15:16:43.000000 authstar-0.0.2/run_checks.sh
+-rw-r--r--   0        0        0        0 2023-08-05 15:16:43.000000 authstar-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-05 15:16:43.000000 authstar-0.0.2/tests/test_middleware.py
+-rw-r--r--   0        0        0     7628 1970-01-01 00:00:00.000000 authstar-0.0.2/PKG-INFO
```

### Comparing `authstar-0.0.1/.github/workflows/ci.yml` & `authstar-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/.pre-commit-config.yaml` & `authstar-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/LICENSE` & `authstar-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/README.md` & `authstar-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/authstar/__init__.py` & `authstar-0.0.2/authstar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Client,
     HeaderAuth,
     Scope,
     ScopeAuthenticator,
     TokenAuthenticator,
 )
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 __all__ = [
     "AuthstarClient",
     "AuthstarMiddleware",
     "BasicAuthenticator",
     "Client",
     "HeaderAuth",
```

### Comparing `authstar-0.0.1/authstar/fastapi.py` & `authstar-0.0.2/authstar/fastapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,40 @@
 import fastapi.responses
 import fastapi.security
 
 from .middleware import AuthstarMiddleware
 from .types import BasicAuthenticator, Client
 
 
+class UnauthorizedError(fastapi.HTTPException):
+    """HTTP 401 Unauthorized Error."""
+
+    def __init__(
+        self,
+        client: Client,
+        detail: typing.Any = None,
+        headers: dict[str, str] | None = None,
+    ) -> None:
+        super().__init__(status_code=401, detail=detail, headers=headers)
+        self.client = client
+
+
+class ForbiddenError(fastapi.HTTPException):
+    """HTTP 403 Forbidden Error."""
+
+    def __init__(
+        self,
+        client: Client,
+        detail: typing.Any = None,
+        headers: dict[str, str] | None = None,
+    ) -> None:
+        super().__init__(status_code=403, detail=detail, headers=headers)
+        self.client = client
+
+
 @dataclasses.dataclass
 class OAuth2TokenRequest:
     """OAuth2 Token Request.
 
     Represents the form values that are sent via POST to an OAuth2 Token
     endpoint.
     """
@@ -127,15 +153,15 @@
     ) -> None:
         """The 'scope_key' should match the one used to configure the
         AuthstarMiddleware. The key is used to retrieve the client information
         from the Scope.
         """
         self.scope_key = scope_key
 
-    def auth_client_from(self, request: fastapi.Request) -> Client:
+    def client(self, request: fastapi.Request) -> Client:
         """Returns the client from the given Request."""
         return typing.cast(Client, request.scope[self.scope_key])
 
     def internal(self, request: fastapi.Request) -> Client:
         """Returns the client if the request was made from an internal network.
 
         This method is designed to be used as a route dependency for any route that
@@ -157,26 +183,27 @@
         >>> @router.get(
         >>>     "/healthcheck",
         >>>     dependencies=[Security(route_security.internal)],
         >>> )
         >>> async def healthcheck() -> dict[str, str]:
         >>>    return {"status": "ok"}
         """
+        auth_client = self.client(request)
         if (client := request.client) and ipaddress.ip_address(client.host).is_private:
-            return self.auth_client_from(request)
-        raise fastapi.HTTPException(status_code=403)
+            return auth_client
+        raise ForbiddenError(client=auth_client)
 
     def authenticated(self, request: fastapi.Request) -> Client:
         """Returns the client if the request came from an authenticated client.
 
         This method is designed to be used as a route dependency for any route that
         should only allow clients that are unathenticated.
 
         If the client is not making the request is not authenticated, an HTTP
-        403 status will be returned.
+        401 Unauthorized will be returned.
 
         For example, a route can be configured as the following example:
 
         >>> from typing import Annotated, Any
 
         >>> from authstar import Client
         >>> from authstar.fastapi import RouteSecurity
@@ -189,32 +216,37 @@
         >>> async def foo() -> dict[str, str]:
         >>>    return {"status": "bar"}
 
         To secure the endpoint and also get access to the client information:
 
         >>> @router.get("/me")
         >>> async def me(
-        >>>     auth_client: Annotated[
+        >>>     client: Annotated[
         >>>         Client, Security(route_security.authenticated)]
         >>> ) -> dict[str, Any]:
         >>>    return auth_client.model_dump()
         """
-        return self.scopes(request, fastapi.security.SecurityScopes(None))
+        auth_client = self.client(request)
+        if auth_client.is_authenticated:
+            return auth_client
+        raise UnauthorizedError(client=auth_client)
 
     def scopes(
         self, request: fastapi.Request, scopes: fastapi.security.SecurityScopes
     ) -> Client:
         """Returns a client if it has at least one of the specified scopes.
 
         This method is designed to be used as a route dependency for any route
         that should only allow clients that have been granted the necessary
         scope(s).
 
-        If the client is not making the request does not possess any of the
-        required scopes, an HTTP 403 status will be returned.
+        If an unauthenticated client is making the request an HTTP 401
+        Unauthorized will be returned. If the client is authenticated but
+        does not possess any of the required scopes, an HTTP 403 status will
+        be returned.
 
         For example, a route can be configured as the following example:
 
         >>> from typing import Annotated, Any
 
         >>> from authstar import Client
         >>> from authstar.fastapi import RouteSecurity
@@ -237,22 +269,21 @@
         >>>     client: Annotated[
         >>>         Client,
         >>>         Security(route_security.scopes, scopes=["api-user"])
         >>>     ]
         >>> ) -> dict[str, Any]:
         >>>    return client.model_dump()
         """
-        auth_client = self.auth_client_from(request)
-        if auth_client.is_authenticated:
-            if not scopes.scopes:
+        auth_client = self.authenticated(request)
+        if not scopes.scopes:
+            return auth_client
+        for scope in scopes.scopes:
+            if scope in auth_client.scopes:
                 return auth_client
-            for scope in scopes.scopes:
-                if scope in auth_client.scopes:
-                    return auth_client
-        raise fastapi.HTTPException(status_code=403)
+        raise ForbiddenError(client=auth_client)
 
     @staticmethod
     def openapi_api_key(
         *,
         name: str = "x-api-key",
         scheme_name: str | None = None,
         description: str | None = None,
@@ -387,15 +418,15 @@
                         ),
                     },
                     status_code=400,
                 )
 
             auth_client: Client | None
             if (
-                not (auth_client := self.auth_client_from(request))
+                not (auth_client := self.client(request))
                 and on_auth_basic is not None
                 and client_id is not None
                 and client_secret is not None
             ):
                 auth_client = await on_auth_basic(client_id, client_secret)
 
             if not auth_client or not auth_client.is_authenticated:
```

### Comparing `authstar-0.0.1/authstar/middleware.py` & `authstar-0.0.2/authstar/middleware.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/authstar/types.py` & `authstar-0.0.2/authstar/types.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/example/routes.py` & `authstar-0.0.2/example/routes.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/example/security.py` & `authstar-0.0.2/example/security.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/example/settings.py` & `authstar-0.0.2/example/settings.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/pyproject.toml` & `authstar-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/tests/test_middleware.py` & `authstar-0.0.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `authstar-0.0.1/PKG-INFO` & `authstar-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authstar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Authstar ASGI Middleware for client authentication
 Keywords: Authentication,ASGI
 Author-email: John Wagenleitner <johnwa@mail.fresnostate.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```


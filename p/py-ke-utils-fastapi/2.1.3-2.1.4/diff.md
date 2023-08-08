# Comparing `tmp/py-ke-utils-fastapi-2.1.3.tar.gz` & `tmp/py-ke-utils-fastapi-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ke-utils-fastapi-2.1.3.tar", last modified: Fri Aug  4 09:56:36 2023, max compression
+gzip compressed data, was "py-ke-utils-fastapi-2.1.4.tar", last modified: Tue Aug  8 13:15:02 2023, max compression
```

## Comparing `py-ke-utils-fastapi-2.1.3.tar` & `py-ke-utils-fastapi-2.1.4.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/PKG-INFO
--rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6383 2023-04-11 16:05:08.000000 py-ke-utils-fastapi-2.1.3/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      415 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       43 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 09:56:36.000000 py-ke-utils-fastapi-2.1.3/py_ke_utils_fastapi.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:13:01.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/__init__.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       76 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3220 2023-08-04 09:56:26.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/_keycloak_auth.py
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       49 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     5056 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/_auth_deco.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 09:56:36.401508 py-ke-utils-fastapi-2.1.3/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      728 2023-08-04 09:56:29.000000 py-ke-utils-fastapi-2.1.3/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6383 2023-04-11 16:05:08.000000 py-ke-utils-fastapi-2.1.4/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-08 13:15:02.000000 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      573 2023-08-08 13:15:02.000000 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-08 13:15:02.000000 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       75 2023-08-08 13:15:02.000000 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-08 13:15:02.000000 py-ke-utils-fastapi-2.1.4/py_ke_utils_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:13:01.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/keycloak/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       76 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/keycloak/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3910 2023-08-08 13:13:23.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/keycloak/_keycloak_auth.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/redis/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       49 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/redis/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     5056 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/redis/_auth_deco.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/sqlalchemy/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       46 2023-08-08 13:13:23.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/sqlalchemy/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     1983 2023-08-08 13:13:23.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/sqlalchemy/_session_handler.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/tenant/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       36 2023-08-08 13:13:23.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/tenant/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      940 2023-08-08 13:13:23.000000 py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/tenant/_utils.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-08 13:15:02.205766 py-ke-utils-fastapi-2.1.4/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      766 2023-08-08 13:14:58.000000 py-ke-utils-fastapi-2.1.4/setup.py
```

### Comparing `py-ke-utils-fastapi-2.1.3/README.md` & `py-ke-utils-fastapi-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/keycloak/_keycloak_auth.py` & `py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/keycloak/_keycloak_auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,49 +3,56 @@
 
 import requests
 from fastapi import Header, Depends, HTTPException
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 from keycloak import KeycloakOpenID, KeycloakError
 from requests import HTTPError
 
+from pykeutilsfastapi.tenant import tenant_extractor
+
 security = HTTPBearer()
 
 
 class KeycloakAuthentication:
     """
     Dependency class for FastAPI. It validates token using keycloak.
     :param server_url: The url of the keycloak.
     :param client_id: The ID of the keycloak client.
     :param client_secret_key: The secret key of the Keycloak client.
+    :param default_tenant: Default tenant.
     """
 
     def __init__(
-        self,
-        server_url: str,
-        client_id: str,
-        client_secret_key: str,
+            self,
+            server_url: str,
+            client_id: str,
+            client_secret_key: str,
+            default_tenant: str = 'public'
     ):
         self.server_url = server_url
         self.client_id = client_id
         self.client_secret_key = client_secret_key
+        self.default_tenant = default_tenant
 
     def __call__(
-        self,
-        x_tenant_id: Annotated[str | None, Header()],
-        credentials: HTTPAuthorizationCredentials = Depends(security),
+            self,
+            x_tenant_id: Annotated[str | None, Header()] = None,
+            origin: Annotated[str | None, Header()] = None,
+            credentials: HTTPAuthorizationCredentials = Depends(security),
     ):
+        tenant_name = tenant_extractor(str(origin), x_tenant_id, self.default_tenant)
         token = credentials.credentials
         if not token:
             logging.error("Bearer Token was not found.")
             raise HTTPException(status_code=401, detail="Unauthorized")
         try:
             oidc = KeycloakOpenID(
                 server_url=self.server_url,
                 client_id=self.client_id,
-                realm_name=x_tenant_id,
+                realm_name=tenant_name,
                 client_secret_key=self.client_secret_key,
             )
             token = token.replace("Bearer ", "")
             oidc.userinfo(token)
             logging.info("Successfully authorized")
         except KeycloakError as e:
             logging.error(f"Error: {e.__doc__} Status code: {e.response_code}")
@@ -53,34 +60,39 @@
 
 
 class KeycloakPermissionCheck:
     """
     Dependency class for FastAPI. It checks the permissions of the user using keycloak.
     :param server_url: The url of the keycloak.
     :param json: The JSON to send to Keycloak
+    :param default_tenant: Default tenant.
     """
 
     def __init__(
-        self,
-        server_url: str,
-        json: dict,
+            self,
+            server_url: str,
+            json: dict,
+            default_tenant: str = 'public'
     ):
         self.server_url = server_url
         self.json = json
+        self.default_tenant = default_tenant
 
     def __call__(
-        self,
-        x_tenant_id: Annotated[str | None, Header()],
-        credentials: HTTPAuthorizationCredentials = Depends(security),
+            self,
+            x_tenant_id: Annotated[str | None, Header()] = None,
+            origin: Annotated[str | None, Header()] = None,
+            credentials: HTTPAuthorizationCredentials = Depends(security),
     ):
         try:
+            tenant_name = tenant_extractor(str(origin), x_tenant_id, self.default_tenant)
             headers = {
                 "Content-Type": "application/json",
                 "Accept": "*/*",
-                "X-Tenant-ID": x_tenant_id,
+                "X-Tenant-ID": tenant_name,
                 "Authorization": f"Bearer {credentials.credentials}",
             }
             response = requests.post(
                 url=self.server_url, json=self.json, headers=headers
             )
             response.raise_for_status()
             logging.info(
```

### Comparing `py-ke-utils-fastapi-2.1.3/pykeutilsfastapi/redis/_auth_deco.py` & `py-ke-utils-fastapi-2.1.4/pykeutilsfastapi/redis/_auth_deco.py`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-2.1.3/setup.py` & `py-ke-utils-fastapi-2.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = "2.1.3"
+VERSION = "2.1.4"
 DESCRIPTION = "Utilities for FastAPI"
 
 # Setting up
 setup(
     name="py-ke-utils-fastapi",
     version=VERSION,
     author="KE",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["redis>=4.5.0", "deepdiff>=6.2.1", "fastapi>=0.90"],
+    install_requires=["redis>=4.5.0", "deepdiff>=6.2.1", "fastapi>=0.90", "SQLAlchemy>=2.0.1", "alembic>=1.10"],
     keywords=["python", "FastAPI", "PyJWT", "decorator", "token"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS",
```


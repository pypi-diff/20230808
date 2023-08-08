# Comparing `tmp/obc-0.1.0.tar.gz` & `tmp/obc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obc-0.1.0.tar", last modified: Fri Feb  3 17:48:20 2023, max compression
+gzip compressed data, was "obc-0.2.0.tar", last modified: Tue Aug  8 07:16:10 2023, max compression
```

## Comparing `obc-0.1.0.tar` & `obc-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-03 17:48:20.319220 obc-0.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-02-03 17:48:18.000000 obc-0.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2743 2023-02-03 17:48:20.319220 obc-0.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2023-02-03 17:48:18.000000 obc-0.1.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2023-02-03 17:48:20.323220 obc-0.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-02-03 17:48:18.000000 obc-0.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-03 17:48:20.319220 obc-0.1.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-03 17:48:20.319220 obc-0.1.0/src/obc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       57 2023-02-03 17:48:18.000000 obc-0.1.0/src/obc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      259 2023-02-03 17:48:18.000000 obc-0.1.0/src/obc/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-03 17:48:20.319220 obc-0.1.0/src/obc/providers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-02-03 17:48:18.000000 obc-0.1.0/src/obc/providers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      810 2023-02-03 17:48:18.000000 obc-0.1.0/src/obc/providers/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15446 2023-02-03 17:48:18.000000 obc-0.1.0/src/obc/providers/obf.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-03 17:48:20.319220 obc-0.1.0/src/obc.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2743 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        4 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-03 17:48:20.000000 obc-0.1.0/src/obc.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 07:16:10.093248 obc-0.2.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-08-08 07:16:09.000000 obc-0.2.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2743 2023-08-08 07:16:10.093248 obc-0.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2022 2023-08-08 07:16:09.000000 obc-0.2.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1613 2023-08-08 07:16:10.093248 obc-0.2.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-08-08 07:16:09.000000 obc-0.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 07:16:10.089248 obc-0.2.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 07:16:10.093248 obc-0.2.0/src/obc/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       57 2023-08-08 07:16:09.000000 obc-0.2.0/src/obc/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      259 2023-08-08 07:16:09.000000 obc-0.2.0/src/obc/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 07:16:10.093248 obc-0.2.0/src/obc/providers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-08 07:16:09.000000 obc-0.2.0/src/obc/providers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      810 2023-08-08 07:16:09.000000 obc-0.2.0/src/obc/providers/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15546 2023-08-08 07:16:09.000000 obc-0.2.0/src/obc/providers/obf.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 07:16:10.093248 obc-0.2.0/src/obc.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2743 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        4 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 07:16:10.000000 obc-0.2.0/src/obc.egg-info/zip-safe
```

### Comparing `obc-0.1.0/LICENSE` & `obc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obc-0.1.0/PKG-INFO` & `obc-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obc
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Open Badges Client
 Home-page: https://github.com/openfun/open-badges-client
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Openbadge,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `obc-0.1.0/README.md` & `obc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `obc-0.1.0/setup.cfg` & `obc-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = obc
-version = 0.1.0
+version = 0.2.0
 description = The Open Badges Client
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://github.com/openfun/open-badges-client
 license = MIT
@@ -17,33 +17,33 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 install_requires = 
-	pydantic[email]>=1.0.0
+	pydantic[email]>=2.0.0
 	requests>=2.0.0
 package_dir = 
 	=src
 packages = find:
 zip_safe = True
 python_requires = >= 3.10
 
 [options.extras_require]
 dev = 
-	bandit==1.7.4
-	black==22.12.0
-	flake8==6.0.0
+	bandit==1.7.5
+	black==23.7.0
+	flake8==6.1.0
 	isort==5.12.0
 	pydocstyle==6.3.0
-	pylint==2.15.10
-	pytest==7.2.1
-	pytest-cov==4.0.0
-	responses==0.22.0
+	pylint==2.17.5
+	pytest==7.4.0
+	pytest-cov==4.1.0
+	responses==0.23.3
 ci = 
 	twine==4.0.2
 
 [options.packages.find]
 where = src
 
 [wheel]
```

### Comparing `obc-0.1.0/src/obc/providers/base.py` & `obc-0.2.0/src/obc/providers/base.py`

 * *Files identical despite different names*

### Comparing `obc-0.1.0/src/obc/providers/obf.py` & `obc-0.2.0/src/obc/providers/obf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 from collections.abc import Iterable
 from functools import cache
 from typing import Literal, Optional
 from urllib.parse import urljoin
 
 # pylint: disable=no-name-in-module
 import requests
-from pydantic import (
-    BaseModel,
-    EmailStr,
-    HttpUrl,
-    NoneStr,
-    ValidationError,
-    root_validator,
-)
+from pydantic import BaseModel, EmailStr, HttpUrl, ValidationError, model_validator
 from requests.exceptions import JSONDecodeError as RequestsJSONDecodeError
 
 from ..exceptions import AuthenticationError, BadgeProviderError
 from .base import BaseProvider
 
 logger = logging.getLogger(__name__)
 
@@ -176,56 +169,56 @@
 
         return response
 
 
 class Badge(BaseModel):
     """Open Badge Factory Badge Model."""
 
-    id: NoneStr = None
+    id: Optional[str] = None
     name: str
     description: str
     draft: bool = False
-    image: NoneStr = None
-    css: NoneStr = None
-    criteria_html: NoneStr = None
-    email_subject: NoneStr = None
-    email_body: NoneStr = None
-    email_link_text: NoneStr = None
-    email_footer: NoneStr = None
+    image: Optional[str] = None
+    css: Optional[str] = None
+    criteria_html: Optional[str] = None
+    email_subject: Optional[str] = None
+    email_body: Optional[str] = None
+    email_link_text: Optional[str] = None
+    email_footer: Optional[str] = None
     expires: Optional[int] = None
     tags: Optional[list[str]] = None
     metadata: Optional[dict] = None
     is_created: bool = False
 
     # pylint: disable=no-self-argument,no-self-use
-    @root_validator
-    def check_id(cls, values):
+    @model_validator(mode="after")
+    def check_id(self) -> "Badge":
         """Created badges (fetched from the API) should have an identifier."""
-        id_ = values.get("id")
-        is_created = values.get("is_created")
+        id_ = self.id
+        is_created = self.is_created
 
         if is_created and id_ is None:
             raise ValidationError("Created badges should have an `id` field.")
 
-        return values
+        return self
 
 
 class BadgeQuery(BaseModel):
     """Open Badge Factory badge query filters."""
 
     draft: Optional[Literal[0, 1]] = None
     category: Optional[list[str]] = None
     id: Optional[list[str]] = None
-    query: NoneStr = None
+    query: Optional[str] = None
     meta: Optional[dict] = None
     external: Optional[Literal[0, 1]] = None
 
     def params(self):
         """Convert model to OBF badge query parameters."""
-        query = self.dict()
+        query = self.model_dump()
         if query.get("category", None) is not None:
             query["category"] = "|".join(query.get("category"))
         if query.get("id", None) is not None:
             query["id"] = "|".join(query.get("id"))
         if query.get("meta", None) is not None:
             for key in query["meta"]:
                 query[f"meta:{key}"] = query["meta"][key]
@@ -233,34 +226,34 @@
 
         return query
 
 
 class IssueBadgeOverride(BaseModel):
     """Open Badge Factory issue badge override model."""
 
-    name: NoneStr = None
-    description: NoneStr = None
+    name: Optional[str] = None
+    description: Optional[str] = None
     tags: Optional[list[str]] = None
-    criteria: NoneStr = None
-    criteria_add: NoneStr = None
+    criteria: Optional[str] = None
+    criteria_add: Optional[str] = None
 
 
 class BadgeIssue(BaseModel):
     """Open Badge Factory badge issue Model."""
 
     recipient: list[EmailStr]
     expires: Optional[int] = None
     issued_on: Optional[int] = None
-    email_subject: NoneStr = None
-    email_body: NoneStr = None
-    email_link_text: NoneStr = None
-    email_footer: NoneStr = None
+    email_subject: Optional[str] = None
+    email_body: Optional[str] = None
+    email_link_text: Optional[str] = None
+    email_footer: Optional[str] = None
     badge_override: Optional[IssueBadgeOverride] = None
     log_entry: Optional[dict] = None
-    api_consumer_id: NoneStr = None
+    api_consumer_id: Optional[str] = None
     send_email: Literal[0, 1] = 1
 
 
 class BadgeRevokation(BaseModel):
     """Open Badge Factory badge revokation model."""
 
     event_id: str
@@ -289,15 +282,15 @@
         self.api_client = OBFAPIClient(
             client_id, client_secret, raise_for_status=raise_for_status
         )
 
     def create(self, badge: Badge) -> Badge:
         """Create a badge."""
         response = self.api_client.post(
-            f"/badge/{self.api_client.client_id}", json=badge.dict()
+            f"/badge/{self.api_client.client_id}", json=badge.model_dump()
         )
         if (
             not response.status_code
             == requests.codes.created  # pylint: disable=no-member
         ):
             raise BadgeProviderError(f"Cannot create badge: {badge}")
 
@@ -308,15 +301,15 @@
         ).groups()[0]
 
         # Get created badge
         fetched = next(self.read(badge=badge))  # type: ignore
         fetched.is_created = True
         logger.info("Successfully created badge '%s' with ID: %s", badge.name, badge.id)
 
-        return Badge(**fetched.dict())
+        return Badge(**fetched.model_dump())
 
     def read(
         self, badge: Badge | None = None, query: BadgeQuery | None = None
     ) -> Iterable[Badge]:
         """Fetch one, selected or all badges.
 
         Args:
@@ -358,15 +351,15 @@
         """Update a badge."""
         if badge.id is None:
             raise BadgeProviderError(
                 "We expect an existing badge instance (the ID field is required)"
             )
 
         response = self.api_client.put(
-            f"/badge/{self.api_client.client_id}/{badge.id}", json=badge.dict()
+            f"/badge/{self.api_client.client_id}/{badge.id}", json=badge.model_dump()
         )
         if (
             not response.status_code
             == requests.codes.no_content  # pylint: disable=no-member
         ):
             raise BadgeProviderError(f"Cannot update badge with ID: {badge.id}")
         logger.info("Successfully updated badge '%s' with ID: %s", badge.name, badge.id)
@@ -423,15 +416,15 @@
             )
         if badge.draft:
             raise BadgeProviderError(
                 f"You cannot issue a badge with a draft status (ID: {badge.id})"
             )
 
         response = self.api_client.post(
-            f"/badge/{self.api_client.client_id}/{badge.id}", json=issue.dict()
+            f"/badge/{self.api_client.client_id}/{badge.id}", json=issue.model_dump()
         )
         if (
             not response.status_code
             == requests.codes.created  # pylint: disable=no-member
         ):
             raise BadgeProviderError(f"Cannot issue badge with ID: {badge.id}")
```

### Comparing `obc-0.1.0/src/obc.egg-info/PKG-INFO` & `obc-0.2.0/src/obc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obc
-Version: 0.1.0
+Version: 0.2.0
 Summary: The Open Badges Client
 Home-page: https://github.com/openfun/open-badges-client
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Openbadge,API
 Classifier: Development Status :: 5 - Production/Stable
```


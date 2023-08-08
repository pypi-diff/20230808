# Comparing `tmp/esmerald_admin-0.2.0.tar.gz` & `tmp/esmerald_admin-0.3.0.tar.gz`

## Comparing `esmerald_admin-0.2.0.tar` & `esmerald_admin-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/__init__.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/application.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/py.typed
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/__init__.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/base.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/email.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/esmerald_admin/backends/username.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/LICENSE
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/README.md
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 esmerald_admin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/__init__.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/application.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/__init__.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/base.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/edgy/__init__.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/edgy/base.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/edgy/email.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/edgy/username.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/saffier/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/saffier/base.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/saffier/email.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/esmerald_admin/backends/saffier/username.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/README.md
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 esmerald_admin-0.3.0/PKG-INFO
```

### Comparing `esmerald_admin-0.2.0/esmerald_admin/application.py` & `esmerald_admin-0.3.0/esmerald_admin/application.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from esmerald import Esmerald, HTTPException, Request, status
 from esmerald.exceptions import ImproperlyConfigured
 from sqladmin import Admin as SQLAdmin  # noqa
 from sqladmin import ModelView as SQLAModelView  # noqa
 from sqladmin._types import ENGINE_TYPE
 from sqladmin.authentication import AuthenticationBackend
 from sqladmin.models import BaseView as SQLAdminBaseView  # noqa
+from sqlalchemy.orm.session import sessionmaker
 from starlette.middleware import Middleware
 
 
 class EsmeraldBase:
-    def is_accessible(self, request: Request) -> bool:  # type: ignore
+    def is_accessible(self, request: Request) -> bool:
         raise ImproperlyConfigured(
             "The `is_accessible` is not used by Esmerald Admin, please use `has_permission` instead."
         )
 
     def has_permission(self, request: Request) -> bool:
         """Override this method to add permission checks.
         Esmerald Admin does not make any assumptions about the authentication system
@@ -40,63 +41,65 @@
     Tha base inherited for Saffier which inherits from the base of sqladmin package.
     """
 
     def __init__(
         self,
         app: Esmerald,
         engine: ENGINE_TYPE,
+        session_maker: Optional[sessionmaker] = None,
         base_url: str = "/admin",
         title: str = "Esmerald Administration",
         logo_url: Optional[str] = None,
         middlewares: Optional[Sequence[Middleware]] = None,
         debug: bool = False,
         templates_dir: str = "templates",
         authentication_backend: Optional[AuthenticationBackend] = None,
     ) -> None:
         super().__init__(
-            app,
-            engine,
-            base_url,
-            title,
-            logo_url,
-            middlewares,
-            debug,
-            templates_dir,
-            authentication_backend,
+            app=app,
+            engine=engine,
+            session_maker=session_maker,
+            base_url=base_url,
+            title=title,
+            logo_url=logo_url,
+            middlewares=middlewares,
+            debug=debug,
+            templates_dir=templates_dir,
+            authentication_backend=authentication_backend,
         )
 
         self.app.router.activate()  # type: ignore
 
     def _find_model_view(self, identity: str) -> ModelView:
         return super()._find_model_view(identity)  # type: ignore
 
     async def _list(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
     async def _create(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.can_create or not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
     async def _details(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.can_view_details or not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
     async def _delete(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.can_delete or not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
     async def _edit(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.can_edit or not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
     async def _export(self, request: Request) -> None:  # type: ignore
-        model_view = self._find_model_view(request.path_params["identity"])  # type: ignore
+        model_view = self._find_model_view(request.path_params["identity"])
         if not model_view.can_export or not model_view.has_permission(request):
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
         if request.path_params["export_type"] not in model_view.export_types:
             raise HTTPException(status_code=404)
```

### Comparing `esmerald_admin-0.2.0/esmerald_admin/backends/base.py` & `esmerald_admin-0.3.0/esmerald_admin/backends/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,63 @@
 from datetime import datetime, timedelta
 from typing import Any, Optional
 
 from esmerald import Request
-from esmerald.exceptions import AuthenticationError, NotAuthorized
+from esmerald.exceptions import AuthenticationError
 from esmerald.security.jwt.token import Token
 from jose import JWSError, JWTError
-from saffier.exceptions import DoesNotFound
 from sqladmin.authentication import AuthenticationBackend
 from starlette.responses import RedirectResponse
 
 DEFAULT_HEADER = "Bearer"
 
 
-class BaseAuthentication(AuthenticationBackend):
+class BackendBaseAuthentication(AuthenticationBackend):
     """
     Uses the AuthenticationProtocol from esmerald_admin assuming it is using the
     Esmerald contrib user and login into the admin.
     """
 
     def __init__(self, secret_key: str, auth_model: Any, config: Any) -> None:
         super().__init__(secret_key)
         self.auth_model = auth_model
         self.config = config
 
-    def generate_user_token(self, user: Any, time=None):
+    def generate_user_token(self, user: Any, time: Any = None) -> str:
         """
         Generates the JWT token for the authenticated user.
         """
         if not time:
             later = datetime.now() + timedelta(minutes=20)
         else:
             later = time
 
         token = Token(sub=user.id, exp=later)
         return token.encode(key=self.config.signing_key, algorithm=self.config.algorithm)
 
-    def is_user_able_to_authenticate(self, user):
+    def is_user_able_to_authenticate(self, user: Any) -> bool:
         """
         Reject users with is_active=False. Custom user models that don't have
         that attribute are allowed.
         """
         return getattr(user, "is_active", True)
 
-    def is_user_staff_and_superuser(self, user):
+    def is_user_staff_and_superuser(self, user: Any) -> bool:
         """Checks if a user is staff and superuser to acess the admin"""
         return bool(user.is_staff and user.is_superuser)
 
     async def clear_session(self, request: Request) -> None:
         """Clears the login sessions form the browser"""
         request.session.clear()
 
     async def logout(self, request: Request) -> bool:  # type: ignore
         """Logout from the admin"""
         await self.clear_session(request)
         return True
 
-    async def retrieve_user(self, token_sub: Any) -> Any:
-        """
-        Retrieves a user from the database using the given token id.
-        """
-        try:
-            sub = int(token_sub)
-            token_sub = sub
-        except (TypeError, ValueError):
-            ...
-
-        user_field = {self.config.user_id_field: token_sub}
-        try:
-            return await self.auth_model.query.get(**user_field)
-        except DoesNotFound:
-            raise NotAuthorized() from None
-        except Exception as e:
-            raise AuthenticationError(detail=str(e)) from e
-
     async def authenticate(self, request: Request) -> Optional[RedirectResponse]:  # type: ignore
         """Authenticates the user and adds to the scope of the application"""
         token = request.session.get("token")
 
         if not token:
             return RedirectResponse(request.url_for("admin:login"), status_code=302)
```

### Comparing `esmerald_admin-0.2.0/esmerald_admin/backends/email.py` & `esmerald_admin-0.3.0/esmerald_admin/backends/saffier/username.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from datetime import datetime
 
 from esmerald import Request
 from saffier.exceptions import DoesNotFound
 
-from esmerald_admin.backends.base import BaseAuthentication
+from esmerald_admin.backends.saffier.base import BaseAuthentication
 
 DEFAULT_HEADER = "Bearer"
 
 
-class EmailAdminAuth(BaseAuthentication):
+class UsernameAdminAuth(BaseAuthentication):
     """
     Uses the AuthenticationProtocol from esmerald_admin assuming it is using the
     Esmerald contrib user and login into the admin.
     """
 
     async def login(self, request: Request) -> bool:  # type: ignore
         form = await request.form()
-        email, password = form["username"], form["password"]
+        username, password = form["username"], form["password"]
 
         try:
-            user = await self.auth_model.query.get(email=email)
+            user = await self.auth_model.query.get(username=username)
         except DoesNotFound:
             return False
 
         is_password_valid = await user.check_password(password)
         if (
             is_password_valid
             and self.is_user_able_to_authenticate(user)
```

### Comparing `esmerald_admin-0.2.0/esmerald_admin/backends/username.py` & `esmerald_admin-0.3.0/esmerald_admin/backends/edgy/username.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
+from edgy.exceptions import ObjectNotFound
 from esmerald import Request
-from saffier.exceptions import DoesNotFound
 
-from esmerald_admin.backends.base import BaseAuthentication
+from esmerald_admin.backends.saffier.base import BaseAuthentication
 
 DEFAULT_HEADER = "Bearer"
 
 
 class UsernameAdminAuth(BaseAuthentication):
     """
     Uses the AuthenticationProtocol from esmerald_admin assuming it is using the
@@ -16,15 +16,15 @@
 
     async def login(self, request: Request) -> bool:  # type: ignore
         form = await request.form()
         username, password = form["username"], form["password"]
 
         try:
             user = await self.auth_model.query.get(username=username)
-        except DoesNotFound:
+        except ObjectNotFound:
             return False
 
         is_password_valid = await user.check_password(password)
         if (
             is_password_valid
             and self.is_user_able_to_authenticate(user)
             and self.is_user_staff_and_superuser(user)
```

### Comparing `esmerald_admin-0.2.0/LICENSE` & `esmerald_admin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.2.0/README.md` & `esmerald_admin-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `esmerald_admin-0.2.0/pyproject.toml` & `esmerald_admin-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = [
-    "esmerald[jwt]>=1.3.0",
-    "saffier>=0.13.0",
-    "sqladmin>=0.12.0,<1.0",
-]
+dependencies = ["esmerald[jwt]>=2.0.4", "sqladmin>=0.14.1,<1.0"]
 keywords = ["esmerald_admin"]
 
 [project.urls]
 Homepage = "https://github.com/tarsil/esmerald-admin"
 Documentation = "https://esmerald-admin.tarsild.io"
 Changelog = "https://esmerald-admin.tarsild.io/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
@@ -61,14 +57,18 @@
     "pytest>=7.2.2,<8.0.0",
     "pytest-cov>=4.0.0,<5.0.0",
     "requests>=2.28.2",
     "ruff>=0.0.256,<1.0.0",
     "saffier[postgres,testing]>=0.12.0",
 ]
 
+saffier = ["saffier>=0.16.0"]
+edgy = ["edgy>=0.1.0"]
+all = ["edgy>=0.1.0", "saffier>=0.16.0"]
+
 dev = [
     "ipdb>=0.13.13,<1.0.0",
     "pre-commit>=3.3.1,<4.0.0",
     "types-python-jose>=3.3.4.7",
 ]
 
 doc = [
@@ -115,17 +115,14 @@
 ]
 
 [[tool.mypy.overrides]]
 module = "esmerald_admin.tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = "docs_src.*"
 ignore_errors = true
 
 [tool.pytest.ini_options]
 addopts = ["--strict-config", "--strict-markers"]
```

### Comparing `esmerald_admin-0.2.0/PKG-INFO` & `esmerald_admin-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald_admin
-Version: 0.2.0
+Version: 0.3.0
 Summary: The needed admin for Saffier ORM with Esmerald
 Project-URL: Homepage, https://github.com/tarsil/esmerald-admin
 Project-URL: Documentation, https://esmerald-admin.tarsild.io
 Project-URL: Changelog, https://esmerald-admin.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/esmerald-admin
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -32,29 +32,35 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: esmerald[jwt]>=1.3.0
-Requires-Dist: saffier>=0.13.0
-Requires-Dist: sqladmin<1.0,>=0.12.0
+Requires-Dist: esmerald[jwt]>=2.0.4
+Requires-Dist: sqladmin<1.0,>=0.14.1
+Provides-Extra: all
+Requires-Dist: edgy>=0.1.0; extra == 'all'
+Requires-Dist: saffier>=0.16.0; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
 Requires-Dist: types-python-jose>=3.3.4.7; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
+Provides-Extra: edgy
+Requires-Dist: edgy>=0.1.0; extra == 'edgy'
+Provides-Extra: saffier
+Requires-Dist: saffier>=0.16.0; extra == 'saffier'
 Provides-Extra: test
 Requires-Dist: anyio<4.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'test'
 Requires-Dist: black<24.0.0,>=23.3.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: mypy<2.0.0,>=1.1.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
```


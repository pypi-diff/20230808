# Comparing `tmp/license_manager_backend-2.3.2.tar.gz` & `tmp/license_manager_backend-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_backend-2.3.2.tar", max compression
+gzip compressed data, was "license_manager_backend-3.0.0.tar", max compression
```

## Comparing `license_manager_backend-2.3.2.tar` & `license_manager_backend-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,38 @@
--rw-r--r--   0        0        0       25 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/README.rst
--rw-r--r--   0        0        0       60 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/__init__.py
--rw-r--r--   0        0        0      453 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/__init__.py
--rw-r--r--   0        0        0     9062 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/booking.py
--rw-r--r--   0        0        0     7864 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/config.py
--rw-r--r--   0        0        0     9015 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/license.py
--rw-r--r--   0        0        0     3665 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api_schemas.py
--rw-r--r--   0        0        0      464 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/compat.py
--rw-r--r--   0        0        0     1147 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/config.py
--rw-r--r--   0        0        0      914 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/constants.py
--rw-r--r--   0        0        0      209 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/exceptions.py
--rw-r--r--   0        0        0     1754 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/helpers.py
--rw-r--r--   0        0        0     2858 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/main.py
--rw-r--r--   0        0        0     1316 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/security.py
--rw-r--r--   0        0        0     1830 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/storage.py
--rw-r--r--   0        0        0     2541 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/table_schemas.py
--rw-r--r--   0        0        0     1099 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/version.py
--rw-r--r--   0        0        0     2011 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 license_manager_backend-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/README.rst
+-rw-r--r--   0        0        0       60 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/__init__.py
+-rw-r--r--   0        0        0      953 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/cruds/__init__.py
+-rw-r--r--   0        0        0     3107 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/cruds/booking.py
+-rw-r--r--   0        0        0     6775 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/cruds/generic.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/__init__.py
+-rw-r--r--   0        0        0     1160 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/booking.py
+-rw-r--r--   0        0        0     1231 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/configuration.py
+-rw-r--r--   0        0        0     2226 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/feature.py
+-rw-r--r--   0        0        0     1036 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/job.py
+-rw-r--r--   0        0        0      887 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/license_server.py
+-rw-r--r--   0        0        0      636 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/models/product.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/__init__.py
+-rw-r--r--   0        0        0     2112 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/bookings.py
+-rw-r--r--   0        0        0     3766 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/configurations.py
+-rw-r--r--   0        0        0     4171 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/features.py
+-rw-r--r--   0        0        0     6922 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/jobs.py
+-rw-r--r--   0        0        0     3234 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/license_servers.py
+-rw-r--r--   0        0        0     2668 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/products.py
+-rw-r--r--   0        0        0     1160 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/routes/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/base.py
+-rw-r--r--   0        0        0      757 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/booking.py
+-rw-r--r--   0        0        0     1150 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/configuration.py
+-rw-r--r--   0        0        0     1265 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/feature.py
+-rw-r--r--   0        0        0     1336 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/job.py
+-rw-r--r--   0        0        0      822 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/license_server.py
+-rw-r--r--   0        0        0      588 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/api/schemas/product.py
+-rw-r--r--   0        0        0     1689 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/config.py
+-rw-r--r--   0        0        0      489 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/constants.py
+-rw-r--r--   0        0        0     7121 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/database.py
+-rw-r--r--   0        0        0     2738 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/main.py
+-rw-r--r--   0        0        0      865 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/permissions.py
+-rw-r--r--   0        0        0     3351 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/security.py
+-rw-r--r--   0        0        0     1099 2023-08-08 21:22:40.980496 license_manager_backend-3.0.0/lm_backend/version.py
+-rw-r--r--   0        0        0     2075 2023-08-08 21:22:40.984496 license_manager_backend-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 license_manager_backend-3.0.0/PKG-INFO
```

### Comparing `license_manager_backend-2.3.2/lm_backend/main.py` & `license_manager_backend-3.0.0/lm_backend/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """ License-manager backend, command line entrypoint
 
 Run with e.g. `uvicorn lm_backend.main:app` OR
 set `licensemanager2.backend.main.handler` as the ASGI handler
 """
 import logging
 import sys
+from contextlib import asynccontextmanager
 from typing import cast
 
 import sentry_sdk
 from fastapi import FastAPI, Response, status
 from fastapi.middleware.cors import CORSMiddleware
 from loguru import logger
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 
-from lm_backend import __version__, storage
-from lm_backend.api import api_v1
+from lm_backend import __version__
+from lm_backend.api import api
 from lm_backend.config import settings
+from lm_backend.database import engine_factory
 
 subapp = FastAPI(
     title="License Manager API",
     version=__version__,
     contact={
         "name": "Omnivector Solutions",
         "url": "https://www.omnivector.solutions/",
@@ -36,15 +38,15 @@
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
-subapp.include_router(api_v1, prefix="/api/v1")
+subapp.include_router(api)
 
 if settings.SENTRY_DSN:
     sentry_sdk.init(
         dsn=settings.SENTRY_DSN,
         sample_rate=cast(float, settings.SENTRY_SAMPLE_RATE),  # The cast silences mypy
         environment=settings.DEPLOY_ENV,
     )
@@ -69,44 +71,32 @@
     return __version__
 
 
 app = FastAPI()
 app.mount("/lm", subapp)
 
 
-@app.on_event("startup")
-def begin_logging():
+@asynccontextmanager
+async def lifespan(_: FastAPI):
     """
-    Configure logging
+    Provide a lifespan context for the app.
+
+    Will set up logging and cleanup database engines when the app is shut down.
+
+    This is the preferred method of handling lifespan events in FastAPI.
+    For more details, see: https://fastapi.tiangolo.com/advanced/events/
     """
     logger.remove()
     logger.add(sys.stderr, level=settings.LOG_LEVEL)
     logger.info(f"Logging configured 📝 Level: {settings.LOG_LEVEL}")
 
     if settings.LOG_LEVEL_SQL:
         level_sql = getattr(logging, settings.LOG_LEVEL_SQL)
 
         engine_logger = logging.getLogger("sqlalchemy.engine")
         engine_logger.setLevel(level_sql)
 
-        databases_logger = logging.getLogger("databases")
-        databases_logger.setLevel(level_sql)
-
         logger.info(f"Database logging configured 📝 Level: {settings.LOG_LEVEL_SQL}")
 
+    yield
 
-@app.on_event("startup")
-async def init_database():
-    """
-    Connect the database; create it if necessary
-    """
-    storage.create_all_tables()
-    await storage.database.connect()
-    logger.info("Database configured 💽")
-
-
-@app.on_event("shutdown")
-async def disconnect_database():
-    """
-    Disconnect the database
-    """
-    await storage.database.disconnect()
+    await engine_factory.cleanup()
```

### Comparing `license_manager_backend-2.3.2/lm_backend/version.py` & `license_manager_backend-3.0.0/lm_backend/version.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.2/pyproject.toml` & `license_manager_backend-3.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-backend"
-version = "2.3.2"
+version = "3.0.0"
 description = "Provides an API for managing license data"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_backend" }]
@@ -16,19 +16,20 @@
 jwt = {version = "^1.2.0", optional = true}
 SQLAlchemy-Utils = "^0.37.8"
 loguru = "^0.5.3"
 asyncpg = "^0.24.0"
 uvicorn = "^0.15.0"
 python-dotenv = "^0.19.0"
 armasec = "^0.11"
-SQLAlchemy = "^1.4.29"
-databases = {extras = ["postgresql"], version = "^0.5.3"}
+SQLAlchemy = {extras = ["asyncio"], version = "^2.0.7"}
 toml = "^0.10.2"
 py-buzz = "^3.2.1"
 psycopg2 = "^2.9.5"
+yarl = "^1.9.2"
+pydantic = {version = "^1", extras = ["email"]}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 pytest-asyncio = "^0.15.1"
 pytest-cov = "^2.12.1"
 pytest-env = "^0.6.2"
 pytest-freezegun = "^0.4.2"
@@ -39,27 +40,23 @@
 pytest-sugar = "^0.9.4"
 aiosqlite = "^0.17.0"
 ipython = "^8.10.0"
 asgi-lifespan = "^1.0.1"
 black = "^22.3"
 alembic = "^1.6.5"
 mypy = "^0.910"
-sqlalchemy-stubs = "^0.4"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--random-order --cov=lm_backend --cov-report=term-missing --cov-fail-under=85"
 testpaths = ["tests"]
 env = [
-    "DATABASE_URL = sqlite:///sqlite-testing.db",
-    "LOG_LEVEL_SQL = ERROR",
-
-    # This setting must align with the rs256_domain fixture from armasec's pytest extension
-    "ARMASEC_DOMAIN = armasec.dev",
-    "ARMASEC_DEBUG = True",
+    "DEPLOY_ENV = TEST",  # Enforces that test database env vars will be used
+    "ARMASEC_DOMAIN = armasec.dev",  # Must align with the rs256_domain fixture in armasec's pytest extension
+    "ARMASEC_DEBUG = False",  # Set this to True to debug armasec issues by seeing verbose logging
 ]
 
 [tool.black]
 line-length = 110
 src = ["lm_backend", "tests"]
 
 [tool.isort]
```

### Comparing `license_manager_backend-2.3.2/PKG-INFO` & `license_manager_backend-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: license-manager-backend
-Version: 2.3.2
+Version: 3.0.0
 Summary: Provides an API for managing license data
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: SQLAlchemy (>=1.4.29,<2.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.37.8,<0.38.0)
+Requires-Dist: SQLAlchemy[asyncio] (>=2.0.7,<3.0.0)
 Requires-Dist: armasec (>=0.11,<0.12)
 Requires-Dist: asyncpg (>=0.24.0,<0.25.0)
-Requires-Dist: databases[postgresql] (>=0.5.3,<0.6.0)
 Requires-Dist: fastapi (>=0.68.0,<0.69.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: py-buzz (>=3.2.1,<4.0.0)
+Requires-Dist: pydantic[email] (>=1,<2)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: sentry-sdk (>=1.3.1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
+Requires-Dist: yarl (>=1.9.2,<2.0.0)
 Project-URL: Documentation, https://omnivector-solutions.github.io/license-manager/
 Project-URL: Repository, https://github.com/omnivector-solutions/license-manager
 Description-Content-Type: text/x-rst
 
 # License-manager Backend
```


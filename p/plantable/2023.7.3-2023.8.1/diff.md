# Comparing `tmp/plantable-2023.7.3.tar.gz` & `tmp/plantable-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantable-2023.7.3.tar", last modified: Sat Jul 29 10:30:54 2023, max compression
+gzip compressed data, was "plantable-2023.8.1.tar", last modified: Tue Aug  8 04:41:38 2023, max compression
```

## Comparing `plantable-2023.7.3.tar` & `plantable-2023.8.1.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      224 2023-07-29 10:30:54.612793 plantable-2023.7.3/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       40 2023-05-28 09:48:20.000000 plantable-2023.7.3/README.md
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 09:49:22.000000 plantable-2023.7.3/pyproject.toml
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      857 2023-07-29 10:30:54.616793 plantable-2023.7.3/setup.cfg
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.608793 plantable-2023.7.3/src/
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.608793 plantable-2023.7.3/src/plantable/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       44 2023-06-29 08:51:03.000000 plantable-2023.7.3/src/plantable/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/agent/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1414 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/app.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      521 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/conf.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/agent/router/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       30 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/router/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1579 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/router/api_token.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2184 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/router/user.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3121 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/agent/util.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/client/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      137 2023-07-29 09:21:07.000000 plantable-2023.7.3/src/plantable/client/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     8043 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/client/account.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    26552 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/client/admin.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    27824 2023-07-29 08:49:04.000000 plantable-2023.7.3/src/plantable/client/base.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4057 2023-07-29 09:35:51.000000 plantable-2023.7.3/src/plantable/client/base_websocket.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      325 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/client/conf.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3296 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/client/core.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2023-06-24 12:53:07.000000 plantable-2023.7.3/src/plantable/client/exception.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)    27754 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/client/user.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/model/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       84 2023-06-12 12:52:09.000000 plantable-2023.7.3/src/plantable/model/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     3059 2023-07-29 01:53:07.000000 plantable-2023.7.3/src/plantable/model/account.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     9847 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/model/core.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1088 2023-06-24 12:53:07.000000 plantable-2023.7.3/src/plantable/model/event.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1748 2023-06-24 12:53:07.000000 plantable-2023.7.3/src/plantable/model/form.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/schema/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-06-04 11:51:49.000000 plantable-2023.7.3/src/plantable/schema/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     2191 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/schema/schema.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      828 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/scripts.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/serde/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       75 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/serde/__init__.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      506 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/serde/const.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4071 2023-07-29 00:39:14.000000 plantable-2023.7.3/src/plantable/serde/from_arrow.py
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     4939 2023-07-29 01:56:05.000000 plantable-2023.7.3/src/plantable/serde/to_python.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.612793 plantable-2023.7.3/src/plantable/static/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:49:22.000000 plantable-2023.7.3/src/plantable/static/__init__.py
-drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-07-29 10:30:54.608793 plantable-2023.7.3/src/plantable.egg-info/
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      224 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1000) eugene    (1000)     1195 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)      249 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1000) eugene    (1000)       10 2023-07-29 10:30:54.000000 plantable-2023.7.3/src/plantable.egg-info/top_level.txt
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      146 2023-08-08 04:41:38.612210 plantable-2023.8.1/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2207 2023-07-30 12:22:48.000000 plantable-2023.8.1/README.md
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      192 2023-05-28 09:49:22.000000 plantable-2023.8.1/pyproject.toml
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      815 2023-08-08 04:41:38.612210 plantable-2023.8.1/setup.cfg
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       56 2023-08-08 04:29:40.000000 plantable-2023.8.1/src/plantable/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable/agent/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       54 2023-07-31 10:30:44.000000 plantable-2023.8.1/src/plantable/agent/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-07-30 11:50:21.000000 plantable-2023.8.1/src/plantable/agent/conf.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable/agent/watcher/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-07-31 10:30:44.000000 plantable-2023.8.1/src/plantable/agent/watcher/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3539 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/agent/watcher/base_watcher.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4244 2023-07-31 10:30:44.000000 plantable-2023.8.1/src/plantable/agent/watcher/view_watcher.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable/client/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      137 2023-07-29 09:21:07.000000 plantable-2023.8.1/src/plantable/client/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     8294 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/account.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    28105 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/admin.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    28172 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/base.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     6318 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/base_websocket.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      325 2023-07-29 00:39:14.000000 plantable-2023.8.1/src/plantable/client/conf.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3353 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/core.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       36 2023-06-24 12:53:07.000000 plantable-2023.8.1/src/plantable/client/exception.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)    28760 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/client/user.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable/model/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       84 2023-06-12 12:52:09.000000 plantable-2023.8.1/src/plantable/model/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3059 2023-07-29 01:53:07.000000 plantable-2023.8.1/src/plantable/model/account.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     9871 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/model/core.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1088 2023-06-24 12:53:07.000000 plantable-2023.8.1/src/plantable/model/event.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1748 2023-06-24 12:53:07.000000 plantable-2023.8.1/src/plantable/model/form.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/src/plantable/schema/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-06-04 11:51:49.000000 plantable-2023.8.1/src/plantable/schema/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2213 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/schema/schema.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      830 2023-07-30 11:44:42.000000 plantable-2023.8.1/src/plantable/scripts.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/src/plantable/serde/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       75 2023-07-29 00:39:14.000000 plantable-2023.8.1/src/plantable/serde/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      506 2023-07-29 00:39:14.000000 plantable-2023.8.1/src/plantable/serde/const.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     4186 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/serde/from_arrow.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     5047 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/serde/to_python.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/src/plantable/server/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-07-30 11:43:58.000000 plantable-2023.8.1/src/plantable/server/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1414 2023-07-29 00:39:14.000000 plantable-2023.8.1/src/plantable/server/app.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      577 2023-07-30 11:46:15.000000 plantable-2023.8.1/src/plantable/server/conf.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/src/plantable/server/router/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       30 2023-07-29 00:39:14.000000 plantable-2023.8.1/src/plantable/server/router/__init__.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1666 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/server/router/api_token.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     2290 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/server/router/user.py
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     3199 2023-08-08 04:28:06.000000 plantable-2023.8.1/src/plantable/server/util.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.612210 plantable-2023.8.1/src/plantable/static/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        0 2023-05-28 09:49:22.000000 plantable-2023.8.1/src/plantable/static/__init__.py
+drwxrwxr-x   0 eugene    (1000) eugene    (1000)        0 2023-08-08 04:41:38.608210 plantable-2023.8.1/src/plantable.egg-info/
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      146 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)     1390 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)        1 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       58 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)      249 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1000) eugene    (1000)       10 2023-08-08 04:41:38.000000 plantable-2023.8.1/src/plantable.egg-info/top_level.txt
```

### Comparing `plantable-2023.7.3/setup.cfg` & `plantable-2023.8.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = plantable
-description = Server for Seatable Webhook
-long_description = file: README.md
+description = 
+long_description = 
 author = Woojin Cho
 author_email = w.cho@cj.net
 keywords = 
 license = MIT License
 
 [options]
 dependency_links =
```

### Comparing `plantable-2023.7.3/src/plantable/agent/app.py` & `plantable-2023.8.1/src/plantable/server/app.py`

 * *Files identical despite different names*

### Comparing `plantable-2023.7.3/src/plantable/agent/conf.py` & `plantable-2023.8.1/src/plantable/server/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
 from dotenv import load_dotenv
 import aioboto3
 from dasida import get_secrets
 
 load_dotenv()
 
-# PROD and DEV
+# consts
 PROD = "prod"
 DEV = "dev"
+SEATABLE_VIEW_SUFFIX_TO_WATCH = "__sync"
 
 # AWS S3
 AWS_S3_BUCKET_NAME = os.getenv("AWS_S3_BUCKET_NAME")
 AWS_S3_BUCKET_PREFIX = os.getenv("AWS_S3_BUCKET_PREFIX")
 
 # From Dasida
 SM_AWS_S3 = os.getenv("SM_AWS_S3")
-aioboto3_conf = get_secrets(
-    SM_AWS_S3,
-    aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
-    aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
-)
-session = aioboto3.Session(**aioboto3_conf)
+if SM_AWS_S3:
+    AIOBOTO3_CONF = get_secrets(
+        SM_AWS_S3,
+        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
+        aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
+    )
+else:
+    AIOBOTO3_CONF = None
```

### Comparing `plantable-2023.7.3/src/plantable/agent/router/api_token.py` & `plantable-2023.8.1/src/plantable/server/router/api_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import aioboto3
 from fastapi import APIRouter, Depends
 from fastapi.security import APIKeyHeader
 
 from ...client import BaseClient
-from ..conf import session
-from ..util import view_to_parquet, upload_to_s3
+from ..util import upload_to_s3, view_to_parquet
+from ..conf import AIOBOTO3_CONF
 
+session = aioboto3.Session(**AIOBOTO3_CONF)
 router = APIRouter(prefix="/api-token", tags=["ApiTokenClient"])
 
 api_key_header = APIKeyHeader(name="Token")
 
 
 ################################################################
 # Basic Auth
@@ -19,30 +21,34 @@
 
 
 ################################################################
 # Endpoints
 ################################################################
 # My API Token
 @router.get("/info")
-async def info_my_seatable_api_token(base_client: BaseClient = Depends(get_base_client)) -> dict:
+async def info_my_seatable_api_token(
+    base_client: BaseClient = Depends(get_base_client),
+) -> dict:
     return base_client.base_token
 
 
 # Export View to S3 Parquet
 @router.get("/export/parquet/view")
 async def export_view_to_s3_with_parquet(
     workspace_name: str,
     base_name: str,
     table_name: str,
     view_name: str,
     group: str = None,
     prod: bool = False,
     base_client: BaseClient = Depends(get_base_client),
 ):
-    content = await view_to_parquet(client=base_client, table_name=table_name, view_name=view_name)
+    content = await view_to_parquet(
+        client=base_client, table_name=table_name, view_name=view_name
+    )
 
     return await upload_to_s3(
         session=session,
         content=content,
         format="parquet",
         prod=prod,
         workspace_name=workspace_name,
```

### Comparing `plantable-2023.7.3/src/plantable/agent/router/user.py` & `plantable-2023.8.1/src/plantable/server/router/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from typing import Annotated
 
+import aioboto3
 from fastapi import APIRouter, Depends, HTTPException, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 
 from ...client import UserClient
-from ..conf import session
-from ..util import view_to_parquet, upload_to_s3
+from ..conf import AIOBOTO3_CONF
+from ..util import upload_to_s3, view_to_parquet
 
+session = aioboto3.Session(**AIOBOTO3_CONF)
 router = APIRouter(prefix="/user", tags=["UserClient"])
 security = HTTPBasic()
 
 
 ################################################################
 # Basic Auth
 ################################################################
-async def get_user_client(credentials: Annotated[HTTPBasicCredentials, Depends(security)]):
-    uc = UserClient(seatable_username=credentials.username, seatable_password=credentials.password)
+async def get_user_client(
+    credentials: Annotated[HTTPBasicCredentials, Depends(security)]
+):
+    uc = UserClient(
+        seatable_username=credentials.username, seatable_password=credentials.password
+    )
     try:
         _ = await uc.login()
     except Exception as ex:
         if ex.status == 400:
             raise HTTPException(
                 status_code=status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect username or password",
@@ -30,15 +36,17 @@
 
 
 ################################################################
 # Endpoints
 ################################################################
 # My SeaTable Account Info
 @router.get("/info")
-async def info_my_seatable_account(user_client: Annotated[dict, Depends(get_user_client)]):
+async def info_my_seatable_account(
+    user_client: Annotated[dict, Depends(get_user_client)]
+):
     return await user_client.get_account_info()
 
 
 # Export View to S3 Parquet
 @router.get("/export/parquet/view")
 async def export_view_to_s3_with_parquet(
     user_client: Annotated[dict, Depends(get_user_client)],
@@ -48,15 +56,17 @@
     view_name: str,
     group: str = None,
     prod: bool = False,
 ):
     base_client = await user_client.get_base_client_with_account_token(
         workspace_name_or_id=workspace_name, base_name=base_name
     )
-    content = await view_to_parquet(client=base_client, table_name=table_name, view_name=view_name)
+    content = await view_to_parquet(
+        client=base_client, table_name=table_name, view_name=view_name
+    )
 
     return await upload_to_s3(
         session=session,
         content=content,
         format="parquet",
         prod=prod,
         workspace_name=workspace_name,
```

### Comparing `plantable-2023.7.3/src/plantable/agent/util.py` & `plantable-2023.8.1/src/plantable/server/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 
 from ..client.base import BaseClient
 from .conf import AWS_S3_BUCKET_NAME, AWS_S3_BUCKET_PREFIX, DEV, PROD
 
 
 # Generate Filename
 def generate_filename(
-    workspace_name: str, base_name: str, table_name: str, view_name: str = None, format: str = "parquet"
+    workspace_name: str,
+    base_name: str,
+    table_name: str,
+    view_name: str = None,
+    format: str = "parquet",
 ):
     names = [workspace_name, base_name, table_name]
     if view_name:
         names.append(view_name)
     return ".".join(["_".join(names), format])
 
 
@@ -26,15 +30,22 @@
     workspace_name: str,
     base_name: str,
     table_name: str,
     view_name: str,
     group: str = None,
     aws_s3_bucket_prefix: str = AWS_S3_BUCKET_PREFIX,
 ) -> str:
-    keys = [aws_s3_bucket_prefix, format, PROD if prod else DEV, workspace_name, base_name, table_name]
+    keys = [
+        aws_s3_bucket_prefix,
+        format,
+        PROD if prod else DEV,
+        workspace_name,
+        base_name,
+        table_name,
+    ]
 
     # append prefix
     if group:
         keys.append(f"group={group}")
     keys.append(f"view={view_name}")
 
     # append filename
@@ -54,15 +65,17 @@
         pq.write_table(table=tbl, where=buffer, version=version)
         buffer.seek(0)
         content = buffer.read()
     return content
 
 
 # Read Table using BaseClient as Parquet
-async def table_to_parquet(client: BaseClient, table_name: str, modified_before: str, modified_after: str):
+async def table_to_parquet(
+    client: BaseClient, table_name: str, modified_before: str, modified_after: str
+):
     records = await client.read_table(
         table_name=table_name,
         modified_before=modified_before,
         modified_after=modified_after,
     )
     return pylist_to_parquet(records)
```

### Comparing `plantable-2023.7.3/src/plantable/client/account.py` & `plantable-2023.8.1/src/plantable/client/account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 import asyncio
 import logging
 from datetime import datetime
 from typing import List, Union
 
 import aiohttp
 import orjson
+import requests
 from pydantic import BaseModel
 from tabulate import tabulate
 
-from .conf import (
-    SEATABLE_ACCOUNT_TOKEN,
-    SEATABLE_PASSWORD,
-    SEATABLE_URL,
-    SEATABLE_USERNAME,
-)
 from ..model import (
     DTABLE_ICON_COLORS,
     DTABLE_ICON_LIST,
     Admin,
     ApiToken,
     Base,
     BaseToken,
     Column,
     Table,
     Team,
     User,
     Webhook,
 )
-from .base import BaseClient
+from .conf import (
+    SEATABLE_ACCOUNT_TOKEN,
+    SEATABLE_PASSWORD,
+    SEATABLE_URL,
+    SEATABLE_USERNAME,
+)
 from .core import TABULATE_CONF, HttpClient
 
 logger = logging.getLogger()
 
 
 ################################################################
 # AccountClient
 ################################################################
 class AccountClient(HttpClient):
     def __init__(
         self,
         seatable_url: str = SEATABLE_URL,
         seatable_username: str = SEATABLE_USERNAME,
         seatable_password: str = SEATABLE_PASSWORD,
-        account_token: str = SEATABLE_ACCOUNT_TOKEN,
-        api_token: str = None,
     ):
         super().__init__(seatable_url=seatable_url)
         self.username = seatable_username
         self.password = seatable_password
-        self.account_token = account_token
-        self.api_token = api_token
-        self.base_tokens = dict()
+        self.account_token = None
 
-    async def login(self):
-        async with self.session_maker() as session:
-            response = await self.request(
-                session=session,
-                method="POST",
-                url="/api2/auth-token/",
-                json={"username": self.username, "password": self.password},
-            )
-        self.account_token = response["token"]
+        # do login
+        self.login()
+
+    def login(self):
+        auth_url = self.seatable_url + "/api2/auth-token/"
+        response = requests.post(
+            auth_url, json={"username": self.username, "password": self.password}
+        )
+        response.raise_for_status()
+        results = response.json()
+        self.account_token = results["token"]
 
     ################################################################
     # AUTHENTICATION - API TOKEN
     ################################################################
     # [API TOKEN] list api tokens
-    async def list_api_tokens(self, workspace_id: str, base_name: str, model: BaseModel = ApiToken):
+    async def list_api_tokens(
+        self, workspace_id: str, base_name: str, model: BaseModel = ApiToken
+    ):
         """
         [NOTE]
          workspace id : group = 1 : 1
         """
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace_id}/dtable/{base_name}/api-tokens/"
         ITEM = "api_tokens"
@@ -82,37 +82,48 @@
         if model:
             results = [model(**x) for x in results]
 
         return results
 
     # [API TOKEN] create api token
     async def get_or_create_api_token(
-        self, workspace_id: str, base_name: str, app_name: str, permission: str = "rw", model: BaseModel = ApiToken
+        self,
+        workspace_id: str,
+        base_name: str,
+        app_name: str,
+        permission: str = "rw",
+        model: BaseModel = ApiToken,
     ):
         """
         [NOTE]
          "bad request" returns if app_name is already exists.
         """
-        api_tokens = await self.list_api_tokens(workspace_id=workspace_id, base_name=base_name)
+        api_tokens = await self.list_api_tokens(
+            workspace_id=workspace_id, base_name=base_name
+        )
         for api_token in api_tokens:
             if api_token.app_name == app_name:
                 return api_token
 
         METHOD = "POST"
         URL = f"/api/v2.1/workspace/{workspace_id}/dtable/{base_name}/api-tokens/"
         JSON = {"app_name": app_name, "permission": permission}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = model(**response) if model else response
 
         return results
 
     # [API TOKEN] create temporary api token
-    async def create_temp_api_token(self, workspace_id: str, base_name: str, model: BaseModel = ApiToken):
+    async def create_temp_api_token(
+        self, workspace_id: str, base_name: str, model: BaseModel = ApiToken
+    ):
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace_id}/dtable/{base_name}/temp-api-token/"
         ITEM = "api_token"
 
         async with self.session_maker(token=self.account_token) as session:
             response = await self.request(session=session, method=METHOD, url=URL)
             results = response[ITEM]
@@ -128,22 +139,29 @@
                 permission="r",
             )
 
         return results
 
     # [API TOKEN] update api token
     async def update_api_token(
-        self, workspace_id: str, base_name: str, app_name: str, permission: str = "rw", model: BaseModel = ApiToken
+        self,
+        workspace_id: str,
+        base_name: str,
+        app_name: str,
+        permission: str = "rw",
+        model: BaseModel = ApiToken,
     ):
         METHOD = "PUT"
         URL = f"/api/v2.1/workspace/{workspace_id}/dtable/{base_name}/api-tokens/{app_name}"
         JSON = {"permission": permission}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = model(**response) if model else response
 
         return results
 
     # [API TOKEN] delete api token
     async def delete_api_token(self, workspace_id: str, base_name: str, app_name: str):
         METHOD = "DELETE"
@@ -157,53 +175,62 @@
         return results
 
     ################################################################
     # AUTHENTICATION - BASE TOKEN
     ################################################################
     # [BASE TOKEN] get base token with account token
     async def get_base_token_with_account_token(
-        self, workspace_id: str = None, base_name: str = None, model: BaseModel = BaseToken
+        self,
+        workspace_id: str = None,
+        base_name: str = None,
+        model: BaseModel = BaseToken,
     ):
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace_id}/dtable/{base_name}/access-token/"
 
         async with self.session_maker(token=self.account_token) as session:
             results = await self.request(session=session, method=METHOD, url=URL)
         if model:
             results = model(**results)
 
         return results
 
     # [BASE TOKEN] get base token with api token
-    async def get_base_token_with_api_token(self, api_token: str, model: BaseModel = BaseToken):
+    async def get_base_token_with_api_token(
+        self, api_token: str, model: BaseModel = BaseToken
+    ):
         METHOD = "GET"
         URL = "/api/v2.1/dtable/app-access-token/"
 
         async with self.session_maker(token=api_token) as session:
             results = await self.request(session=session, method=METHOD, url=URL)
         if model:
             results = model(**results)
 
         return results
 
     # [BASE TOKEN] get base token with invite link
-    async def get_base_token_with_invite_link(self, link: str, model: BaseModel = BaseToken):
+    async def get_base_token_with_invite_link(
+        self, link: str, model: BaseModel = BaseToken
+    ):
         link = link.rsplit("/links/", 1)[-1].strip("/")
         METHOD = "GET"
         URL = "/api/v2.1/dtable/share-link-access-token/"
 
         async with self.session_maker(token=link) as session:
             results = await self.request(session=session, method=METHOD, url=URL)
         if model:
             results = model(**results)
 
         return results
 
     # [BASE TOKEN] get base token with external link
-    async def get_base_token_with_external_link(self, link: str, model: BaseModel = BaseToken):
+    async def get_base_token_with_external_link(
+        self, link: str, model: BaseModel = BaseToken
+    ):
         link = link.rsplit("/external-links/", 1)[-1].strip("/")
         METHOD = "GET"
         URL = f"/api/v2.1/external-link-tokens/{link}/access-token/"
 
         async with self.session_maker(token=link) as session:
             results = await self.request(session=session, method=METHOD, url=URL)
         if model:
@@ -211,12 +238,19 @@
 
         return results
 
     ################################################################
     # (CUSTOM) GET BASE CLIENT
     ################################################################
     # [BASE CLIENT] (custom) get base client with account token
-    async def get_base_client_with_account_token(self, workspace_id: str, base_name: str):
-        base_token = await self.get_base_token_with_account_token(workspace_id=workspace_id, base_name=base_name)
+    async def get_base_client_with_account_token(
+        self, workspace_id: str, base_name: str
+    ):
+        # 특정 환경에서 Circular Import 문제 발생하여 이곳에서 BaseClient Load
+        from .base import BaseClient
+
+        base_token = await self.get_base_token_with_account_token(
+            workspace_id=workspace_id, base_name=base_name
+        )
         client = BaseClient(base_token=base_token)
 
         return client
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plantable-2023.7.3/src/plantable/client/admin.py` & `plantable-2023.8.1/src/plantable/client/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -424,15 +424,18 @@
         if model:
             results = [model(**x) for x in results]
 
         return results
 
     # Reorder Your Groups
     async def reorder_group(
-        self, name_or_id: Union[str, int], anchor_group_name_or_id: Union[str, int] = None, to_last: bool = False
+        self,
+        name_or_id: Union[str, int],
+        anchor_group_name_or_id: Union[str, int] = None,
+        to_last: bool = False,
     ):
         if isinstance(name_or_id, str):
             group = await self.get_group(name_or_id=name_or_id)
             name_or_id = group.id
         if isinstance(anchor_group_name_or_id, str):
             anchor_group = await self.get_group(name_or_id=anchor_group_name_or_id)
             anchor_group_name_or_id = anchor_group.id
@@ -466,15 +469,20 @@
 
         if model:
             results = [model(**x) for x in results]
 
         return results
 
     # Add Group Members
-    async def add_group_members(self, name_or_id: Union[str, int], user_emails: List[str], model: BaseModel = None):
+    async def add_group_members(
+        self,
+        name_or_id: Union[str, int],
+        user_emails: List[str],
+        model: BaseModel = None,
+    ):
         if isinstance(name_or_id, str):
             group = await self.get_group(name_or_id=name_or_id)
             name_or_id = group.id
         user_emails = user_emails if isinstance(user_emails, list) else [user_emails]
         user_emails = await asyncio.gather(*[self.encode_user(contact_email=user_email) for user_email in user_emails])
 
         METHOD = "POST"
@@ -677,26 +685,64 @@
 
         async with self.session_maker(token=self.account_token) as session:
             response = await self.request(session=session, method=METHOD, url=URL)
 
         return response
 
     ################################################################
-    # CUSTOM
+    # OVERRIDE ACCOUNT CLIENT
     ################################################################
     async def infer_workspace_id(self, group_name_or_id: Union[str, int]):
         bases = await self.list_group_bases(group_name_or_id)
         workspace_id = None
         for base in bases:
             if workspace_id is None:
                 workspace_id = base.workspace_id
             if workspace_id != base.workspace_id:
                 raise KeyError("workspace id is not unique!")
         return workspace_id
 
+    async def get_or_create_api_token(
+        self,
+        group_name_or_id: str,
+        base_name: str,
+        app_name: str,
+        permission: str = "rw",
+    ):
+        workspace_id = await self.infer_workspace_id(group_name_or_id=group_name_or_id)
+        return await super().get_or_create_api_token(
+            workspace_id=workspace_id,
+            base_name=base_name,
+            app_name=app_name,
+            permission=permission,
+        )
+
+    async def update_api_token(
+        self,
+        group_name_or_id: str,
+        base_name: str,
+        app_name: str,
+        permission: str = "rw",
+    ):
+        workspace_id = await self.infer_workspace_id(group_name_or_id=group_name_or_id)
+        return await super().update_api_token(
+            workspace_id=workspace_id,
+            base_name=base_name,
+            app_name=app_name,
+            permission=permission,
+        )
+
+    async def delete_api_token(self, group_name_or_id: str, base_name: str, app_name: str):
+        workspace_id = await self.infer_workspace_id(group_name_or_id=group_name_or_id)
+        return await super().delete_api_token(workspace_id=workspace_id, base_name=base_name, app_name=app_name)
+
+    async def create_temp_api_token(self, group_name_or_id: str, base_name: str):
+        workspace_id = await self.infer_workspace_id(group_name_or_id=group_name_or_id)
+        return await super().create_temp_api_token(workspace_id=workspace_id, base_name=base_name)
+
     async def get_base_client_with_account_token(self, group_name_or_id: Union[str, int], base_name: str):
         members = await self.list_group_members(name_or_id=group_name_or_id)
         for member in members:
             if member.contact_email == self.username:
                 break
         else:
             me = await self.encode_user(contact_email=self.username)
```

### Comparing `plantable-2023.7.3/src/plantable/client/base.py` & `plantable-2023.8.1/src/plantable/client/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,36 +159,36 @@
             results = [model(**x) for x in results]
 
         return results
 
     # (CUSTOM) ls
     async def ls(self, table_name: str = None):
         metadata = await self.get_metadata()
-        tables = metadata["tables"]
+        tables = metadata.tables
         if table_name:
             for table in tables:
-                if table["name"] == table_name:
+                if table.name == table_name:
                     break
             else:
                 raise KeyError()
-            columns = [{"key": c["key"], "name": c["name"], "type": c["type"]} for c in table["columns"]]
+            columns = [{"key": c.key, "name": c.name, "type": c.type} for c in table.columns]
             print(tabulate(columns, **TABULATE_CONF))
             return
         _tables = list()
         for table in tables:
-            _n = len(table["columns"])
-            _columns = ", ".join(c["name"] for c in table["columns"])
+            _n = len(table.columns)
+            _columns = ", ".join(c.name for c in table.columns)
             if len(_columns) > 50:
                 _columns = _columns[:50] + "..."
             _columns += f" ({_n})"
             _tables += [
                 {
-                    "id": table["_id"],
-                    "name": table["name"],
-                    "views": ", ".join([v["name"] for v in table["views"]]),
+                    "id": table.id,
+                    "name": table.name,
+                    "views": ", ".join([v.name for v in table.views]),
                     "columns": _columns,
                 },
             ]
         print(tabulate(_tables, **TABULATE_CONF))
 
     ################################################################
     # ROWS
@@ -198,15 +198,18 @@
         """
         [NOTE]
          default LIMIT 100 when not LIMIT is given!
          max LIMIT 10000
         """
         METHOD = "POST"
         URL = f"/dtable-db/api/v1/query/{self.base_token.dtable_uuid}/"
-        JSON = {"sql": sql.get_sql() if isinstance(sql, QueryBuilder) else sql, "convert_keys": convert_keys}
+        JSON = {
+            "sql": sql.get_sql() if isinstance(sql, QueryBuilder) else sql,
+            "convert_keys": convert_keys,
+        }
         SUCCESS = "success"
         ITEM = "results"
 
         async with self.session_maker(token=self.base_token.access_token) as session:
             response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
             if not response[SUCCESS]:
                 raise Exception(response)
@@ -279,22 +282,31 @@
             direction=direction,
             start=start,
             limit=limit,
         )
 
     # Add Row
     async def add_row(
-        self, table_name: str, row: dict, anchor_row_id: str = None, row_insert_position: str = "insert_below"
+        self,
+        table_name: str,
+        row: dict,
+        anchor_row_id: str = None,
+        row_insert_position: str = "insert_below",
     ):
         # insert_below or insert_above
         METHOD = "POST"
         URL = f"/dtable-server/api/v1/dtables/{self.base_token.dtable_uuid}/rows/"
         JSON = {"table_name": table_name, "row": row}
         if anchor_row_id:
-            JSON.update({"ahchor_row_id": anchor_row_id, "row_insert_position": row_insert_position})
+            JSON.update(
+                {
+                    "ahchor_row_id": anchor_row_id,
+                    "row_insert_position": row_insert_position,
+                }
+            )
 
         async with self.session_maker(token=self.base_token.access_token) as session:
             results = await self.request(session=session, method=METHOD, url=URL, json=JSON)
 
         return results
 
     # Update Row
@@ -593,29 +605,40 @@
         if model:
             results = [model(**x) for x in results]
 
         return results
 
     # Create View
     async def create_view(
-        self, table_name: str, name: str, type: str = "table", is_locked: bool = False, model: BaseModel = View
+        self,
+        table_name: str,
+        name: str,
+        type: str = "table",
+        is_locked: bool = False,
+        model: BaseModel = View,
     ):
         """
         type: "table" or "archive" (bigdata)
         """
         METHOD = "POST"
         URL = f"/dtable-server/api/v1/dtables/{self.base_token.dtable_uuid}/views/"
         JSON = {
             "name": name,
             "type": type,
             "is_locked": str(is_locked).lower(),
         }
 
         async with self.session_maker(token=self.base_token.access_token) as session:
-            results = await self.request(session=session, method=METHOD, url=URL, json=JSON, table_name=table_name)
+            results = await self.request(
+                session=session,
+                method=METHOD,
+                url=URL,
+                json=JSON,
+                table_name=table_name,
+            )
 
         if model:
             results = model(**results)
 
         return results
 
     # Get View
@@ -643,15 +666,21 @@
         METHOD = "PUT"
         URL = f"/dtable-server/api/v1/dtables/{self.base_token.dtable_uuid}/views/{view_name}/"
 
         if isinstance(conf, BaseModel):
             conf = conf.dict()
 
         async with self.session_maker(token=self.base_token.access_token) as session:
-            results = await self.request(session=session, method=METHOD, url=URL, json=conf, table_name=table_name)
+            results = await self.request(
+                session=session,
+                method=METHOD,
+                url=URL,
+                json=conf,
+                table_name=table_name,
+            )
 
         return results
 
     # Delete View
     async def delete_view(self, table_name: str, view_name: str):
         METHOD = "DELETE"
         URL = f"/dtable-server/api/v1/dtables/{self.base_token.dtable_uuid}/views/{view_name}/"
```

### Comparing `plantable-2023.7.3/src/plantable/client/core.py` & `plantable-2023.8.1/src/plantable/client/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 from typing import List, Union
 
 import aiohttp
 import orjson
 from pydantic import BaseModel
 from tabulate import tabulate
 
-from ..model import Admin, ApiToken, Base, BaseToken, Column, File, Table, Team, User, Webhook
+from ..model import (
+    Admin,
+    ApiToken,
+    Base,
+    BaseToken,
+    Column,
+    File,
+    Table,
+    Team,
+    User,
+    Webhook,
+)
 from .conf import SEATABLE_URL
 
 logger = logging.getLogger()
 
 TABULATE_CONF = {"tablefmt": "psql", "headers": "keys"}
 
 
@@ -21,15 +32,15 @@
 
 
 ################################################################
 # HttpClient
 ################################################################
 class HttpClient:
     def __init__(self, seatable_url: str = SEATABLE_URL):
-        self.seatable_url = seatable_url
+        self.seatable_url = seatable_url.rstrip("/")
 
         self.headers = {"accept": "application/json"}
         self.debug = False
         self._request = None
 
     async def info(self):
         async with self.session_maker() as session:
```

### Comparing `plantable-2023.7.3/src/plantable/client/user.py` & `plantable-2023.8.1/src/plantable/client/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,17 @@
     ################################################################
     # Helper
     ################################################################
     async def get_base_client_with_account_token(
         self, workspace_name_or_id: Union[str, int] = None, base_name: str = None
     ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
-        return await super().get_base_client_with_account_token(workspace_id=workspace.id, base_name=base_name)
+        return await super().get_base_client_with_account_token(
+            workspace_id=workspace.id, base_name=base_name
+        )
 
     ################################################################
     # USER
     ################################################################
     # [USER] get account info
     async def get_account_info(self, model: BaseModel = AccountInfo):
         METHOD = "GET"
@@ -81,22 +83,26 @@
 
         if model:
             results = model(**results)
 
         return results
 
     # [USER] list public user info
-    async def list_public_user_info(self, user_id_list: List[str], model: BaseModel = UserInfo):
+    async def list_public_user_info(
+        self, user_id_list: List[str], model: BaseModel = UserInfo
+    ):
         METHOD = "POST"
         URL = "/api/v2.1/user-list/"
         JSON = {"user_id_list": user_id_list}
         ITEM = "user_list"
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = response[ITEM]
 
         if model:
             results = [model(**x) for x in results]
 
         return results
 
@@ -134,15 +140,17 @@
         URL = f"/api/v2.1/dtables/"
         ITEM = "table"
         DATA = aiohttp.FormData([("workspace_id", workspace.id), ("name", base_name)])
         _ = DATA.add_field("icon", icon) if icon else None
         _ = DATA.add_field("color", color) if color else None
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, data=DATA)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, data=DATA
+            )
             results = response[ITEM]
 
         if model:
             results = model(**results)
 
         return results
 
@@ -163,15 +171,17 @@
         ITEM = "table"
         DATA = aiohttp.FormData([("name", base_name)])
         _ = DATA.add_field("new_name", new_base_name) if new_base_name else None
         _ = DATA.add_field("icon", new_icon) if new_icon else None
         _ = DATA.add_field("color", new_color) if new_color else None
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, data=DATA)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, data=DATA
+            )
             results = response[ITEM]
 
         if model:
             results = model(**results)
 
         return results
 
@@ -224,28 +234,32 @@
     async def favorite_base(self, base: Base):
         METHOD = "POST"
         URL = "/api/v2.1/starred-dtables/"
         ITEM = "success"
         JSON = {"dtable_uuid": base.uuid}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = response[ITEM]
 
         return results
 
     # [BASES] unfavorite base
     async def unfavorite_base(self, base: Base):
         METHOD = "DELETE"
         URL = "/api/v2.1/starred-dtables/"
         ITEM = "success"
         PARAMS = {"dtable_uuid": base.uuid}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, **PARAMS)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, **PARAMS
+            )
             results = response[ITEM]
 
         return results
 
     # [BASES] (custom) get base by name
     async def get_base(self, workspace_name: str, base_name: str):
         results = await self.list_bases()
@@ -266,25 +280,29 @@
         else:
             raise KeyError()
 
     ################################################################
     # GROUPS & WORKSPACES
     ################################################################
     # [GROUPS & WORKSPACES] list workspaces
-    async def list_workspaces(self, detail: bool = True, incl: List[str] = None, model: BaseModel = Workspace) -> dict:
+    async def list_workspaces(
+        self, detail: bool = True, incl: List[str] = None, model: BaseModel = Workspace
+    ) -> dict:
         """
         incl: "personal" or "group"
         """
         METHOD = "GET"
         URL = "/api/v2.1/workspaces/"
         ITEM = "workspace_list"
         PARAMS = {"detail": str(detail).lower()}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, **PARAMS)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, **PARAMS
+            )
             results = response[ITEM]
 
         if incl:
             incl = incl if isinstance(incl, list) else [incl]
             results = [x for x in results if x["type"] in incl]
 
         if model:
@@ -292,15 +310,17 @@
             # shared는 데이터 형식이 다르기 때문에 별도 method 사용, 여기서는 ignore
             results = [x for x in results if x["type"] != "shared"]
             results = [model(**x) for x in results]
 
         return results
 
     # [GROUPS & WORKSPACES] get workspace
-    async def get_workspace(self, name_or_id: Union[str, int], workspace_type: str = "group"):
+    async def get_workspace(
+        self, name_or_id: Union[str, int], workspace_type: str = "group"
+    ):
         """
         workspace_type: "group", "personal", "starred", or "shared"
         """
         workspaces = await self.list_workspaces(detail=True, model=Workspace)
         for workspace in workspaces:
             if workspace_type and workspace.type != workspace_type:
                 continue
@@ -311,28 +331,39 @@
         else:
             raise KeyError()
 
     ################################################################
     # (CUSTOM) LS & GET
     ################################################################
     # (custom) get
-    async def get(self, workspace_name_or_id: str, base_name: str = None, table_name: str = None):
-        workspace_name_or_id, base_name, table_name = parse_name(workspace_name_or_id, base_name, table_name)
+    async def get(
+        self, workspace_name_or_id: str, base_name: str = None, table_name: str = None
+    ):
+        workspace_name_or_id, base_name, table_name = parse_name(
+            workspace_name_or_id, base_name, table_name
+        )
 
         if table_name:
             bc = await self.get_base_client_with_account_token(
                 workspace_name_or_id=workspace_name_or_id, base_name=base_name
             )
             return await bc.get_table(table_name=table_name)
         if base_name:
-            return await self.get_base(workspace_name_or_id=workspace_name_or_id, base_name=base_name)
+            return await self.get_base(
+                workspace_name_or_id=workspace_name_or_id, base_name=base_name
+            )
         return await self.get_workspace(name_or_id=workspace_name_or_id)
 
     # (custom) ls
-    async def ls(self, workspace_name_or_id: str = None, base_name: str = None, table_name: str = None):
+    async def ls(
+        self,
+        workspace_name_or_id: str = None,
+        base_name: str = None,
+        table_name: str = None,
+    ):
         # coros
         async def _get_records(workspace_name_or_id, base_name):
             bc = await self.get_base_client_with_account_token(
                 workspace_name_or_id=workspace_name_or_id, base_name=base_name
             )
             tables = await bc.list_tables()
             return {
@@ -372,28 +403,34 @@
     # [GROUPS & WORKSPACES] copy base from workspace
     async def copy_base_from_workspace(
         self,
         src_workspace_name_or_id: str,
         src_base_name: str,
         dst_workspace_name_or_id: str,
     ) -> dict:
-        src_workspace = await self.get_workspace(workspace_name_or_id=src_workspace_name_or_id)
-        dst_workspace = await self.get_workspace(workspace_name_or_id=dst_workspace_name_or_id)
+        src_workspace = await self.get_workspace(
+            workspace_name_or_id=src_workspace_name_or_id
+        )
+        dst_workspace = await self.get_workspace(
+            workspace_name_or_id=dst_workspace_name_or_id
+        )
 
         METHOD = "POST"
         URL = f"/api/v2.1/dtable-copy/"
         JSON = {
             "src_workspace_id": src_workspace.id,
             "name": src_base_name,
             "dst_workspace_id": dst_workspace.id,
         }
         ITEM = "dtable"
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = response[ITEM]
 
         return results
 
     # [GROUPS & WORKSPACES] copy base from external link
     async def copy_base_from_external_link(
         self,
@@ -404,30 +441,36 @@
 
         METHOD = "POST"
         URL = f"/api/v2.1/dtable-external-link/dtable-copy/"
         JSON = {"link": link, "dst_workspace_id": dst_workspace.id}
         ITEM = "dtable"
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = response[ITEM]
 
         return results
 
     ################################################################
     # ATTACHMENT
     ################################################################
     # TBD
 
     ################################################################
     # IMPORT & EXPORT
     ################################################################
     # (CUSTOM) Get Table Name and View Name from Table ID and View ID - View ID is Optional
     async def get_ids_by_names(
-        self, workspace_name_or_id: Union[str, int], base_name: str, table_name: str, view_name: str = None
+        self,
+        workspace_name_or_id: Union[str, int],
+        base_name: str,
+        table_name: str,
+        view_name: str = None,
     ):
         bc = await self.get_base_client_with_account_token(
             workspace_name_or_id=workspace_name_or_id, base_name=base_name
         )
         tables = await bc.list_tables()
 
         for table in tables:
@@ -454,21 +497,30 @@
         URL = f"/api/v2.1/workspace/{workspace.id}/synchronous-import/import-excel-csv-to-base/"
         JSON = {"dtable": file, "folder": folder_id}
 
         raise NotImplementedError
 
     # Import Table from xlsx or csv
     async def import_table_from_xlsx_or_csv(
-        self, workspace_name_or_id: Union[str, int], file: bytes, base_uuid: str, table_name: str
+        self,
+        workspace_name_or_id: Union[str, int],
+        file: bytes,
+        base_uuid: str,
+        table_name: str,
     ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "POST"
         URL = f"/api/v2.1/workspace/{workspace.id}/synchronous-import/import-excel-csv-to-table/"
-        JSON = {"workspace_id": workspace.id, "file": file, "dtable_uuid": base_uuid, "table_name": table_name}
+        JSON = {
+            "workspace_id": workspace.id,
+            "file": file,
+            "dtable_uuid": base_uuid,
+            "table_name": table_name,
+        }
         raise NotImplementedError
 
     # Update Table from xlsx or csv
     async def update_base_from_xlsx_or_csv(
         self,
         workspace_name_or_id: Union[str, int],
         file: bytes,
@@ -481,29 +533,33 @@
         METHOD = "POST"
         URL = f"/api/v2.1/workspace/{workspace.id}/synchronous-import/update-table-via-excel-csv/"
         JSON = {
             "workspace_id": workspace.id,
             "file": file,
             "dtable_uuid": base_uuid,
             "table_name": table_name,
-            "selected_columns": ",".join(selected_columns) if isinstance(selected_columns, list) else selected_columns,
+            "selected_columns": ",".join(selected_columns)
+            if isinstance(selected_columns, list)
+            else selected_columns,
         }
         raise NotImplementedError
 
     # Export Base
     # NOT WORKING
     async def export_base(self, workspace_name_or_id: Union[str, int], base_name: str):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace.id}/synchronous-export/export-dtable/"
         PARAMS = {"dtable_name": base_name}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, **PARAMS)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, **PARAMS
+            )
 
         return response
 
     # Export Table
     async def export_table(
         self,
         workspace_name_or_id: Union[str, int],
@@ -518,57 +574,77 @@
         PARAMS = {
             "dtable_name": base_name,
             "table_id": table_id,
             "table_name": table_name,
         }
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, **PARAMS)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, **PARAMS
+            )
 
         return response
 
     # (CUSTOM) Export Table by Name
     async def export_table_by_name(
         self,
         workspace_name_or_id: Union[str, int],
         base_name: str,
         table_name: str = None,
     ):
         table_id = await self.get_ids_by_names(
-            workspace_name_or_id=workspace_name_or_id, base_name=base_name, table_name=table_name
+            workspace_name_or_id=workspace_name_or_id,
+            base_name=base_name,
+            table_name=table_name,
         )
         return await self.export_table(
-            workspace_name_or_id=workspace_name_or_id, base_name=base_name, table_id=table_id, table_name=table_name
+            workspace_name_or_id=workspace_name_or_id,
+            base_name=base_name,
+            table_id=table_id,
+            table_name=table_name,
         )
 
     # Export View
     async def export_view(
-        self, workspace_name_or_id: int, base_name: str, table_id: str, table_name: str, view_id: str, view_name: str
+        self,
+        workspace_name_or_id: int,
+        base_name: str,
+        table_id: str,
+        table_name: str,
+        view_id: str,
+        view_name: str,
     ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace.id}/synchronous-export/export-view-to-excel/"
         PARAMS = {
             "dtable_name": base_name,
             "table_id": table_id,
             "table_name": table_name,
             "view_id": view_id,
             "view_name": view_name,
         }
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, **PARAMS)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, **PARAMS
+            )
 
         return response
 
     # (CUSTOM) Export View by Name
-    async def export_view_by_name(self, workspace_name_or_id: int, base_name: str, table_name: str, view_name: str):
+    async def export_view_by_name(
+        self, workspace_name_or_id: int, base_name: str, table_name: str, view_name: str
+    ):
         table_id, view_id = await self.get_ids_by_names(
-            workspace_name_or_id=workspace_name_or_id, base_name=base_name, table_name=table_name, view_name=view_name
+            workspace_name_or_id=workspace_name_or_id,
+            base_name=base_name,
+            table_name=table_name,
+            view_name=view_name,
         )
 
         return await self.export_view(
             workspace_name_or_id=workspace_name_or_id,
             base_name=base_name,
             table_id=table_id,
             table_name=table_name,
@@ -592,15 +668,18 @@
         if model:
             results = [model(**x) for x in results]
 
         return results
 
     # List User Shares
     async def list_users_share_base(
-        self, workspace_name_or_id: Union[str, int], base_name: str, model: BaseModel = UserInfo
+        self,
+        workspace_name_or_id: Union[str, int],
+        base_name: str,
+        model: BaseModel = UserInfo,
     ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/share/"
         ITEM = "user_list"
 
@@ -634,15 +713,17 @@
         async with self.session_maker(token=self.account_token) as session:
             response = await self.request(session=session, method=METHOD, url=URL)
             results = response[ITEM]
 
         return results
 
     # List Group Shares
-    async def list_tables_shared_to_group(self, workspace_name_or_id: Union[str, int], base_name: str):
+    async def list_tables_shared_to_group(
+        self, workspace_name_or_id: Union[str, int], base_name: str
+    ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/group-shares/"
         ITEM = "dtable_group_share_list"
 
         async with self.session_maker(token=self.account_token) as session:
             response = await self.request(session=session, method=METHOD, url=URL)
@@ -694,15 +775,20 @@
     ################################################################
     # TBD
 
     ################################################################
     # WEBHOOKS
     ################################################################
     # [WEBHOOKS] list webhooks
-    async def list_webhooks(self, workspace_name_or_id: Union[str, int], base_name: str, model: BaseModel = Webhook):
+    async def list_webhooks(
+        self,
+        workspace_name_or_id: Union[str, int],
+        base_name: str,
+        model: BaseModel = Webhook,
+    ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "GET"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/webhooks/"
         ITEM = "webhook_list"
 
         async with self.session_maker(token=self.account_token) as session:
@@ -727,15 +813,17 @@
 
         METHOD = "POST"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/webhooks/"
         JSON = {"url": url, "secret": str(secret)}
         ITEM = "webhook"
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             results = response[ITEM]
 
         if model:
             results = model(**results)
 
         return results
 
@@ -751,19 +839,23 @@
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "PUT"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/webhooks/{webhook_id}/"
         JSON = {"url": url, "secret": str(secret)}
 
         async with self.session_maker(token=self.account_token) as session:
-            response = await self.request(session=session, method=METHOD, url=URL, json=JSON)
+            response = await self.request(
+                session=session, method=METHOD, url=URL, json=JSON
+            )
             print(response)
 
     # [WEBHOOKS] delete webhook
-    async def delete_webhook(self, workspace_name_or_id: Union[str, int], base_name: str, webhook_id: str):
+    async def delete_webhook(
+        self, workspace_name_or_id: Union[str, int], base_name: str, webhook_id: str
+    ):
         workspace = await self.get_workspace(name_or_id=workspace_name_or_id)
 
         METHOD = "DELETE"
         URL = f"/api/v2.1/workspace/{workspace.id}/dtable/{base_name}/webhooks/{webhook_id}/"
         ITEM = "success"
 
         async with self.session_maker(token=self.account_token) as session:
```

### Comparing `plantable-2023.7.3/src/plantable/model/account.py` & `plantable-2023.8.1/src/plantable/model/account.py`

 * *Files identical despite different names*

### Comparing `plantable-2023.7.3/src/plantable/model/core.py` & `plantable-2023.8.1/src/plantable/model/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,17 @@
 
     def to_record(self):
         bases = self.bases or self.shared_bases
         return {
             "type": self.type,
             "workspace_id": self.id,
             "workspace": self.name,
-            "folders": [x["name"] for x in self.folders] if self.folders else self.folders,
+            "folders": [x["name"] for x in self.folders]
+            if self.folders
+            else self.folders,
             "bases": [x.name for x in bases] if bases else bases,
         }
 
 
 class File(_Model):
     filename: str
     content: bytes
```

### Comparing `plantable-2023.7.3/src/plantable/model/event.py` & `plantable-2023.8.1/src/plantable/model/event.py`

 * *Files identical despite different names*

### Comparing `plantable-2023.7.3/src/plantable/model/form.py` & `plantable-2023.8.1/src/plantable/model/form.py`

 * *Files identical despite different names*

### Comparing `plantable-2023.7.3/src/plantable/schema/schema.py` & `plantable-2023.8.1/src/plantable/schema/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,22 @@
     "last_modifier": "last-modifier",
     "mtime": "mtime",
     "auto_number": "auto-number",
 }
 
 STR = {"column_type": "text"}
 LONGTEXT = {"column_type": "long-text"}
-INT = {"column_type": "number", "data": {"format": "number", "decimal": "dot", "thousands": "comma"}}
-FLOAT = {"column_type": "number", "data": {"format": "number", "decimal": "dot", "thousands": "comma"}}
+INT = {
+    "column_type": "number",
+    "data": {"format": "number", "decimal": "dot", "thousands": "comma"},
+}
+FLOAT = {
+    "column_type": "number",
+    "data": {"format": "number", "decimal": "dot", "thousands": "comma"},
+}
 DATETIME = {"column_type": "date", "data": {"format": "YYYY-MM-DD HH:mm"}}
 BOOL = {"column_type": "checkbox"}
 
 BASE = {
     "table_name": "Base",
     "columns": [
         {"column_name": "base_uuid", **STR},  # "uuid"
```

### Comparing `plantable-2023.7.3/src/plantable/scripts.py` & `plantable-2023.8.1/src/plantable/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 @click.option("--reload", is_flag=True)
 @click.option("--workers", type=int, default=None)
 @click.option("--log-level", type=LogLevel(), default=logging.INFO)
 def run(host, port, reload, workers, log_level):
     logging.basicConfig(level=log_level)
 
     if reload:
-        app = "plantable.agent.app:app"
+        app = "plantable.server.app:app"
     else:
-        from .agent.app import app
+        from .server.app import app
 
     uvicorn.run(
         app,
         host=host,
         port=port,
         reload=reload,
         workers=workers,
```

### Comparing `plantable-2023.7.3/src/plantable/serde/from_arrow.py` & `plantable-2023.8.1/src/plantable/serde/from_arrow.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 
 from .const import SYSTEM_FIELDS
 
 # SeaTable dtypes
 CHECKBOX = {"column_type": "checkbox"}
 TEXT = {"column_type": "text"}
 LONG_TEXT = {"column_type": "long-text"}
-INTEGER = {"column_type": "number", "column_data": {"format": "number", "decimal": "dot", "thousands": "comma"}}
-NUMBER = {"column_type": "number", "column_data": {"format": "number", "decimal": "dot", "thousands": "comma"}}
+INTEGER = {
+    "column_type": "number",
+    "column_data": {"format": "number", "decimal": "dot", "thousands": "comma"},
+}
+NUMBER = {
+    "column_type": "number",
+    "column_data": {"format": "number", "decimal": "dot", "thousands": "comma"},
+}
 DURATION = {"column_type": "duration", "column_data": {"format": "h:mm:ss"}}
 DATE = {"column_type": "date", "column_data": {"format": "YYYY-MM-DD"}}
 DATETIME = {"column_type": "date", "column_data": {"format": "YYYY-MM-DD HH:mm"}}
 SINGLE_SELECT = {"column_type": "single-select"}
 MULTIPLE_SELECT = {"column_type": "multiple-select"}
 
 # Arrow to Seatable Schema
@@ -74,21 +80,27 @@
     def dtype_parser(x):
         for pattern in ARROW_STR_DTYPE_PATTERNS:
             r = pattern.parse(x)
             if r:
                 return r.named
 
     def get_rows_for_append(self):
-        return [{k: v for k, v in r.items() if k not in SYSTEM_FIELDS} for r in self.tbl.to_pylist()]
+        return [
+            {k: v for k, v in r.items() if k not in SYSTEM_FIELDS}
+            for r in self.tbl.to_pylist()
+        ]
 
     def get_rows_for_update(self, row_id_field: str = "_id"):
         updates = list()
         for row in self.tbl.to_pylist():
             updates.append(
-                {"row_id": row[row_id_field], "row": {k: v for k, v in row.items() if k not in SYSTEM_FIELDS}}
+                {
+                    "row_id": row[row_id_field],
+                    "row": {k: v for k, v in row.items() if k not in SYSTEM_FIELDS},
+                }
             )
         return updates
 
     def null(self, value):
         pass
 
     def bool(self, value):
```

### Comparing `plantable-2023.7.3/src/plantable/serde/to_python.py` & `plantable-2023.8.1/src/plantable/serde/to_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 ################################################################
 class ToPythonDict:
     def __init__(self, table: Table, users: dict = None):
         self.table = table
         self.users = users
 
         self.columns = {
-            **{column.name: {"column_type": column.type, "column_data": column.data} for column in table.columns},
+            **{
+                column.name: {"column_type": column.type, "column_data": column.data}
+                for column in table.columns
+            },
             **SYSTEM_FIELDS,
         }
 
         self.user_map = (
-            {user.email: f"{user.name} ({user.contact_email})" for user in self.users} if self.users else None
+            {user.email: f"{user.name} ({user.contact_email})" for user in self.users}
+            if self.users
+            else None
         )
         self.row_id_map = {column.key: column.name for column in table.columns}
 
     def __call__(self, row):
         return {
-            column: getattr(self, self.columns[column]["column_type"].replace("-", "_"))(
-                value=row[column], data=self.columns[column].get("column_data")
-            )
+            column: getattr(
+                self, self.columns[column]["column_type"].replace("-", "_")
+            )(value=row[column], data=self.columns[column].get("column_data"))
             for column in self.columns
             if column in row
         }
 
     def checkbox(self, value, data: dict = None) -> bool:
         return value
 
@@ -108,15 +113,17 @@
         if not value:
             return
         if data:
             if "array_type" in data:
                 array_data = data.get("array_data")
                 if not isinstance(value, list):
                     value = [value]
-                value = [getattr(self, data["array_type"])(x, array_data) for x in value]
+                value = [
+                    getattr(self, data["array_type"])(x, array_data) for x in value
+                ]
             link_column = self.columns[self.row_id_map[data["link_column_key"]]]
             if not link_column["column_data"]["is_multiple"]:
                 value = value[0]
         return value
 
     def user(self, user: str):
         if not self.user_map:
```

### Comparing `plantable-2023.7.3/src/plantable.egg-info/SOURCES.txt` & `plantable-2023.8.1/src/plantable.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 src/plantable.egg-info/PKG-INFO
 src/plantable.egg-info/SOURCES.txt
 src/plantable.egg-info/dependency_links.txt
 src/plantable.egg-info/entry_points.txt
 src/plantable.egg-info/requires.txt
 src/plantable.egg-info/top_level.txt
 src/plantable/agent/__init__.py
-src/plantable/agent/app.py
 src/plantable/agent/conf.py
-src/plantable/agent/util.py
-src/plantable/agent/router/__init__.py
-src/plantable/agent/router/api_token.py
-src/plantable/agent/router/user.py
+src/plantable/agent/watcher/__init__.py
+src/plantable/agent/watcher/base_watcher.py
+src/plantable/agent/watcher/view_watcher.py
 src/plantable/client/__init__.py
 src/plantable/client/account.py
 src/plantable/client/admin.py
 src/plantable/client/base.py
 src/plantable/client/base_websocket.py
 src/plantable/client/conf.py
 src/plantable/client/core.py
@@ -32,8 +30,15 @@
 src/plantable/model/form.py
 src/plantable/schema/__init__.py
 src/plantable/schema/schema.py
 src/plantable/serde/__init__.py
 src/plantable/serde/const.py
 src/plantable/serde/from_arrow.py
 src/plantable/serde/to_python.py
+src/plantable/server/__init__.py
+src/plantable/server/app.py
+src/plantable/server/conf.py
+src/plantable/server/util.py
+src/plantable/server/router/__init__.py
+src/plantable/server/router/api_token.py
+src/plantable/server/router/user.py
 src/plantable/static/__init__.py
```


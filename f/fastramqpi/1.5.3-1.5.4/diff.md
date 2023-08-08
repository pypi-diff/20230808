# Comparing `tmp/fastramqpi-1.5.3.tar.gz` & `tmp/fastramqpi-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.5.3.tar", max compression
+gzip compressed data, was "fastramqpi-1.5.4.tar", max compression
```

## Comparing `fastramqpi-1.5.3.tar` & `fastramqpi-1.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0        0        0        0 2023-07-27 06:57:03.418647 fastramqpi-1.5.3/LICENSES/
--rw-r--r--   0        0        0    15177 2023-07-27 06:57:03.418647 fastramqpi-1.5.3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     6602 2023-07-27 06:57:03.418647 fastramqpi-1.5.3/README.md
--rw-r--r--   0        0        0       85 2023-07-27 06:57:03.419647 fastramqpi-1.5.3/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2206 2023-07-27 06:57:03.419647 fastramqpi-1.5.3/fastramqpi/config.py
--rw-r--r--   0        0        0     1298 2023-07-27 06:57:03.419647 fastramqpi-1.5.3/fastramqpi/context.py
--rw-r--r--   0        0        0     1425 2023-07-27 06:57:03.419647 fastramqpi-1.5.3/fastramqpi/depends.py
--rw-r--r--   0        0        0     7150 2023-07-27 06:57:03.419647 fastramqpi-1.5.3/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1577 2023-07-27 06:57:03.420647 fastramqpi-1.5.3/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     6935 2023-07-27 06:57:03.420647 fastramqpi-1.5.3/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-07-27 06:57:03.551659 fastramqpi-1.5.3/fastramqpi/py.typed
--rw-r--r--   0        0        0     1587 2023-07-27 06:57:34.568515 fastramqpi-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     7561 1970-01-01 00:00:00.000000 fastramqpi-1.5.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-08-08 08:02:22.827925 fastramqpi-1.5.4/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-08-08 08:02:22.827925 fastramqpi-1.5.4/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     6676 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/README.md
+-rw-r--r--   0        0        0       85 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/fastramqpi/config.py
+-rw-r--r--   0        0        0     1298 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/fastramqpi/context.py
+-rw-r--r--   0        0        0     1425 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/fastramqpi/depends.py
+-rw-r--r--   0        0        0     7149 2023-08-08 08:02:22.828925 fastramqpi-1.5.4/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-08-08 08:02:22.829925 fastramqpi-1.5.4/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     6935 2023-08-08 08:02:22.829925 fastramqpi-1.5.4/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-08-08 08:02:22.871929 fastramqpi-1.5.4/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1587 2023-08-08 08:02:35.908085 fastramqpi-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7635 1970-01-01 00:00:00.000000 fastramqpi-1.5.4/PKG-INFO
```

### Comparing `fastramqpi-1.5.3/LICENSES/MPL-2.0.txt` & `fastramqpi-1.5.4/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/README.md` & `fastramqpi-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
     "ariadne_codegen.contrib.shorter_results.ShorterResultsPlugin",
 ]
 [tool.ariadne-codegen.scalars.DateTime]
 type = "datetime.datetime"
 [tool.ariadne-codegen.scalars.UUID]
 type = "uuid.UUID"
 ```
+Where you replace `"my_integration/"` with the path to your integration.
+
 Grab OS2mo's GraphQL schema:
 ```bash
 curl -O http://localhost:5000/graphql/v8/schema.graphql
 ```
 Define your queries:
 ```gql
 # queries.graphql
```

### Comparing `fastramqpi-1.5.3/fastramqpi/config.py` & `fastramqpi-1.5.4/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/fastramqpi/context.py` & `fastramqpi-1.5.4/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/fastramqpi/depends.py` & `fastramqpi-1.5.4/fastramqpi/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/fastramqpi/fastapi.py` & `fastramqpi-1.5.4/fastramqpi/fastapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         # Setup FastAPI
         app = FastAPI(
             title=application_name,
             version=self.settings.commit_tag,
             contact={
                 "name": "Magenta Aps",
                 "url": "https://www.magenta.dk/",
-                "email": "info@magenta.dk>",
+                "email": "info@magenta.dk",
             },
             license_info={
                 "name": "MPL-2.0",
                 "url": "https://www.mozilla.org/en-US/MPL/2.0/",
             },
             lifespan=_lifespan,
         )
```

### Comparing `fastramqpi-1.5.3/fastramqpi/healthcheck.py` & `fastramqpi-1.5.4/fastramqpi/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/fastramqpi/main.py` & `fastramqpi-1.5.4/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.3/pyproject.toml` & `fastramqpi-1.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.5.3"
+version = "1.5.4"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
```

### Comparing `fastramqpi-1.5.3/PKG-INFO` & `fastramqpi-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.5.3
+Version: 1.5.4
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -142,14 +142,16 @@
     "ariadne_codegen.contrib.shorter_results.ShorterResultsPlugin",
 ]
 [tool.ariadne-codegen.scalars.DateTime]
 type = "datetime.datetime"
 [tool.ariadne-codegen.scalars.UUID]
 type = "uuid.UUID"
 ```
+Where you replace `"my_integration/"` with the path to your integration.
+
 Grab OS2mo's GraphQL schema:
 ```bash
 curl -O http://localhost:5000/graphql/v8/schema.graphql
 ```
 Define your queries:
 ```gql
 # queries.graphql
```


# Comparing `tmp/nsj_flask_utils-0.1.2.tar.gz` & `tmp/nsj_flask_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_utils-0.1.2.tar", max compression
+gzip compressed data, was "nsj_flask_utils-0.1.3.tar", max compression
```

## Comparing `nsj_flask_utils-0.1.2.tar` & `nsj_flask_utils-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.2/nsj_flask_utils/__init__.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.2/nsj_flask_utils/daos/__init__.py
--rw-r--r--   0        0        0     4238 2023-08-08 12:45:07.643448 nsj_flask_utils-0.1.2/nsj_flask_utils/daos/base_dao.py
--rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.2/nsj_flask_utils/dtos/__init__.py
--rw-r--r--   0        0        0      233 2023-08-08 12:49:50.743121 nsj_flask_utils-0.1.2/nsj_flask_utils/dtos/base_dto.py
--rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.2/nsj_flask_utils/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 19:42:03.906006 nsj_flask_utils-0.1.2/nsj_flask_utils/py.typed
--rw-r--r--   0        0        0        0 2023-08-04 18:34:53.078783 nsj_flask_utils-0.1.2/nsj_flask_utils/service/__init__.py
--rw-r--r--   0        0        0     3153 2023-08-08 12:48:48.643974 nsj_flask_utils-0.1.2/nsj_flask_utils/service/base_service.py
--rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/__init__.py
--rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/error_handlers.py
--rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/filter_params.py
--rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/json.py
--rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/pagination_params.py
--rw-r--r--   0        0        0     3155 2023-08-08 12:43:29.667218 nsj_flask_utils-0.1.2/nsj_flask_utils/utils/request_args.py
--rw-r--r--   0        0        0      508 2023-08-08 12:51:32.553362 nsj_flask_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-08-04 20:16:13.230462 nsj_flask_utils-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 19:16:54.719394 nsj_flask_utils-0.1.3/nsj_flask_utils/__init__.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:10.746192 nsj_flask_utils-0.1.3/nsj_flask_utils/daos/__init__.py
+-rw-r--r--   0        0        0     4238 2023-08-08 12:45:07.643448 nsj_flask_utils-0.1.3/nsj_flask_utils/daos/base_dao.py
+-rw-r--r--   0        0        0       53 2023-08-04 20:08:26.739234 nsj_flask_utils-0.1.3/nsj_flask_utils/dtos/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-08 12:49:50.743121 nsj_flask_utils-0.1.3/nsj_flask_utils/dtos/base_dto.py
+-rw-r--r--   0        0        0      629 2023-08-04 19:15:17.291078 nsj_flask_utils-0.1.3/nsj_flask_utils/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 19:42:03.906006 nsj_flask_utils-0.1.3/nsj_flask_utils/py.typed
+-rw-r--r--   0        0        0       65 2023-08-08 12:58:25.989332 nsj_flask_utils-0.1.3/nsj_flask_utils/service/__init__.py
+-rw-r--r--   0        0        0     3153 2023-08-08 12:48:48.643974 nsj_flask_utils-0.1.3/nsj_flask_utils/service/base_service.py
+-rw-r--r--   0        0        0      212 2023-08-04 20:01:49.619187 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/__init__.py
+-rw-r--r--   0        0        0     1059 2023-08-04 19:16:06.086236 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/error_handlers.py
+-rw-r--r--   0        0        0      147 2023-07-06 20:22:50.549765 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/filter_params.py
+-rw-r--r--   0        0        0      434 2023-08-04 19:57:27.085483 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/json.py
+-rw-r--r--   0        0        0     1051 2023-08-04 19:04:40.476273 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/pagination_params.py
+-rw-r--r--   0        0        0     3155 2023-08-08 12:43:29.667218 nsj_flask_utils-0.1.3/nsj_flask_utils/utils/request_args.py
+-rw-r--r--   0        0        0      508 2023-08-08 12:59:18.110454 nsj_flask_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 nsj_flask_utils-0.1.3/PKG-INFO
```

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/daos/base_dao.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/daos/base_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/exceptions/__init__.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/service/base_service.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/service/base_service.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/error_handlers.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/utils/error_handlers.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/pagination_params.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/utils/pagination_params.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/nsj_flask_utils/utils/request_args.py` & `nsj_flask_utils-0.1.3/nsj_flask_utils/utils/request_args.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_utils-0.1.2/PKG-INFO` & `nsj_flask_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utils for Flask
 License: MIT
 Author: Vinicius Teshima
 Author-email: viniciusteshima@nasajon.com.br
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


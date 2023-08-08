# Comparing `tmp/tap_dbf-0.0.1a2.tar.gz` & `tmp/tap_dbf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbf-0.0.1a2.tar", max compression
+gzip compressed data, was "tap_dbf-0.0.2.tar", max compression
```

## Comparing `tap_dbf-0.0.1a2.tar` & `tap_dbf-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-07 17:07:09.806123 tap_dbf-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     1423 2023-07-07 17:07:09.806123 tap_dbf-0.0.1a2/README.md
--rw-r--r--   0        0        0     2293 2023-07-07 17:07:28.110250 tap_dbf-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-07-07 17:07:09.810123 tap_dbf-0.0.1a2/tap_dbf/__init__.py
--rw-r--r--   0        0        0     6981 2023-07-07 17:07:09.810123 tap_dbf-0.0.1a2/tap_dbf/tap.py
--rw-r--r--   0        0        0     2591 1970-01-01 00:00:00.000000 tap_dbf-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 16:45:37.884030 tap_dbf-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1423 2023-08-08 16:45:37.884030 tap_dbf-0.0.2/README.md
+-rw-r--r--   0        0        0     2264 2023-08-08 16:45:58.780022 tap_dbf-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-08-08 16:45:37.888031 tap_dbf-0.0.2/tap_dbf/__init__.py
+-rw-r--r--   0        0        0     6981 2023-08-08 16:45:37.888031 tap_dbf-0.0.2/tap_dbf/tap.py
+-rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 tap_dbf-0.0.2/PKG-INFO
```

### Comparing `tap_dbf-0.0.1a2/LICENSE` & `tap_dbf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1a2/README.md` & `tap_dbf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1a2/pyproject.toml` & `tap_dbf-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-dbf"
-version = "0.0.1a2"
+version = "0.0.2"
 description = "Singer tap for .DBF files"
 authors = ["Edgar R. Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "dbf",
   "dBase",
 ]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/edgarrmondragon/tap-pulumi-cloud"
-repository = "https://github.com/edgarrmondragon/tap-pulumi-cloud"
-documentation = "https://github.com/edgarrmondragon/tap-pulumi-cloud#readme"
+homepage = "https://github.com/edgarrmondragon/tap-dbf"
+repository = "https://github.com/edgarrmondragon/tap-dbf"
+documentation = "https://github.com/edgarrmondragon/tap-dbf#readme"
 classifiers = [
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.12"
-singer-sdk = "==0.29.0"
+singer-sdk = "==0.31.0"
 dbfread = "==2.0.7"
 fs = "==2.4.16"
 fs-s3fs = {version = "==1.1.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 singer-sdk = {version = "*", extras = ["testing"]}
 pytest-github-actions-annotate-failures = "^0.2.0"
```

### Comparing `tap_dbf-0.0.1a2/tap_dbf/tap.py` & `tap_dbf-0.0.2/tap_dbf/tap.py`

 * *Files identical despite different names*

### Comparing `tap_dbf-0.0.1a2/PKG-INFO` & `tap_dbf-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tap-dbf
-Version: 0.0.1a2
+Version: 0.0.2
 Summary: Singer tap for .DBF files
-Home-page: https://github.com/edgarrmondragon/tap-pulumi-cloud
+Home-page: https://github.com/edgarrmondragon/tap-dbf
 License: Apache-2.0
 Keywords: ELT,singer.io,dbf,dBase
 Author: Edgar R. Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Database
 Provides-Extra: s3
 Requires-Dist: dbfread (==2.0.7)
 Requires-Dist: fs (==2.4.16)
 Requires-Dist: fs-s3fs (==1.1.1) ; extra == "s3"
-Requires-Dist: singer-sdk (==0.29.0)
-Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pulumi-cloud#readme
-Project-URL: Repository, https://github.com/edgarrmondragon/tap-pulumi-cloud
+Requires-Dist: singer-sdk (==0.31.0)
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-dbf#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-dbf
 Description-Content-Type: text/markdown
 
 # tap-dbf
 
 Singer tap for the [dBase file format](https://en.wikipedia.org/wiki/.dbf).
 
 ## Configuration
```


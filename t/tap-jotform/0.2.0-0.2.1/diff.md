# Comparing `tmp/tap_jotform-0.2.0.tar.gz` & `tmp/tap_jotform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_jotform-0.2.0.tar", max compression
+gzip compressed data, was "tap_jotform-0.2.1.tar", max compression
```

## Comparing `tap_jotform-0.2.0.tar` & `tap_jotform-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-07-29 00:55:13.786449 tap_jotform-0.2.0/LICENSE
--rw-r--r--   0        0        0     5067 2023-07-29 00:55:13.786449 tap_jotform-0.2.0/README.md
--rw-r--r--   0        0        0     1845 2023-07-29 00:55:31.034561 tap_jotform-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/__init__.py
--rw-r--r--   0        0        0      116 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/__main__.py
--rw-r--r--   0        0        0     5285 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/client.py
--rw-r--r--   0        0        0     8428 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/streams.py
--rw-r--r--   0        0        0     2738 2023-07-29 00:55:13.790449 tap_jotform-0.2.0/tap_jotform/tap.py
--rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 tap_jotform-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5067 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/README.md
+-rw-r--r--   0        0        0     1849 2023-08-08 16:37:30.050296 tap_jotform-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/tap_jotform/__init__.py
+-rw-r--r--   0        0        0      116 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/tap_jotform/__main__.py
+-rw-r--r--   0        0        0     5285 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/tap_jotform/client.py
+-rw-r--r--   0        0        0     8428 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/tap_jotform/streams.py
+-rw-r--r--   0        0        0     2738 2023-08-08 16:37:08.077289 tap_jotform-0.2.1/tap_jotform/tap.py
+-rw-r--r--   0        0        0     6209 1970-01-01 00:00:00.000000 tap_jotform-0.2.1/PKG-INFO
```

### Comparing `tap_jotform-0.2.0/LICENSE` & `tap_jotform-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.2.0/README.md` & `tap_jotform-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.2.0/pyproject.toml` & `tap_jotform-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core>=1.1",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-jotform"
-version = "0.2.0"
+version = "0.2.1"
 description = "Singer tap for Jotform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-jotform"
 repository = "https://github.com/edgarrmondragon/tap-jotform"
@@ -19,15 +19,15 @@
 keywords = ["ELT", "Jotform"]
 
 [tool.poetry.dependencies]
 colorama = "==0.4.*"
 importlib-metadata = {version = "<5.0.0", python = "<3.8"}
 python = "<3.12,>=3.7.1"
 requests-cache = "==1.1.*"
-singer-sdk = ">=0.28,<0.31"
+singer-sdk = ">=0.31.0,<0.32.0"
 structlog = "==23.1.*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `tap_jotform-0.2.0/tap_jotform/client.py` & `tap_jotform-0.2.1/tap_jotform/client.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.2.0/tap_jotform/streams.py` & `tap_jotform-0.2.1/tap_jotform/streams.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.2.0/tap_jotform/tap.py` & `tap_jotform-0.2.1/tap_jotform/tap.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.2.0/PKG-INFO` & `tap_jotform-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-jotform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Singer tap for Jotform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-jotform
 License: Apache-2.0
 Keywords: ELT,Jotform
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (==0.4.*)
 Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
 Requires-Dist: requests-cache (==1.1.*)
-Requires-Dist: singer-sdk (>=0.28,<0.31)
+Requires-Dist: singer-sdk (>=0.31.0,<0.32.0)
 Requires-Dist: structlog (==23.1.*)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-jotform/#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-jotform
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: tap-jotform Version: 0.2.0 Summary: Singer tap for
+Metadata-Version: 2.1 Name: tap-jotform Version: 0.2.1 Summary: Singer tap for
 Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-jotform License: Apache-2.0 Keywords:
 ELT,Jotform Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: colorama
 (==0.4.*) Requires-Dist: importlib-metadata (<5.0.0) ; python_version < "3.8"
 Requires-Dist: requests-cache (==1.1.*) Requires-Dist: singer-sdk
-(>=0.28,<0.31) Requires-Dist: structlog (==23.1.*) Project-URL: Documentation,
-https://github.com/edgarrmondragon/tap-jotform/#readme Project-URL: Repository,
-https://github.com/edgarrmondragon/tap-jotform Description-Content-Type: text/
-markdown
+(>=0.31.0,<0.32.0) Requires-Dist: structlog (==23.1.*) Project-URL:
+Documentation, https://github.com/edgarrmondragon/tap-jotform/#readme Project-
+URL: Repository, https://github.com/edgarrmondragon/tap-jotform Description-
+Content-Type: text/markdown
                                  # tap-jotform
                        [pre-commit.ci_status] [License]
      Singer Tap for Jotform. Built with the [Meltano Singer SDK](https://
                                sdk.meltano.com).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
 `schema-flattening` ## Settings | Setting | Required | Default | Description |
 |:--------------------|:--------:|:-------:|:------------| | api_key | True |
```


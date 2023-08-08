# Comparing `tmp/tap_readthedocs-0.1.0.tar.gz` & `tmp/tap_readthedocs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_readthedocs-0.1.0.tar", max compression
+gzip compressed data, was "tap_readthedocs-0.1.1.tar", max compression
```

## Comparing `tap_readthedocs-0.1.0.tar` & `tap_readthedocs-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-07 17:29:20.797075 tap_readthedocs-0.1.0/LICENSE
--rw-r--r--   0        0        0     3089 2023-07-07 17:29:20.797075 tap_readthedocs-0.1.0/README.md
--rw-r--r--   0        0        0     2307 2023-07-07 17:29:39.637418 tap_readthedocs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/__init__.py
--rw-r--r--   0        0        0     3690 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/client.py
--rw-r--r--   0        0        0     7367 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/streams.py
--rw-r--r--   0        0        0      836 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/tap.py
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 tap_readthedocs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 15:23:10.920471 tap_readthedocs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3089 2023-08-08 15:23:10.920471 tap_readthedocs-0.1.1/README.md
+-rw-r--r--   0        0        0     2307 2023-08-08 15:23:30.349099 tap_readthedocs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-08-08 15:23:10.920471 tap_readthedocs-0.1.1/tap_readthedocs/__init__.py
+-rw-r--r--   0        0        0     3688 2023-08-08 15:23:10.920471 tap_readthedocs-0.1.1/tap_readthedocs/client.py
+-rw-r--r--   0        0        0     7367 2023-08-08 15:23:10.920471 tap_readthedocs-0.1.1/tap_readthedocs/streams.py
+-rw-r--r--   0        0        0      836 2023-08-08 15:23:10.924471 tap_readthedocs-0.1.1/tap_readthedocs/tap.py
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 tap_readthedocs-0.1.1/PKG-INFO
```

### Comparing `tap_readthedocs-0.1.0/LICENSE` & `tap_readthedocs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.1.0/README.md` & `tap_readthedocs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.1.0/pyproject.toml` & `tap_readthedocs-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-readthedocs"
-version = "0.1.0"
+version = "0.1.1"
 description = "`tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
     "ELT",
     "ReadTheDocs",
     "singer.io",
 ]
@@ -19,15 +19,15 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-readthedocs"
 repository = "https://github.com/edgarrmondragon/tap-readthedocs"
 documentation = "https://github.com/edgarrmondragon/tap-readthedocs#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.29.0"
+singer-sdk = "0.31.0"
 toolz = "0.12.0"
 requests-cache = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 singer-sdk = { version = "*", extras = ["testing"] }
 
 [tool.poetry.scripts]
```

### Comparing `tap_readthedocs-0.1.0/tap_readthedocs/client.py` & `tap_readthedocs-0.1.1/tap_readthedocs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
             raise RetriableAPIError(response.reason)
         super().validate_response(response)
 
     def get_url_params(
         self,
         context: dict | None,  # noqa: ARG002
-        next_page_token: t.Any | None,
+        next_page_token: int | None,
     ) -> dict[str, t.Any]:
         """Get URL query parameters.
 
         Args:
             context: Stream sync context.
             next_page_token: Next offset.
```

### Comparing `tap_readthedocs-0.1.0/tap_readthedocs/streams.py` & `tap_readthedocs-0.1.1/tap_readthedocs/streams.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.1.0/tap_readthedocs/tap.py` & `tap_readthedocs-0.1.1/tap_readthedocs/tap.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.1.0/PKG-INFO` & `tap_readthedocs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tap-readthedocs
-Version: 0.1.0
+Version: 0.1.1
 Summary: `tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0
 Keywords: ELT,ReadTheDocs,singer.io
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: singer-sdk (==0.29.0)
+Requires-Dist: singer-sdk (==0.31.0)
 Requires-Dist: toolz (==0.12.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-readthedocs#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readthedocs
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.1.0 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.1.1 Summary: `tap-
 readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0 Keywords: ELT,ReadTheDocs,singer.io Author: Edgar RamÃ­rez-
 MondragÃ³n Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: requests-cache (>=1.0.1,<2.0.0) Requires-Dist:
-singer-sdk (==0.29.0) Requires-Dist: toolz (==0.12.0) Project-URL:
+singer-sdk (==0.31.0) Requires-Dist: toolz (==0.12.0) Project-URL:
 Documentation, https://github.com/edgarrmondragon/tap-readthedocs#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readthedocs
 Description-Content-Type: text/markdown
                                # tap-readthedocs
             [pre-commit.ci_status] [Ruff] [Nox] [License] [License]
 Singer Tap for [**Read the Docs**](https://docs.readthedocs.io). Built with the
                 [Meltano Singer SDK](https://sdk.meltano.com).
```


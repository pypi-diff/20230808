# Comparing `tmp/google_ads_report-0.2.1.tar.gz` & `tmp/google_ads_report-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ads_report-0.2.1.tar", max compression
+gzip compressed data, was "google_ads_report-0.3.0.tar", max compression
```

## Comparing `google_ads_report-0.2.1.tar` & `google_ads_report-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/LICENSE
--rw-r--r--   0        0        0      785 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/README.md
--rw-r--r--   0        0        0       88 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/__init__.py
--rw-r--r--   0        0        0     6121 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/base_client.py
--rw-r--r--   0        0        0     1486 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/google_ads_client.py
--rw-r--r--   0        0        0      445 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/google_ads_report/google_search_ads_client.py
--rw-r--r--   0        0        0     2593 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      988 2023-08-04 07:58:41.120173 google_ads_report-0.2.1/tests/test_app.py
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 google_ads_report-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/LICENSE
+-rw-r--r--   0        0        0      785 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/README.md
+-rw-r--r--   0        0        0       88 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/google_ads_report/__init__.py
+-rw-r--r--   0        0        0     6121 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/google_ads_report/base_client.py
+-rw-r--r--   0        0        0     1974 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/google_ads_report/google_ads_client.py
+-rw-r--r--   0        0        0      445 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/google_ads_report/google_search_ads_client.py
+-rw-r--r--   0        0        0     2593 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      988 2023-08-08 07:19:48.508728 google_ads_report-0.3.0/tests/test_app.py
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 google_ads_report-0.3.0/PKG-INFO
```

### Comparing `google_ads_report-0.2.1/LICENSE` & `google_ads_report-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.1/README.md` & `google_ads_report-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.1/google_ads_report/base_client.py` & `google_ads_report-0.3.0/google_ads_report/base_client.py`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.1/google_ads_report/google_ads_client.py` & `google_ads_report-0.3.0/google_ads_report/google_ads_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,35 @@
 from typing import Iterator
 from google.protobuf import json_format
 from google.ads.googleads.client import GoogleAdsClient  # type: ignore
 from .base_client import BaseClient
 
 
 class GoogleAdsApiClient(BaseClient):
-    def __init__(self, credentials_path: str = None, version: str = "v14"):
+    def __init__(self, credentials: dict = None, credentials_path: str = None, version: str = "v14"):
+        """
+        Args:
+            credentials: A dictionary of credentials for the Google Ads API.
+            credentials_path: The path to a JSON file containing credentials for the Google Ads API.
+            version: The version of the Google Ads API to use.
+
+        Returns:
+            An instance of the GoogleAdsApiClient class.
+
+        Author:
+            minhpc@ikameglobal.com
+        """
         super().__init__(version)
 
-        if not credentials_path:
-            raise ValueError("Specify the path to your googleads_credentials.json file")
+        if not credentials_path and not credentials:
+            raise ValueError("Either credentials or credentials_path must be provided.")
 
-        with open(credentials_path, 'r') as f:
-            credentials = json.load(f)
+        if not credentials:
+            with open(credentials_path, 'r') as f:
+                credentials = json.load(f)
 
         self.client = GoogleAdsClient.load_from_dict(credentials, version)
         self.ads_service = self.client.get_service("GoogleAdsService")
         self.version = version
 
     def get_response_batch(self, customer_id: str, query: str) -> Iterator[dict]:
         """
```

### Comparing `google_ads_report-0.2.1/pyproject.toml` & `google_ads_report-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-ads-report"
-version = "0.2.1"
+version = "0.3.0"
 homepage = "https://github.com/ikameglobal/google-ads-report"
 description = "Easier to use"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `google_ads_report-0.2.1/tests/test_app.py` & `google_ads_report-0.3.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `google_ads_report-0.2.1/PKG-INFO` & `google_ads_report-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ads-report
-Version: 0.2.1
+Version: 0.3.0
 Summary: Easier to use
 Home-page: https://github.com/ikameglobal/google-ads-report
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```


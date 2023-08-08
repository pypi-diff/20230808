# Comparing `tmp/stowrap-0.0.3.tar.gz` & `tmp/stowrap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stowrap-0.0.3.tar", last modified: Sun Aug  6 14:18:25 2023, max compression
+gzip compressed data, was "stowrap-0.0.4.tar", last modified: Tue Aug  8 12:27:17 2023, max compression
```

## Comparing `stowrap-0.0.3.tar` & `stowrap-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-06 14:18:16.000000 stowrap-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-06 14:18:25.636995 stowrap-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-06 14:18:16.000000 stowrap-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 14:18:25.636995 stowrap-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-06 14:18:16.000000 stowrap-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.632995 stowrap-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/src/stowrap/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-06 14:18:16.000000 stowrap-0.0.3/src/stowrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-06 14:18:16.000000 stowrap-0.0.3/src/stowrap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/src/stowrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-06 14:18:25.000000 stowrap-0.0.3/src/stowrap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 14:18:25.636995 stowrap-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-06 14:18:16.000000 stowrap-0.0.3/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:17.599928 stowrap-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 12:27:07.000000 stowrap-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-08 12:27:17.599928 stowrap-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 12:27:07.000000 stowrap-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:27:17.599928 stowrap-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-08 12:27:07.000000 stowrap-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:17.591928 stowrap-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:17.595928 stowrap-0.0.4/src/stowrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-08 12:27:07.000000 stowrap-0.0.4/src/stowrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-08 12:27:07.000000 stowrap-0.0.4/src/stowrap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:17.599928 stowrap-0.0.4/src/stowrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-08 12:27:17.000000 stowrap-0.0.4/src/stowrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-08 12:27:17.000000 stowrap-0.0.4/src/stowrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:27:17.000000 stowrap-0.0.4/src/stowrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 12:27:17.000000 stowrap-0.0.4/src/stowrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 12:27:17.000000 stowrap-0.0.4/src/stowrap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:27:17.599928 stowrap-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 12:27:07.000000 stowrap-0.0.4/tests/test_upload.py
```

### Comparing `stowrap-0.0.3/LICENSE` & `stowrap-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stowrap-0.0.3/PKG-INFO` & `stowrap-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stowrap
-Version: 0.0.3
+Version: 0.0.4
 Summary: stowrap: Python Storage Service Wrapper.
 Home-page: https://github.com/yokoe/stowrap
 Download-URL: https://github.com/yokoe/stowrap
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
```

### Comparing `stowrap-0.0.3/setup.py` & `stowrap-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "stowrap: Python Storage Service Wrapper."
 NAME = "stowrap"
 AUTHOR = "yokoe"
 AUTHOR_EMAIL = "kreuz45@kreuz45.com"
 URL = "https://github.com/yokoe/stowrap"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 PYTHON_REQUIRES = ">=3.9"
 INSTALL_REQUIRES = [
     "gcshus",
     "boto3",
 ]
 PACKAGES = ["stowrap"]
 PACKAGE_DIR = {"": "src"}
```

### Comparing `stowrap-0.0.3/src/stowrap/client.py` & `stowrap-0.0.4/src/stowrap/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     pass
 
 
 class UnsupportedOperation(Exception):
     pass
 
 
+class NotServiceAccountException(Exception):
+    pass
+
+
 @dataclasses.dataclass
 class UploadResult:
     url: str
 
 
 class Client:
     def __init__(self, service) -> None:
@@ -28,26 +32,47 @@
             return
 
         raise UnsupportedService(f"Unsupported service: {service}")
 
     def upload(self, bucket, src_file, dst_file) -> UploadResult:
         return self.storage_service.upload(bucket, src_file, dst_file)
 
+    def generate_download_url(self, bucket, file, mins) -> str:
+        return self.storage_service.generate_download_url(bucket, file, mins)
+
 
 class StorageService:
     def upload(self, bucket, src_file, dst_file) -> UploadResult:
         raise UnsupportedOperation("Upload operation is not supported")
 
+    def generate_download_url(self, bucket, file, mins) -> str:
+        raise UnsupportedOperation("Download URL generation is not supported")
+
 
 class GCS(StorageService):
     def __init__(self) -> None:
         self.gcs_client = storage.Client()
 
     def upload(self, bucket, src_file, dst_file) -> UploadResult:
         gcshus.upload(self.gcs_client, bucket, src_file, dst_file)
         return UploadResult(f"https://storage.googleapis.com/{bucket}/{dst_file}")
 
+    def generate_download_url(self, bucket, file, mins) -> str:
+        try:
+            return gcshus.generate_download_signed_url_with_token_refresh(
+                self.gcs_client, bucket, file, mins * 60
+            )
+        except gcshus.NotServiceAccountException:
+            raise NotServiceAccountException("GCS client is not a service account. ")
+
 
 class S3(StorageService):
     def upload(self, bucket, src_file, dst_file) -> UploadResult:
         boto3.resource("s3").Bucket(bucket).upload_file(src_file, dst_file)
         return UploadResult(f"https://{bucket}.s3.amazonaws.com/{dst_file}")
+
+    def generate_download_url(self, bucket, file, mins) -> str:
+        return boto3.client("s3").generate_presigned_url(
+            "get_object",
+            Params={"Bucket": bucket, "Key": file},
+            ExpiresIn=mins * 60,
+        )
```

### Comparing `stowrap-0.0.3/src/stowrap.egg-info/PKG-INFO` & `stowrap-0.0.4/src/stowrap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stowrap
-Version: 0.0.3
+Version: 0.0.4
 Summary: stowrap: Python Storage Service Wrapper.
 Home-page: https://github.com/yokoe/stowrap
 Download-URL: https://github.com/yokoe/stowrap
 Author: yokoe
 Author-email: kreuz45@kreuz45.com
 Maintainer: yokoe
 Maintainer-email: kreuz45@kreuz45.com
```


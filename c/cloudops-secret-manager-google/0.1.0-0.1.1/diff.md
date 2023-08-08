# Comparing `tmp/cloudops_secret_manager_google-0.1.0.tar.gz` & `tmp/cloudops_secret_manager_google-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudops_secret_manager_google-0.1.0.tar", max compression
+gzip compressed data, was "cloudops_secret_manager_google-0.1.1.tar", max compression
```

## Comparing `cloudops_secret_manager_google-0.1.0.tar` & `cloudops_secret_manager_google-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       33 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/cloudops/__init__.py
--rw-r--r--   0        0        0        0 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/cloudops/secret_manager/__init__.py
--rw-r--r--   0        0        0       98 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/cloudops/secret_manager/google/__init__.py
--rw-r--r--   0        0        0     2091 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/cloudops/secret_manager/google/secret.py
--rw-r--r--   0        0        0      679 2022-10-27 11:06:22.366863 cloudops_secret_manager_google-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 cloudops_secret_manager_google-0.1.0/setup.py
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 cloudops_secret_manager_google-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/cloudops/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/cloudops/secret_manager/__init__.py
+-rw-r--r--   0        0        0       86 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/cloudops/secret_manager/google/__init__.py
+-rw-r--r--   0        0        0     1915 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/cloudops/secret_manager/google/secret.py
+-rw-r--r--   0        0        0      679 2023-08-08 09:47:17.551787 cloudops_secret_manager_google-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 cloudops_secret_manager_google-0.1.1/PKG-INFO
```

### Comparing `cloudops_secret_manager_google-0.1.0/cloudops/secret_manager/google/secret.py` & `cloudops_secret_manager_google-0.1.1/cloudops/secret_manager/google/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,37 @@
 import logging
 
 import google_crc32c
 from google.api_core.exceptions import AlreadyExists
 from google.cloud import secretmanager
 
 
-class GoogleSecret:
+class Secret:
     def __init__(self, project_id: str, secret_id: str):
         self.project_id = project_id
         self.secret_id = secret_id
         self.client = secretmanager.SecretManagerServiceClient()
-        self.initialize()
 
-    def initialize(self) -> None:
-        logging.info("Creating secret...")
-        try:
-            self.client.create_secret(
-                request={
-                    "parent": f"projects/{self.project_id}",
-                    "secret_id": self.secret_id,
-                    "secret": {"replication": {"automatic": {}}},
-                }
-            )
-            logging.info(f"Created secret {self.secret_id}")
-
-        except AlreadyExists:
-            logging.info(f"Secret {self.secret_id} already exists")
+    def create(self) -> None:
+        self.client.create_secret(
+            request={
+                "parent": f"projects/{self.project_id}",
+                "secret_id": self.secret_id,
+                "secret": {"replication": {"automatic": {}}},
+            }
+        )
+        logging.info(f"Created secret {self.secret_id}")
 
     def pull(self) -> dict:
         logging.info("Pulling latest secret version...")
-        name = self.client.secret_version_path(self.project_id, self.secret_id, "latest")
+        name = self.client.secret_version_path(
+            self.project_id,
+            self.secret_id,
+            "latest",
+        )
         response = self.client.access_secret_version(request={"name": name})
         crc32c = google_crc32c.Checksum()
         crc32c.update(response.payload.data)
         if response.payload.data_crc32c != int(crc32c.hexdigest(), 16):
             print("Data corruption detected.")
             raise ValueError("Data corruption detected.")
```

### Comparing `cloudops_secret_manager_google-0.1.0/pyproject.toml` & `cloudops_secret_manager_google-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cloudops-secret-manager-google"
 packages = [{include = "cloudops"}]
-version = "0.1.0"
+version = "0.1.1"
 description = "The cloudops-secret-manager-google package"
 authors = ["Manuel Castillo <manucalop@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/manucalop/cloudops-secret-manager-google"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```


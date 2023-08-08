# Comparing `tmp/dassana-0.9.0.tar.gz` & `tmp/dassana-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.9.0.tar", last modified: Thu Aug  3 18:56:37 2023, max compression
+gzip compressed data, was "dassana-0.9.1.tar", last modified: Tue Aug  8 09:35:42 2023, max compression
```

## Comparing `dassana-0.9.0.tar` & `dassana-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:56:37.904365 dassana-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-03 18:56:37.904365 dassana-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-03 18:56:26.000000 dassana-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:56:37.900365 dassana-0.9.0/dassana/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 18:56:26.000000 dassana-0.9.0/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-08-03 18:56:26.000000 dassana-0.9.0/dassana/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-03 18:56:26.000000 dassana-0.9.0/dassana/dassana_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:56:37.904365 dassana-0.9.0/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 18:56:37.000000 dassana-0.9.0/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:56:37.904365 dassana-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-03 18:56:26.000000 dassana-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:35:42.954155 dassana-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 09:35:42.954155 dassana-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 09:35:34.000000 dassana-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:35:42.954155 dassana-0.9.1/dassana/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 09:35:34.000000 dassana-0.9.1/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-08-08 09:35:34.000000 dassana-0.9.1/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-08 09:35:34.000000 dassana-0.9.1/dassana/dassana_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:35:42.954155 dassana-0.9.1/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 09:35:42.000000 dassana-0.9.1/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:35:42.954155 dassana-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 09:35:34.000000 dassana-0.9.1/setup.py
```

### Comparing `dassana-0.9.0/dassana/common.py` & `dassana-0.9.1/dassana/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     headers = {
         "x-dassana-tenant-id": tenant_id,
         "Authorization": f"Bearer {access_token}", 
     }
     res = requests.post(ingestion_service_url +"/job/"+job_id+"/"+fail_type, headers=headers, json={
         "metadata": metadata
     })
-    print("Ingestion status updated to failed")
+    print("Ingestion status updated to " + str(fail_type))
     return res.json()
 
 @retry(wait=wait_fixed(30), stop=stop_after_attempt(3))
 def get_ingestion_details(tenant_id, source, record_type, config_id, metadata, priority, is_snapshot):
     access_token = get_access_token()
 
     headers = {
@@ -362,15 +362,15 @@
                 cancel_ingestion_job(self.job_id, self.tenant_id, {}, "cancel")
             except:
                 raise
             
     def close(self, pass_counter, fail_counter):
         self.file.close()
         metadata = {}
-        job_result = {"status": "done", "pass" : int(pass_counter), "fail": int(fail_counter)}
+        job_result = {"status": "ready_for_download", "source": {"pass" : int(pass_counter), "fail": int(fail_counter)}}
         metadata["job_result"] = job_result
         if self.bytes_written > 0:
             self.compress_file()
             self.upload_to_cloud()
             print(f"Ingested remaining data: {self.bytes_written} bytes")
             self.bytes_written = 0
         update_ingestion_to_done(self.job_id, self.tenant_id, metadata)
```

### Comparing `dassana-0.9.0/dassana/dassana_env.py` & `dassana-0.9.1/dassana/dassana_env.py`

 * *Files identical despite different names*

### Comparing `dassana-0.9.0/setup.py` & `dassana-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="dassana",
-    version="0.9.0",
+    version="0.9.1",
     description="Dassana common data ingestion utilities",
     long_description="Dassana common data ingestion utilities",
     url="https://github.com/dassana-io/dassana-python",
     author="Dassana",
     author_email="support@dassana.io",
     license="MIT",
     packages=["dassana"],
```


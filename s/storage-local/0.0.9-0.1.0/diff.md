# Comparing `tmp/storage-local-0.0.9.tar.gz` & `tmp/storage-local-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-local-0.0.9.tar", last modified: Sun Aug  6 17:31:37 2023, max compression
+gzip compressed data, was "storage-local-0.1.0.tar", last modified: Tue Aug  8 10:46:23 2023, max compression
```

## Comparing `storage-local-0.0.9.tar` & `storage-local-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-06 17:31:37.346613 storage-local-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-06 17:31:12.000000 storage-local-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-06 17:31:12.000000 storage-local-0.0.9/circles_local_aws_s3_storage_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-06 17:31:12.000000 storage-local-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 17:31:37.346613 storage-local-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-06 17:31:12.000000 storage-local-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/storage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-06 17:31:37.000000 storage-local-0.0.9/storage_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:37.346613 storage-local-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-06 17:31:12.000000 storage-local-0.0.9/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:23.140908 storage-local-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-08 10:46:23.140908 storage-local-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 10:46:00.000000 storage-local-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:23.140908 storage-local-0.1.0/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 10:46:00.000000 storage-local-0.1.0/circles_local_aws_s3_storage_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 10:46:00.000000 storage-local-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:46:23.140908 storage-local-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 10:46:00.000000 storage-local-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:23.140908 storage-local-0.1.0/storage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-08 10:46:23.000000 storage-local-0.1.0/storage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 10:46:23.000000 storage-local-0.1.0/storage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:46:23.000000 storage-local-0.1.0/storage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-08 10:46:23.000000 storage-local-0.1.0/storage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:23.140908 storage-local-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 10:46:00.000000 storage-local-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 10:46:00.000000 storage-local-0.1.0/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-08 10:46:00.000000 storage-local-0.1.0/tests/test_circles_storage.py
```

### Comparing `storage-local-0.0.9/circles_local_aws_s3_storage_python/AWSStorage.py` & `storage-local-0.1.0/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/circles_local_aws_s3_storage_python/CirclesStorage.py` & `storage-local-0.1.0/circles_local_aws_s3_storage_python/CirclesStorage.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,15 +66,22 @@
         """
         select_stmt = "SELECT created_user_id, path, filename FROM storage.storage_table WHERE id = %s"
         select_data = (storage_id)
         self.db.cursor.execute(select_stmt, [select_data])
         profile_id, folder, file_name = self.db.cursor.fetchall()[0]
         path_local = os.path.join(os.getcwd(), file_name)
         self.s3.download_file(folder+file_name,path_local)
+        return path_local
         
+    def system_check(self):
+        cursor =  self.db.cursor
+        sql_query = f"DESCRIBE logger.logger_table"
+        cursor.execute(sql_query)
+        columns_info = cursor.fetchall()
+        print(columns_info)
 
 
     def download(self, profile_id, entity_type_id, file_name, local_path):
         """Downlaods file from S3 to local computer
 
         Args:
             entity_type_id int: 1 - Profile Image
```

### Comparing `storage-local-0.0.9/circles_local_aws_s3_storage_python/FileTypeDB.py` & `storage-local-0.1.0/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageDB.py` & `storage-local-0.1.0/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/circles_local_aws_s3_storage_python/StorageInterface.py` & `storage-local-0.1.0/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/setup.py` & `storage-local-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='storage-local',
-    version='0.0.9', # https://pypi.org/project/storage-local/
+    version='0.1.0', # https://pypi.org/project/storage-local/
     author="Circles",
     author_email="info@circle.zone",
     description="PyPI Package for Circles Storage functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

### Comparing `storage-local-0.0.9/storage_local.egg-info/SOURCES.txt` & `storage-local-0.1.0/storage_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/tests/test_S3.py` & `storage-local-0.1.0/tests/test_S3.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.9/tests/test_circles_storage.py` & `storage-local-0.1.0/tests/test_circles_storage.py`

 * *Files identical despite different names*


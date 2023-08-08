# Comparing `tmp/galaxy-fds-sdk-1.4.8.tar.gz` & `tmp/galaxy-fds-sdk-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galaxy-fds-sdk-1.4.8.tar", last modified: Wed Oct 24 07:10:27 2018, max compression
+gzip compressed data, was "dist/galaxy-fds-sdk-1.4.9.tar", last modified: Tue Oct 30 07:05:15 2018, max compression
```

## Comparing `galaxy-fds-sdk-1.4.8.tar` & `galaxy-fds-sdk-1.4.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/test/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      919 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/test/testMultithreading.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      132 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/test/test_common.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     2259 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/test/test_fdscli_cli.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      534 2018-10-24 07:10:09.000000 galaxy-fds-sdk-1.4.8/setup.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      217 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/PKG-INFO
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/fds/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     3157 2018-10-24 07:10:09.000000 galaxy-fds-sdk-1.4.8/fds/fds_client_configuration.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)    53930 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/galaxy_fds_client.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      967 2018-10-24 02:31:55.000000 galaxy-fds-sdk-1.4.8/fds/utils.py
--rwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)    41131 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/fds_cli.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1733 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/fds_request.py
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/fds/model/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      547 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/subresource.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      484 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_bucket.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      632 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/upload_part_result.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4527 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/permission.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      246 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/init_multipart_upload_result.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      421 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_object.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4571 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_lifecycle.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      127 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.8/fds/model/__init__.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      198 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_object_summary.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1037 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/timestamp_anti_stealing_link_config.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      954 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/access_control_policy.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      421 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/upload_part_result_list.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      449 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/put_object_result.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1218 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_object_metadata.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      496 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/copy_object_result.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     2299 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/model/fds_object_listing.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      210 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/__init__.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      703 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/test_utils.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      264 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/galaxy_fds_client_exception.py
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/fds/auth/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1082 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/auth/common.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       27 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.8/fds/auth/__init__.py
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/fds/auth/signature/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     5451 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.8/fds/auth/signature/signer.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       27 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.8/fds/auth/signature/__init__.py
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)    24691 2018-10-24 02:31:55.000000 galaxy-fds-sdk-1.4.8/fds/fdscli_cli.py
-drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)        1 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      217 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       71 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)        4 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/top_level.txt
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       72 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/requires.txt
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1111 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       38 2018-10-24 07:10:27.000000 galaxy-fds-sdk-1.4.8/setup.cfg
--rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4570 2018-09-11 07:34:56.000000 galaxy-fds-sdk-1.4.8/README.md
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/test/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      919 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/test/testMultithreading.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      132 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/test/test_common.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     2259 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/test/test_fdscli_cli.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      534 2018-10-30 07:04:33.000000 galaxy-fds-sdk-1.4.9/setup.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      217 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/PKG-INFO
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/fds/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     3157 2018-10-24 07:10:09.000000 galaxy-fds-sdk-1.4.9/fds/fds_client_configuration.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)    53930 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/galaxy_fds_client.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      967 2018-10-24 02:31:55.000000 galaxy-fds-sdk-1.4.9/fds/utils.py
+-rwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)    41131 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/fds_cli.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1733 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/fds_request.py
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/fds/model/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      547 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/subresource.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      484 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_bucket.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      632 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/upload_part_result.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4527 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/permission.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      246 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/init_multipart_upload_result.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      421 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_object.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4571 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_lifecycle.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      127 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.9/fds/model/__init__.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      198 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_object_summary.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1037 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/timestamp_anti_stealing_link_config.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      954 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/access_control_policy.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      421 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/upload_part_result_list.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      449 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/put_object_result.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1218 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_object_metadata.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      496 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/copy_object_result.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     2299 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/model/fds_object_listing.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      210 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/__init__.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      703 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/test_utils.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      264 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/galaxy_fds_client_exception.py
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/fds/auth/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1082 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/auth/common.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       27 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.9/fds/auth/__init__.py
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/fds/auth/signature/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     5451 2018-10-12 08:33:09.000000 galaxy-fds-sdk-1.4.9/fds/auth/signature/signer.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       27 2018-08-29 12:20:33.000000 galaxy-fds-sdk-1.4.9/fds/auth/signature/__init__.py
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)    24196 2018-10-30 07:04:33.000000 galaxy-fds-sdk-1.4.9/fds/fdscli_cli.py
+drwxrwxr-x   0 maxiaoxin  (1000) maxiaoxin  (1000)        0 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)        1 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)      217 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       71 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)        4 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       72 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/requires.txt
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     1111 2018-10-30 07:05:14.000000 galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)       38 2018-10-30 07:05:15.000000 galaxy-fds-sdk-1.4.9/setup.cfg
+-rw-rw-r--   0 maxiaoxin  (1000) maxiaoxin  (1000)     4570 2018-09-11 07:34:56.000000 galaxy-fds-sdk-1.4.9/README.md
```

### Comparing `galaxy-fds-sdk-1.4.8/test/testMultithreading.py` & `galaxy-fds-sdk-1.4.9/test/testMultithreading.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/test/test_fdscli_cli.py` & `galaxy-fds-sdk-1.4.9/test/test_fdscli_cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/setup.py` & `galaxy-fds-sdk-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
   name='galaxy-fds-sdk',
-  version='1.4.8',
+  version='1.4.9',
   author='haxiaolin',
   author_email='haxiaolin@xiaomi.com',
   include_package_data=True,
   install_requires=[
     'requests>=2.6.0',
     'argcomplete>=1.4.1',
     'fire',
```

### Comparing `galaxy-fds-sdk-1.4.8/fds/fds_client_configuration.py` & `galaxy-fds-sdk-1.4.9/fds/fds_client_configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/galaxy_fds_client.py` & `galaxy-fds-sdk-1.4.9/fds/galaxy_fds_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/utils.py` & `galaxy-fds-sdk-1.4.9/fds/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/fds_cli.py` & `galaxy-fds-sdk-1.4.9/fds/fds_cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/fds_request.py` & `galaxy-fds-sdk-1.4.9/fds/fds_request.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/subresource.py` & `galaxy-fds-sdk-1.4.9/fds/model/subresource.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/upload_part_result.py` & `galaxy-fds-sdk-1.4.9/fds/model/upload_part_result.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/permission.py` & `galaxy-fds-sdk-1.4.9/fds/model/permission.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/fds_lifecycle.py` & `galaxy-fds-sdk-1.4.9/fds/model/fds_lifecycle.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/timestamp_anti_stealing_link_config.py` & `galaxy-fds-sdk-1.4.9/fds/model/timestamp_anti_stealing_link_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/access_control_policy.py` & `galaxy-fds-sdk-1.4.9/fds/model/access_control_policy.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/fds_object_metadata.py` & `galaxy-fds-sdk-1.4.9/fds/model/fds_object_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/model/fds_object_listing.py` & `galaxy-fds-sdk-1.4.9/fds/model/fds_object_listing.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/test_utils.py` & `galaxy-fds-sdk-1.4.9/fds/test_utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/auth/common.py` & `galaxy-fds-sdk-1.4.9/fds/auth/common.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/auth/signature/signer.py` & `galaxy-fds-sdk-1.4.9/fds/auth/signature/signer.py`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/fds/fdscli_cli.py` & `galaxy-fds-sdk-1.4.9/fds/fdscli_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,30 +35,14 @@
       os.makedirs(path)
   except OSError as exc:
     if exc.errno == errno.EEXIST and os.path.isdir(
         os.path.join(os.path.expanduser("~"), ".config", "xiaomi")):
       pass
 
 
-def async_task(fds_client, upload_token, part_number, data):
-  for i in range(max_upload_retry_time):
-    try:
-      rtn = fds_client.upload_part(bucket_name=upload_token.bucket_name,
-                                   object_name=upload_token.object_name,
-                                   upload_id=upload_token.upload_id,
-                                   part_number=part_number,
-                                   data=data)
-      return rtn
-    except GalaxyFDSClientException:
-      sleep_seconds = (i + 1) * 10
-      CLIPrinter.warn("upload part %d failed, retry after %d seconds" % (
-        part_number, sleep_seconds))
-      time.sleep(sleep_seconds)
-
-
 class LocalConfig(object):
   def __init__(self):
     self.__config_path = os.path.join(
       os.path.expanduser("~"), ".config", "xiaomi", "config")
     mkdirs(os.path.join(os.path.expanduser("~"), ".config", "xiaomi"))
 
     self.__data = None
@@ -616,15 +600,14 @@
     elif sync:
       dst_object_name = filename[2:]
     elif dst_url.is_object_dir():
       dst_object_name = dst_url.object_dir() + os.path.basename(filename)
     else:
       dst_object_name = os.path.basename(filename)
 
-
     if self._fds.does_object_exists(dst_bucket_name, dst_object_name):
       # check md5 firstly
       metadata = self._fds.get_object_metadata(dst_bucket_name, dst_object_name)
       if metadata.metadata.get(Common.CONTENT_MD5) is not None:
         local_md5 = file_md5(filename)
         if local_md5 == metadata.metadata.get(Common.CONTENT_MD5):
           CLIPrinter.done('upload object %s/%s(skip because of same md5)' % (dst_bucket_name, dst_object_name))
@@ -644,23 +627,50 @@
         return
     mimetype = None
     if autodetect_mimetype:
       mimetype = mimetypes.guess_type(filename)[0]
     metadata = FDSObjectMetadata()
     if mimetype is not None:
       metadata.add_header(Common.CONTENT_TYPE, mimetype)
+    result = None
     with open(filename, "rb") as f:
       file_length = os.path.getsize(filename)
       if file_length < multipart_upload_buffer_size:
         try:
           result = self._fds.put_object(dst_bucket_name, dst_object_name, f, metadata=metadata)
         except GalaxyFDSClientException as e:
           CLIPrinter.fail(e.args)
       else:
-        result = self._upload_concurrency(dst_bucket_name, dst_object_name, f, metadata)
+        try:
+          upload_token = self._fds.init_multipart_upload(dst_bucket_name, dst_object_name)
+          part_number = 1
+          result_list = []
+          while True:
+            data = f.read(multipart_upload_buffer_size)
+            if len(data) <= 0:
+              break
+            for i in range(max_upload_retry_time):
+              upload_result = None
+              try:
+                upload_result = self._fds.upload_part(dst_bucket_name, dst_object_name, upload_token.upload_id, part_number, data)
+                result_list.append(upload_result)
+                break
+              except GalaxyFDSClientException as e:
+                sleep_seconds = (i + 1) * 10
+                CLIPrinter.warn("upload part %d failed, retry after %d seconds" % (
+                  part_number, sleep_seconds))
+                time.sleep(sleep_seconds)
+            part_number = part_number + 1
+          upload_part_result = UploadPartResultList({"uploadPartResultList": result_list})
+          result = self._fds.complete_multipart_upload(upload_token.bucket_name, upload_token.object_name,
+                                                       upload_token.upload_id, metadata,
+                                                       json.dumps(upload_part_result))
+        except Exception as e:
+          self._fds.abort_multipart_upload(dst_bucket_name, dst_object_name, upload_token.upload_id)
+          CLIPrinter.fail(e.args)
     if result is not None:
       CLIPrinter.done('upload object %s/%s' % (dst_bucket_name, dst_object_name))
     else:
       CLIPrinter.fail('upload object %s/%s' % (dst_bucket_name, dst_object_name))
 
   def _upload_batch(self, d, dst_url, recursive, autodetect_mimetype, sync=False):
     for root, dirs, files in os.walk(d):
@@ -670,40 +680,14 @@
         continue
       for filename in files:
         object_name = os.path.join(root, filename)
         self._upload(object_name, dst_url, autodetect_mimetype, sync)
       if not recursive:
         break
 
-  def _upload_concurrency(self, bucket_name, object_name, stream, metadata):
-    upload_token = None
-    try:
-      upload_token = self._fds.init_multipart_upload(bucket_name, object_name)
-      part_number = 1
-      futures = []
-      result_list = []
-      with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
-        while True:
-          data = stream.read(multipart_upload_buffer_size)
-          if len(data) <= 0:
-            break
-          future = executor.submit(async_task, self._fds, upload_token, part_number, data)
-          futures.append(future)
-          part_number += 1
-
-      for f in concurrent.futures.as_completed(futures):
-        result_list.append(f.result())
-      upload_part_result = UploadPartResultList({"uploadPartResultList": result_list})
-      return self._fds.complete_multipart_upload(upload_token.bucket_name, upload_token.object_name,
-                                                 upload_token.upload_id, metadata,
-                                                 json.dumps(upload_part_result))
-    except Exception as e:
-      self._fds.abort_multipart_upload(bucket_name, object_name, upload_token.upload_id)
-      CLIPrinter.fail(e.args)
-
   def sync(self, src, dst, autodetect_mimetype=False):
     """
     sync command syncs between (local directory and fds) (fds and local directory) (fds and fds)
     :param src: src can be a fds bucket url like fds://bucketname or '.'
     :param dst: src can be a fds bucket url like fds://bucketname or '.'
     :param delete: todo delete target file if source file is deleted
     :param exclude: todo
```

### Comparing `galaxy-fds-sdk-1.4.8/galaxy_fds_sdk.egg-info/SOURCES.txt` & `galaxy-fds-sdk-1.4.9/galaxy_fds_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-fds-sdk-1.4.8/README.md` & `galaxy-fds-sdk-1.4.9/README.md`

 * *Files identical despite different names*


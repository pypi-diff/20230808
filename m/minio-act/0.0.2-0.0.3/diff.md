# Comparing `tmp/minio_act-0.0.2.tar.gz` & `tmp/minio_act-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minio_act-0.0.2.tar", last modified: Tue Aug  8 17:23:49 2023, max compression
+gzip compressed data, was "minio_act-0.0.3.tar", last modified: Tue Aug  8 17:28:21 2023, max compression
```

## Comparing `minio_act-0.0.2.tar` & `minio_act-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:23:49.107692 minio_act-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-08 17:23:49.107692 minio_act-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-08 17:23:46.000000 minio_act-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:23:49.103692 minio_act-0.0.2/minio_act/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 17:23:46.000000 minio_act-0.0.2/minio_act/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 17:23:46.000000 minio_act-0.0.2/minio_act/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-08 17:23:46.000000 minio_act-0.0.2/minio_act/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 17:23:46.000000 minio_act-0.0.2/minio_act/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:23:49.103692 minio_act-0.0.2/minio_act.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-08 17:23:49.000000 minio_act-0.0.2/minio_act.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 17:23:49.000000 minio_act-0.0.2/minio_act.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:23:49.000000 minio_act-0.0.2/minio_act.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 17:23:49.000000 minio_act-0.0.2/minio_act.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 17:23:49.000000 minio_act-0.0.2/minio_act.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:23:49.107692 minio_act-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-08 17:23:48.000000 minio_act-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:21.309888 minio_act-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-08 17:28:21.309888 minio_act-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-08 17:28:18.000000 minio_act-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:21.309888 minio_act-0.0.3/minio_act/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 17:28:18.000000 minio_act-0.0.3/minio_act/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 17:28:18.000000 minio_act-0.0.3/minio_act/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-08-08 17:28:18.000000 minio_act-0.0.3/minio_act/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-08 17:28:18.000000 minio_act-0.0.3/minio_act/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:21.309888 minio_act-0.0.3/minio_act.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-08 17:28:21.000000 minio_act-0.0.3/minio_act.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 17:28:21.000000 minio_act-0.0.3/minio_act.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:28:21.000000 minio_act-0.0.3/minio_act.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 17:28:21.000000 minio_act-0.0.3/minio_act.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 17:28:21.000000 minio_act-0.0.3/minio_act.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:28:21.309888 minio_act-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-08 17:28:20.000000 minio_act-0.0.3/setup.py
```

### Comparing `minio_act-0.0.2/PKG-INFO` & `minio_act-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minio_act
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for interact with Minio resource
 Home-page: https://github.com/trancongtuanmanh/minio-act
 Author: John Doe
 Author-email: manhtct.dev@gmail.com
 Keywords: pypi,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 ```
 
 ## Download source
 
 ```sh
 $ git clone https://github.com/trancongtuanmanh/minio-act
 $ cd minio-act
-python setup.py install
+$ python setup.py install
 ```
 
 ## Quick Start Example - File Uploader
 This example program connects to an S3-compatible object storage server, make a bucket on that server, and upload a file to the bucket.
 
 You need the following items to connect to an S3-compatible object storage server:
 
@@ -63,15 +63,15 @@
 )
 minio_src.create_bucket(
     bucket_name="minio-bk",
     region="ap-southeast-1"
 )
 ```
 
-#### Run File Uploader
+#### Run File Create Bucket
 ```sh
 $ python3 examples/bucket/create.py
 2023-08-09 00:07:41,848 - Minio Client - INFO - Creating bucket minio-bk ...
 ```
 
 ## More References
 * [Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)
```

### Comparing `minio_act-0.0.2/README.md` & `minio_act-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 
 ## Download source
 
 ```sh
 $ git clone https://github.com/trancongtuanmanh/minio-act
 $ cd minio-act
-python setup.py install
+$ python setup.py install
 ```
 
 ## Quick Start Example - File Uploader
 This example program connects to an S3-compatible object storage server, make a bucket on that server, and upload a file to the bucket.
 
 You need the following items to connect to an S3-compatible object storage server:
 
@@ -46,15 +46,15 @@
 )
 minio_src.create_bucket(
     bucket_name="minio-bk",
     region="ap-southeast-1"
 )
 ```
 
-#### Run File Uploader
+#### Run File Create Bucket
 ```sh
 $ python3 examples/bucket/create.py
 2023-08-09 00:07:41,848 - Minio Client - INFO - Creating bucket minio-bk ...
 ```
 
 ## More References
 * [Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)
```

### Comparing `minio_act-0.0.2/minio_act/client.py` & `minio_act-0.0.3/minio_act/client.py`

 * *Files identical despite different names*

### Comparing `minio_act-0.0.2/minio_act.egg-info/PKG-INFO` & `minio_act-0.0.3/minio_act.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minio-act
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package for interact with Minio resource
 Home-page: https://github.com/trancongtuanmanh/minio-act
 Author: John Doe
 Author-email: manhtct.dev@gmail.com
 Keywords: pypi,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 ```
 
 ## Download source
 
 ```sh
 $ git clone https://github.com/trancongtuanmanh/minio-act
 $ cd minio-act
-python setup.py install
+$ python setup.py install
 ```
 
 ## Quick Start Example - File Uploader
 This example program connects to an S3-compatible object storage server, make a bucket on that server, and upload a file to the bucket.
 
 You need the following items to connect to an S3-compatible object storage server:
 
@@ -63,15 +63,15 @@
 )
 minio_src.create_bucket(
     bucket_name="minio-bk",
     region="ap-southeast-1"
 )
 ```
 
-#### Run File Uploader
+#### Run File Create Bucket
 ```sh
 $ python3 examples/bucket/create.py
 2023-08-09 00:07:41,848 - Minio Client - INFO - Creating bucket minio-bk ...
 ```
 
 ## More References
 * [Python Client API Reference](https://min.io/docs/minio/linux/developers/python/API.html)
```

### Comparing `minio_act-0.0.2/setup.py` & `minio_act-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="minio_act",
-    version='0.0.2',
+    version='0.0.3',
     author="John Doe",
     author_email="manhtct.dev@gmail.com",
     description="Python package for interact with Minio resource",
     url = "https://github.com/trancongtuanmanh/minio-act",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```


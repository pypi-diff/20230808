# Comparing `tmp/gammarer.aws-secure-cloudfront-origin-bucket-0.7.0.tar.gz` & `tmp/gammarer.aws-secure-cloudfront-origin-bucket-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-0.7.0.tar", last modified: Tue Aug  8 07:47:39 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-cloudfront-origin-bucket-0.7.1.tar", last modified: Tue Aug  8 18:17:42 2023, max compression
```

## Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0.tar` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.505368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.505368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@0.7.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:47:25.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:47:39.509368 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 07:47:39.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 07:47:39.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:47:39.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 07:47:39.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:47:39.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.493729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.493729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29289 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@0.7.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:17:30.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:17:42.497729 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 18:17:42.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 18:17:42.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:17:42.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 18:17:42.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 18:17:42.000000 gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/LICENSE` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 0.7.0
+Version: 0.7.1
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/yicr/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/README.md` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/setup.py` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-cloudfront-origin-bucket",
-    "version": "0.7.0",
+    "version": "0.7.1",
     "description": "AWS CloudFront distribution origin S3 bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-cloudfront-origin-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_cloudfront_origin_bucket",
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_cloudfront_origin_bucket._jsii": [
-            "aws-secure-cloudfront-origin-bucket@0.7.0.jsii.tgz"
+            "aws-secure-cloudfront-origin-bucket@0.7.1.jsii.tgz"
         ],
         "gammarer.aws_secure_cloudfront_origin_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-cloudfront-origin-bucket
-Version: 0.7.0
+Version: 0.7.1
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/yicr/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-cloudfront-origin-bucket-0.7.0/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-cloudfront-origin-bucket-0.7.1/src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_cloudfront_origin_bucket/__init__.py
 src/gammarer/aws_secure_cloudfront_origin_bucket/py.typed
 src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@0.7.0.jsii.tgz
+src/gammarer/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@0.7.1.jsii.tgz
```


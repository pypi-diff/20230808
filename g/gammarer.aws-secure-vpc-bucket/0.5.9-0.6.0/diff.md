# Comparing `tmp/gammarer.aws-secure-vpc-bucket-0.5.9.tar.gz` & `tmp/gammarer.aws-secure-vpc-bucket-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-vpc-bucket-0.5.9.tar", last modified: Fri Jul 28 18:22:07 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-vpc-bucket-0.6.0.tar", last modified: Tue Aug  8 07:17:21 2023, max compression
```

## Comparing `gammarer.aws-secure-vpc-bucket-0.5.9.tar` & `gammarer.aws-secure-vpc-bucket-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.632548 gammarer.aws-secure-vpc-bucket-0.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.632548 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29583 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:21:53.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:22:07.636548 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-28 18:22:07.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 18:22:07.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:22:07.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-28 18:22:07.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:22:07.000000 gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.6.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:17:07.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:17:21.282953 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 07:17:21.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-08 07:17:21.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:17:21.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 07:17:21.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 07:17:21.000000 gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/LICENSE` & `gammarer.aws-secure-vpc-bucket-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/PKG-INFO` & `gammarer.aws-secure-vpc-bucket-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-vpc-bucket
-Version: 0.5.9
+Version: 0.6.0
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/yicr/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/README.md` & `gammarer.aws-secure-vpc-bucket-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/setup.py` & `gammarer.aws-secure-vpc-bucket-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-vpc-bucket",
-    "version": "0.5.9",
+    "version": "0.6.0",
     "description": "Access from specific VPC Endpoint only Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-vpc-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "gammarer.aws_secure_vpc_bucket",
         "gammarer.aws_secure_vpc_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_vpc_bucket._jsii": [
-            "aws-secure-vpc-bucket@0.5.9.jsii.tgz"
+            "aws-secure-vpc-bucket@0.6.0.jsii.tgz"
         ],
         "gammarer.aws_secure_vpc_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.65.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-bucket>=0.10.2, <0.11.0",
-        "jsii>=1.85.0, <2.0.0",
+        "gammarer.aws-secure-bucket>=0.11.3, <0.12.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer/aws_secure_vpc_bucket/__init__.py` & `gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer/aws_secure_vpc_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-vpc-bucket
-Version: 0.5.9
+Version: 0.6.0
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/yicr/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.9/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-vpc-bucket-0.6.0/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_vpc_bucket/__init__.py
 src/gammarer/aws_secure_vpc_bucket/py.typed
 src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.9.jsii.tgz
+src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.6.0.jsii.tgz
```


# Comparing `tmp/ez-constructs-0.0.24.tar.gz` & `tmp/ez-constructs-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-constructs-0.0.24.tar", last modified: Thu Jul 20 18:50:45 2023, max compression
+gzip compressed data, was "ez-constructs-0.0.25.tar", last modified: Tue Aug  8 10:55:46 2023, max compression
```

## Comparing `ez-constructs-0.0.24.tar` & `ez-constructs-0.0.25.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/src/ez_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)    48251 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/src/ez_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/src/ez_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/src/ez_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   489266 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/src/ez_constructs/_jsii/ez-constructs@0.0.24.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:50:29.000000 ez-constructs-0.0.24/src/ez_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:50:45.956843 ez-constructs-0.0.24/src/ez_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 18:50:45.000000 ez-constructs-0.0.24/src/ez_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 18:50:45.000000 ez-constructs-0.0.24/src/ez_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:50:45.000000 ez-constructs-0.0.24/src/ez_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 18:50:45.000000 ez-constructs-0.0.24/src/ez_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 18:50:45.000000 ez-constructs-0.0.24/src/ez_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/src/ez_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)    48203 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/src/ez_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/src/ez_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/src/ez_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   489179 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/src/ez_constructs/_jsii/ez-constructs@0.0.25.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:55:33.000000 ez-constructs-0.0.25/src/ez_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 10:55:46.309300 ez-constructs-0.0.25/src/ez_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-08 10:55:45.000000 ez-constructs-0.0.25/src/ez_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 10:55:46.000000 ez-constructs-0.0.25/src/ez_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 10:55:45.000000 ez-constructs-0.0.25/src/ez_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-08 10:55:46.000000 ez-constructs-0.0.25/src/ez_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 10:55:46.000000 ez-constructs-0.0.25/src/ez_constructs.egg-info/top_level.txt
```

### Comparing `ez-constructs-0.0.24/LICENSE` & `ez-constructs-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-constructs-0.0.24/PKG-INFO` & `ez-constructs-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-constructs
-Version: 0.0.24
+Version: 0.0.25
 Summary: ez-constructs
 Home-page: https://github.com/SavvyTools/ez-constructs.git
 Author: Biju Joseph<biju.joseph@semanticbits.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SavvyTools/ez-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `ez-constructs-0.0.24/README.md` & `ez-constructs-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `ez-constructs-0.0.24/setup.py` & `ez-constructs-0.0.25/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ez-constructs",
-    "version": "0.0.24",
+    "version": "0.0.25",
     "description": "ez-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/SavvyTools/ez-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Biju Joseph<biju.joseph@semanticbits.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "ez_constructs",
         "ez_constructs._jsii"
     ],
     "package_data": {
         "ez_constructs._jsii": [
-            "ez-constructs@0.0.24.jsii.tgz"
+            "ez-constructs@0.0.25.jsii.tgz"
         ],
         "ez_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ez-constructs-0.0.24/src/ez_constructs/__init__.py` & `ez-constructs-0.0.25/src/ez_constructs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 
 
 @jsii.enum(jsii_type="ez-constructs.GitEvent")
 class GitEvent(enum.Enum):
     '''The Github events which should trigger this build.'''
 
     PULL_REQUEST = "PULL_REQUEST"
-    PULL_REQUEST_MERGED = "PULL_REQUEST_MERGED"
     PUSH = "PUSH"
     ALL = "ALL"
 
 
 @jsii.implements(aws_cdk.IAspect)
 class PermissionsBoundaryAspect(
     metaclass=jsii.JSIIMeta,
```

### Comparing `ez-constructs-0.0.24/src/ez_constructs.egg-info/PKG-INFO` & `ez-constructs-0.0.25/src/ez_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-constructs
-Version: 0.0.24
+Version: 0.0.25
 Summary: ez-constructs
 Home-page: https://github.com/SavvyTools/ez-constructs.git
 Author: Biju Joseph<biju.joseph@semanticbits.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/SavvyTools/ez-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```


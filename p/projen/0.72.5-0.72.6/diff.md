# Comparing `tmp/projen-0.72.5.tar.gz` & `tmp/projen-0.72.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.72.5.tar", last modified: Mon Aug  7 12:37:32 2023, max compression
+gzip compressed data, was "projen-0.72.6.tar", last modified: Tue Aug  8 12:36:36 2023, max compression
```

## Comparing `projen-0.72.5.tar` & `projen-0.72.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.087376 projen-0.72.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-07 12:37:19.000000 projen-0.72.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-07 12:37:19.000000 projen-0.72.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-07 12:37:32.087376 projen-0.72.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-08-07 12:37:19.000000 projen-0.72.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-07 12:37:19.000000 projen-0.72.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 12:37:32.087376 projen-0.72.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-07 12:37:19.000000 projen-0.72.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.071375 projen-0.72.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.075376 projen-0.72.5/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   601934 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.075376 projen-0.72.5/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  2754130 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/_jsii/projen@0.72.5.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1040675 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    40847 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   480911 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   575465 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   213323 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.079376 projen-0.72.5/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   291142 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   607210 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   248786 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   430274 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.083376 projen-0.72.5/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   756498 2023-08-07 12:37:19.000000 projen-0.72.5/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 12:37:32.075376 projen-0.72.5/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-07 12:37:32.000000 projen-0.72.5/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-07 12:37:32.000000 projen-0.72.5/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 12:37:32.000000 projen-0.72.5/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-07 12:37:32.000000 projen-0.72.5/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 12:37:32.000000 projen-0.72.5/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.459621 projen-0.72.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-08 12:36:24.000000 projen-0.72.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:36:24.000000 projen-0.72.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-08 12:36:36.455620 projen-0.72.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-08-08 12:36:24.000000 projen-0.72.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 12:36:24.000000 projen-0.72.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:36:36.459621 projen-0.72.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-08 12:36:24.000000 projen-0.72.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.443620 projen-0.72.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.447620 projen-0.72.6/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   601934 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.447620 projen-0.72.6/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  2754135 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/_jsii/projen@0.72.6.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1040675 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    40847 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   480911 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   575465 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   213323 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   291142 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.451620 projen-0.72.6/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   607210 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   248786 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   430274 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.455620 projen-0.72.6/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   756498 2023-08-08 12:36:24.000000 projen-0.72.6/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:36:36.447620 projen-0.72.6/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-08-08 12:36:36.000000 projen-0.72.6/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 12:36:36.000000 projen-0.72.6/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:36:36.000000 projen-0.72.6/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-08 12:36:36.000000 projen-0.72.6/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 12:36:36.000000 projen-0.72.6/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.72.5/LICENSE` & `projen-0.72.6/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/PKG-INFO` & `projen-0.72.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.72.5
+Version: 0.72.6
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.72.5/README.md` & `projen-0.72.6/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/setup.py` & `projen-0.72.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.72.5",
+    "version": "0.72.6",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.72.5.jsii.tgz"
+            "projen@0.72.6.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.72.5/src/projen/__init__.py` & `projen-0.72.6/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/awscdk/__init__.py` & `projen-0.72.6/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/build/__init__.py` & `projen-0.72.6/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/cdk/__init__.py` & `projen-0.72.6/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/cdk8s/__init__.py` & `projen-0.72.6/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/cdktf/__init__.py` & `projen-0.72.6/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/circleci/__init__.py` & `projen-0.72.6/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/github/__init__.py` & `projen-0.72.6/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/github/workflows/__init__.py` & `projen-0.72.6/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/gitlab/__init__.py` & `projen-0.72.6/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/java/__init__.py` & `projen-0.72.6/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/javascript/__init__.py` & `projen-0.72.6/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/python/__init__.py` & `projen-0.72.6/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/release/__init__.py` & `projen-0.72.6/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/typescript/__init__.py` & `projen-0.72.6/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/vscode/__init__.py` & `projen-0.72.6/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen/web/__init__.py` & `projen-0.72.6/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.72.5/src/projen.egg-info/PKG-INFO` & `projen-0.72.6/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.72.5
+Version: 0.72.6
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.72.5/src/projen.egg-info/SOURCES.txt` & `projen-0.72.6/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.72.5.jsii.tgz
+src/projen/_jsii/projen@0.72.6.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```


# Comparing `tmp/localstack-2.2.1.dev20230805180111.tar.gz` & `tmp/localstack-2.2.1.dev20230808110233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.2.1.dev20230805180111.tar", last modified: Sat Aug  5 18:04:16 2023, max compression
+gzip compressed data, was "localstack-2.2.1.dev20230808110233.tar", last modified: Tue Aug  8 11:05:56 2023, max compression
```

## Comparing `localstack-2.2.1.dev20230805180111.tar` & `localstack-2.2.1.dev20230808110233.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/
--rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-08-05 18:04:15.000000 localstack-2.2.1.dev20230805180111/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-08-05 18:00:56.000000 localstack-2.2.1.dev20230805180111/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-08 11:05:56.981598 localstack-2.2.1.dev20230808110233/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-08 11:05:56.981598 localstack-2.2.1.dev20230808110233/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-08 11:05:56.977598 localstack-2.2.1.dev20230808110233/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-08 11:05:56.981598 localstack-2.2.1.dev20230808110233/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-08-08 11:05:56.000000 localstack-2.2.1.dev20230808110233/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-08-08 11:05:56.981598 localstack-2.2.1.dev20230808110233/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-08-08 11:02:18.000000 localstack-2.2.1.dev20230808110233/setup.py
```

### Comparing `localstack-2.2.1.dev20230805180111/PKG-INFO` & `localstack-2.2.1.dev20230808110233/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.2.1.dev20230805180111
+Version: 2.2.1.dev20230808110233
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230805180111
+Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230808110233
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
```

### Comparing `localstack-2.2.1.dev20230805180111/localstack.egg-info/PKG-INFO` & `localstack-2.2.1.dev20230808110233/localstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.2.1.dev20230805180111
+Version: 2.2.1.dev20230808110233
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230805180111
+Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230808110233
 Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
 github.com/localstack/localstack Author: LocalStack Contributors Author-email:
 info@localstack.cloud License: Apache License 2.0 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Topic :: Internet Classifier: Topic :: Software
 Development :: Testing Classifier: Topic :: System :: Emulators Description-
 Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
```

### Comparing `localstack-2.2.1.dev20230805180111/setup.py` & `localstack-2.2.1.dev20230808110233/setup.py`

 * *Files identical despite different names*


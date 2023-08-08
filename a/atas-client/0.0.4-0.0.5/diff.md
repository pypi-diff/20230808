# Comparing `tmp/atas_client-0.0.4.tar.gz` & `tmp/atas_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atas_client-0.0.4.tar", last modified: Thu May 11 06:29:36 2023, max compression
+gzip compressed data, was "atas_client-0.0.5.tar", last modified: Tue Aug  8 09:19:36 2023, max compression
```

## Comparing `atas_client-0.0.4.tar` & `atas_client-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.888454 atas_client-0.0.4/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.0.4/LICENSE
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-05-11 06:29:36.888331 atas_client-0.0.4/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.0.4/README.md
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2023-05-11 06:13:09.000000 atas_client-0.0.4/pyproject.toml
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2023-05-11 06:29:36.888499 atas_client-0.0.4/setup.cfg
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.886418 atas_client-0.0.4/src/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.0.4/src/__init__.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.887433 atas_client-0.0.4/src/atas_client/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2274 2022-12-08 01:19:04.000000 atas_client-0.0.4/src/atas_client/CoreATASApi.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1357 2023-05-11 06:11:15.000000 atas_client-0.0.4/src/atas_client/HttpUtil.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.0.4/src/atas_client/__init__.py
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      960 2022-12-08 01:19:04.000000 atas_client-0.0.4/src/atas_client/atas_client.py
-drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-05-11 06:29:36.888167 atas_client-0.0.4/src/atas_client.egg-info/
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/PKG-INFO
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/SOURCES.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/dependency_links.txt
--rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2023-05-11 06:29:36.000000 atas_client-0.0.4/src/atas_client.egg-info/top_level.txt
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-08-08 09:19:36.454863 atas_client-0.0.5/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1073 2022-12-05 06:04:48.000000 atas_client-0.0.5/LICENSE
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-08-08 09:19:36.454735 atas_client-0.0.5/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       23 2022-12-05 06:50:55.000000 atas_client-0.0.5/README.md
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      551 2023-08-08 09:19:12.000000 atas_client-0.0.5/pyproject.toml
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       38 2023-08-08 09:19:36.454902 atas_client-0.0.5/setup.cfg
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-08-08 09:19:36.452601 atas_client-0.0.5/src/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:17.000000 atas_client-0.0.5/src/__init__.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-08-08 09:19:36.453789 atas_client-0.0.5/src/atas_client/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     2274 2022-12-08 01:19:04.000000 atas_client-0.0.5/src/atas_client/CoreATASApi.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1357 2023-05-11 06:11:15.000000 atas_client-0.0.5/src/atas_client/HttpUtil.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2022-12-08 00:45:10.000000 atas_client-0.0.5/src/atas_client/__init__.py
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1028 2023-08-08 09:17:53.000000 atas_client-0.0.5/src/atas_client/atas_client.py
+drwxr-xr-x   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        0 2023-08-08 09:19:36.454563 atas_client-0.0.5/src/atas_client.egg-info/
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)     1702 2023-08-08 09:19:36.000000 atas_client-0.0.5/src/atas_client.egg-info/PKG-INFO
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)      322 2023-08-08 09:19:36.000000 atas_client-0.0.5/src/atas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)        1 2023-08-08 09:19:36.000000 atas_client-0.0.5/src/atas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tao.ding (1879105732) INTRA\Domain Users (679754705)       21 2023-08-08 09:19:36.000000 atas_client-0.0.5/src/atas_client.egg-info/top_level.txt
```

### Comparing `atas_client-0.0.4/LICENSE` & `atas_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.4/PKG-INFO` & `atas_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas_client
-Version: 0.0.4
+Version: 0.0.5
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `atas_client-0.0.4/pyproject.toml` & `atas_client-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atas_client"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="tao.ding", email="tao.ding@rakuten.com" },
 ]
 description = "ATAS Automation API"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `atas_client-0.0.4/src/atas_client/CoreATASApi.py` & `atas_client-0.0.5/src/atas_client/CoreATASApi.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.4/src/atas_client/HttpUtil.py` & `atas_client-0.0.5/src/atas_client/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `atas_client-0.0.4/src/atas_client/atas_client.py` & `atas_client-0.0.5/src/atas_client/atas_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 
 def init(endpoints, token, launch_name, executor):
     return CoreATASApi.init_result(endpoints, token, launch_name, executor)
 
 
 def upload_result(endpoints, token, execution_id, case_name, step_desc, step_status, case_status, executor, path,
                   screenshot,
-                  attachment, start_time, end_time):
+                  attachment, start_time, end_time, test_plan_case_id):
     data = {'caseName': case_name,
             'path': path,
             'stepStatus': step_status,
             'stepDescription': step_desc,
             'caseStatus': case_status,
             'executor': executor,
             'screen_path': screenshot,
             'attachment_path': attachment,
             'executionId': execution_id,
             'startTime': start_time,
-            'endTime': end_time}
+            'endTime': end_time,
+            'testPlanCaseId': test_plan_case_id}
     CoreATASApi.save_result(endpoints, token, data)
 
 
 def complete(endpoints, token, execution_id, case_status):
     CoreATASApi.run_complete(endpoints, token, execution_id, case_status)
```

### Comparing `atas_client-0.0.4/src/atas_client.egg-info/PKG-INFO` & `atas_client-0.0.5/src/atas_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atas-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: ATAS Automation API
 Author-email: "tao.ding" <tao.ding@rakuten.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```


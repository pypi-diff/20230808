# Comparing `tmp/leetquery-0.1.0.tar.gz` & `tmp/leetquery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leetquery-0.1.0.tar", last modified: Mon Aug  7 04:52:11 2023, max compression
+gzip compressed data, was "leetquery-0.1.5.tar", last modified: Mon Aug  7 14:31:24 2023, max compression
```

## Comparing `leetquery-0.1.0.tar` & `leetquery-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:52:11.259110 leetquery-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 04:52:00.000000 leetquery-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 04:52:11.259110 leetquery-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-07 04:52:00.000000 leetquery-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:52:11.259110 leetquery-0.1.0/leetquery/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 04:52:00.000000 leetquery-0.1.0/leetquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-07 04:52:00.000000 leetquery-0.1.0/leetquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-07 04:52:00.000000 leetquery-0.1.0/leetquery/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:52:11.259110 leetquery-0.1.0/leetquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-07 04:52:11.000000 leetquery-0.1.0/leetquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 04:52:11.000000 leetquery-0.1.0/leetquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 04:52:11.000000 leetquery-0.1.0/leetquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 04:52:11.000000 leetquery-0.1.0/leetquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 04:52:11.000000 leetquery-0.1.0/leetquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 04:52:11.259110 leetquery-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-07 04:52:00.000000 leetquery-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 04:52:11.259110 leetquery-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-07 04:52:00.000000 leetquery-0.1.0/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-07 14:31:13.000000 leetquery-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 14:31:24.568527 leetquery-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-07 14:31:13.000000 leetquery-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/leetquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-07 14:31:13.000000 leetquery-0.1.5/leetquery/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/leetquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 14:31:24.000000 leetquery-0.1.5/leetquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:31:24.568527 leetquery-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-07 14:31:13.000000 leetquery-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:31:24.568527 leetquery-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-07 14:31:13.000000 leetquery-0.1.5/tests/test_user.py
```

### Comparing `leetquery-0.1.0/LICENSE` & `leetquery-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `leetquery-0.1.0/PKG-INFO` & `leetquery-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetquery
-Version: 0.1.0
+Version: 0.1.5
 Summary: Query and analyze data from leetcode
 Home-page: https://github.com/ShuYuHuang/leetcode-query
 Author: Shu-Yu Huang
 Author-email: b123767195@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,22 +12,24 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 
 # Leetcode Query
-A library for retriving informations from Leetcode
-
-## Install 🚧
+A library for retriving Human Resource information from Leetcode.
 
+## Install
+``` shell
+    pip install leetquery
+```
 ## Usage
 ### Retriving User Submissions
 ``` python
-from leetquery.user import get_submissions
+from leetquery import get_submissions
 
 submissions = get_submissions(username="syhaung", limits)
 ```
 return value:
 ```
 ["question1", "question2", ...]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `leetquery-0.1.0/leetquery/user.py` & `leetquery-0.1.5/leetquery/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-# Copyright (c) 2023 Shu-Yu Huang
-#
-# Licensed under the MIT License
-import requests
+"""
+Copyright (c) 2023 Shu-Yu Huang
+
+Licensed under the MIT License
+"""
 import json
 from typing import List
+import requests
 
 __all__  = ["get_submissions"]
 
 def get_submissions(username: str="syhaung", limit: int= 12) -> List[str]:
+    """
+        Gwt
+    """
     url = "https://leetcode.com/graphql?"
     headers = {'Content-Type': 'application/json'}
     query = """
     query recentAcSubmissions($username: String!, $limit: Int!) {
         recentAcSubmissionList(username: $username, limit: $limit) {
             id
             title
             titleSlug
             timestamp
         }
     }
     """
-    variables = {'username': username, 'limit': 50}
+    variables = {'username': username, 'limit': limit}
     payload = {
             'query': query,
             'operationName': 'recentAcSubmissions',
             'variables': variables
     }
 
-    response = requests.post(url, headers=headers, data=json.dumps(payload)).json()
+    response = requests.post(
+        url,
+        headers=headers,
+        data=json.dumps(payload),
+        timeout=1.5
+    ).json()
     return [x["title"] for x in response["data"]["recentAcSubmissionList"]]
```

### Comparing `leetquery-0.1.0/leetquery.egg-info/PKG-INFO` & `leetquery-0.1.5/leetquery.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leetquery
-Version: 0.1.0
+Version: 0.1.5
 Summary: Query and analyze data from leetcode
 Home-page: https://github.com/ShuYuHuang/leetcode-query
 Author: Shu-Yu Huang
 Author-email: b123767195@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,22 +12,24 @@
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 
 # Leetcode Query
-A library for retriving informations from Leetcode
-
-## Install 🚧
+A library for retriving Human Resource information from Leetcode.
 
+## Install
+``` shell
+    pip install leetquery
+```
 ## Usage
 ### Retriving User Submissions
 ``` python
-from leetquery.user import get_submissions
+from leetquery import get_submissions
 
 submissions = get_submissions(username="syhaung", limits)
 ```
 return value:
 ```
 ["question1", "question2", ...]
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `leetquery-0.1.0/setup.py` & `leetquery-0.1.5/setup.py`

 * *Files identical despite different names*


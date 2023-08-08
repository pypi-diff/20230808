# Comparing `tmp/webrequests-1.0.5.tar.gz` & `tmp/webrequests-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webrequests-1.0.5.tar", last modified: Thu Dec  1 03:49:30 2022, max compression
+gzip compressed data, was "webrequests-1.0.6.tar", last modified: Tue Aug  8 03:37:06 2023, max compression
```

## Comparing `webrequests-1.0.5.tar` & `webrequests-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2022-12-01 03:49:30.290140 webrequests-1.0.5/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       58 2022-12-01 02:20:09.000000 webrequests-1.0.5/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2033 2022-12-01 03:49:30.283263 webrequests-1.0.5/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      986 2022-12-01 03:47:00.000000 webrequests-1.0.5/README.md
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       32 2022-12-01 02:38:41.000000 webrequests-1.0.5/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2022-12-01 03:49:30.299508 webrequests-1.0.5/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1150 2022-12-01 03:36:22.000000 webrequests-1.0.5/setup.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2022-12-01 03:49:30.146949 webrequests-1.0.5/webrequests/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      219 2022-12-01 03:44:23.000000 webrequests-1.0.5/webrequests/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     4516 2022-12-01 03:43:07.000000 webrequests-1.0.5/webrequests/core.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      652 2022-12-01 02:48:00.000000 webrequests-1.0.5/webrequests/util.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      250 2022-12-01 03:02:06.000000 webrequests-1.0.5/webrequests/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2022-12-01 03:49:30.258142 webrequests-1.0.5/webrequests.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2033 2022-12-01 03:49:29.000000 webrequests-1.0.5/webrequests.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      310 2022-12-01 03:49:29.000000 webrequests-1.0.5/webrequests.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2022-12-01 03:49:29.000000 webrequests-1.0.5/webrequests.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       33 2022-12-01 03:49:29.000000 webrequests-1.0.5/webrequests.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       12 2022-12-01 03:49:29.000000 webrequests-1.0.5/webrequests.egg-info/top_level.txt
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-08-08 03:37:06.288467 webrequests-1.0.6/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       58 2022-12-01 02:20:09.000000 webrequests-1.0.6/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2033 2023-08-08 03:37:06.281350 webrequests-1.0.6/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      986 2022-12-01 03:47:00.000000 webrequests-1.0.6/README.md
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       32 2022-12-01 02:38:41.000000 webrequests-1.0.6/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-08-08 03:37:06.293707 webrequests-1.0.6/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1150 2022-12-01 03:36:22.000000 webrequests-1.0.6/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-08-08 03:37:06.160400 webrequests-1.0.6/webrequests/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      219 2022-12-01 03:44:23.000000 webrequests-1.0.6/webrequests/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     4586 2023-08-08 03:36:12.000000 webrequests-1.0.6/webrequests/core.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      652 2022-12-01 02:48:00.000000 webrequests-1.0.6/webrequests/util.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      250 2023-08-08 03:36:45.000000 webrequests-1.0.6/webrequests/version.json
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-08-08 03:37:06.260733 webrequests-1.0.6/webrequests.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2033 2023-08-08 03:37:05.000000 webrequests-1.0.6/webrequests.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      310 2023-08-08 03:37:05.000000 webrequests-1.0.6/webrequests.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-08-08 03:37:05.000000 webrequests-1.0.6/webrequests.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       33 2023-08-08 03:37:05.000000 webrequests-1.0.6/webrequests.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       12 2023-08-08 03:37:05.000000 webrequests-1.0.6/webrequests.egg-info/top_level.txt
```

### Comparing `webrequests-1.0.5/PKG-INFO` & `webrequests-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webrequests
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple wrapper of requests, simple but useful!
 Home-page: https://github.com/suqingdong/webrequests
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: BSD License
 Description: # A simple wrapper of requests, simple but useful!
```

### Comparing `webrequests-1.0.5/README.md` & `webrequests-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `webrequests-1.0.5/setup.py` & `webrequests-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `webrequests-1.0.5/webrequests/core.py` & `webrequests-1.0.6/webrequests/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             'Mozilla/5.0 (Windows NT 5.1; U; en; rv:1.8.1) Gecko/20061208 Firefox/2.0.0 Opera 9.50',
             'Mozilla/5.0 (Windows NT 6.1; WOW64; rv:34.0) Gecko/20100101 Firefox/34.0',
         ]
         return {'User-Agent': random.choice(ua_list)}
 
 
     @classmethod
-    def get_response(cls, url, method='GET', session=None, max_try=10, allowed_codes=[200], **kwargs):
+    def get_response(cls, url, method='GET', session=None, max_try=10, allowed_codes=[200], encoding='utf-8', **kwargs):
         """
             params
                 - allowed_codes: the allowed status_code
 
             Return a response object
         """
         if 'headers' not in kwargs:
@@ -67,14 +67,15 @@
         elif 'User-Agent' not in kwargs['headers']:
             kwargs['headers'].update(cls.random_ua())
 
         for n in range(max_try):
             try:
                 r = session or requests
                 resp = r.request(method, url, **kwargs)
+                resp.encoding = encoding or 'utf-8'
                 if resp.status_code in allowed_codes:
                     return resp
                 cls.logger.warning('{}st time bad status code: {} [{}]'.format(n + 1, resp.status_code, resp.text))
             except Exception as e:
                 cls.logger.debug('{}st time failed for url: {}, as {}'.format(n + 1, url, e))
             time.sleep(random.randint(2, 6))
```

### Comparing `webrequests-1.0.5/webrequests/util.py` & `webrequests-1.0.6/webrequests/util.py`

 * *Files identical despite different names*

### Comparing `webrequests-1.0.5/webrequests.egg-info/PKG-INFO` & `webrequests-1.0.6/webrequests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webrequests
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple wrapper of requests, simple but useful!
 Home-page: https://github.com/suqingdong/webrequests
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: BSD License
 Description: # A simple wrapper of requests, simple but useful!
```


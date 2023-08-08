# Comparing `tmp/userinput-1.0.8.tar.gz` & `tmp/userinput-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/userinput-1.0.8.tar", last modified: Sat Aug 10 07:59:33 2019, max compression
+gzip compressed data, was "dist/userinput-1.0.9.tar", last modified: Sun Aug 11 10:37:50 2019, max compression
```

## Comparing `userinput-1.0.8.tar` & `userinput-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-10 07:59:33.000000 userinput-1.0.8/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2019-06-05 18:29:19.000000 userinput-1.0.8/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3789 2019-08-10 07:59:33.000000 userinput-1.0.8/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2856 2019-06-05 18:56:59.000000 userinput-1.0.8/README.rst
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2019-08-10 07:59:33.000000 userinput-1.0.8/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1809 2019-06-20 11:06:52.000000 userinput-1.0.8/setup.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      147 2019-07-31 10:07:47.000000 userinput-1.0.8/userinput/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       64 2019-08-10 07:59:25.000000 userinput-1.0.8/userinput/__version__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3918 2019-08-10 07:58:11.000000 userinput-1.0.8/userinput/userinput.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput/utils/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      315 2019-07-31 10:07:30.000000 userinput-1.0.8/userinput/utils/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      159 2019-06-16 14:25:51.000000 userinput-1.0.8/userinput/utils/clear.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      861 2019-06-16 13:29:43.000000 userinput-1.0.8/userinput/utils/closest.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       86 2019-06-16 16:49:09.000000 userinput-1.0.8/userinput/utils/default_sanitizers.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      942 2019-08-10 07:44:59.000000 userinput-1.0.8/userinput/utils/default_validators.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      456 2019-06-16 14:06:00.000000 userinput-1.0.8/userinput/utils/set_validator.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      607 2019-07-31 10:06:05.000000 userinput-1.0.8/userinput/utils/start.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3789 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      479 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      134 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       10 2019-08-10 07:59:33.000000 userinput-1.0.8/userinput.egg-info/top_level.txt
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-11 10:37:50.000000 userinput-1.0.9/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2019-06-05 18:29:19.000000 userinput-1.0.9/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3789 2019-08-11 10:37:50.000000 userinput-1.0.9/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2856 2019-06-05 18:56:59.000000 userinput-1.0.9/README.rst
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2019-08-11 10:37:50.000000 userinput-1.0.9/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1809 2019-06-20 11:06:52.000000 userinput-1.0.9/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-11 10:37:50.000000 userinput-1.0.9/userinput/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      147 2019-07-31 10:07:47.000000 userinput-1.0.9/userinput/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       64 2019-08-11 10:37:44.000000 userinput-1.0.9/userinput/__version__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3918 2019-08-10 07:58:11.000000 userinput-1.0.9/userinput/userinput.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-11 10:37:50.000000 userinput-1.0.9/userinput/utils/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      315 2019-07-31 10:07:30.000000 userinput-1.0.9/userinput/utils/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      159 2019-06-16 14:25:51.000000 userinput-1.0.9/userinput/utils/clear.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      861 2019-06-16 13:29:43.000000 userinput-1.0.9/userinput/utils/closest.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       86 2019-06-16 16:49:09.000000 userinput-1.0.9/userinput/utils/default_sanitizers.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      979 2019-08-10 10:15:45.000000 userinput-1.0.9/userinput/utils/default_validators.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      456 2019-06-16 14:06:00.000000 userinput-1.0.9/userinput/utils/set_validator.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      607 2019-07-31 10:06:05.000000 userinput-1.0.9/userinput/utils/start.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2019-08-11 10:37:50.000000 userinput-1.0.9/userinput.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3789 2019-08-11 10:37:49.000000 userinput-1.0.9/userinput.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      479 2019-08-11 10:37:50.000000 userinput-1.0.9/userinput.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2019-08-11 10:37:49.000000 userinput-1.0.9/userinput.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      134 2019-08-11 10:37:49.000000 userinput-1.0.9/userinput.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       10 2019-08-11 10:37:49.000000 userinput-1.0.9/userinput.egg-info/top_level.txt
```

### Comparing `userinput-1.0.8/PKG-INFO` & `userinput-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userinput
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple python package to handle cli user input.
 Home-page: https://github.com/LucaCappelletti94/userinput
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: userinput
         =========================================================================================
```

### Comparing `userinput-1.0.8/README.rst` & `userinput-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `userinput-1.0.8/setup.py` & `userinput-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `userinput-1.0.8/userinput/userinput.py` & `userinput-1.0.9/userinput/userinput.py`

 * *Files identical despite different names*

### Comparing `userinput-1.0.8/userinput/utils/closest.py` & `userinput-1.0.9/userinput/utils/closest.py`

 * *Files identical despite different names*

### Comparing `userinput-1.0.8/userinput/utils/default_validators.py` & `userinput-1.0.9/userinput/utils/default_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     try:
         socket.gethostbyaddr(address)
         return True
     except socket.error:
         return False
 
 default_validators = {
-    "email":validate_email,
+    "email": lambda x: isinstance(x, str) and validate_email(x),
     "version_code":validate_version_code,
     "human_bool": set_validator(["yes", "y", "true", "no", "n", "false"]),
     "url":url,
     "integer":lambda x: str(x).isdigit(),
     "positive_integer":lambda x: str(x).isdigit() and int(x)>=0,
     "non_empty":lambda x: isinstance(x, str) and len(x)>0,
     "hostname":hostname,
```

### Comparing `userinput-1.0.8/userinput/utils/start.py` & `userinput-1.0.9/userinput/utils/start.py`

 * *Files identical despite different names*

### Comparing `userinput-1.0.8/userinput.egg-info/PKG-INFO` & `userinput-1.0.9/userinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userinput
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple python package to handle cli user input.
 Home-page: https://github.com/LucaCappelletti94/userinput
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: userinput
         =========================================================================================
```


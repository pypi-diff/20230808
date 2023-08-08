# Comparing `tmp/speedruncompy-0.0.1.tar.gz` & `tmp/speedruncompy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedruncompy-0.0.1.tar", last modified: Mon Aug  7 17:01:21 2023, max compression
+gzip compressed data, was "speedruncompy-0.0.2.tar", last modified: Tue Aug  8 20:19:23 2023, max compression
```

## Comparing `speedruncompy-0.0.1.tar` & `speedruncompy-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 17:01:21.171416 speedruncompy-0.0.1/
--rw-rw-rw-   0        0        0     1753 2023-08-07 17:01:21.170915 speedruncompy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1168 2023-08-06 20:04:01.000000 speedruncompy-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-07 17:01:21.171416 speedruncompy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-08-06 20:17:07.000000 speedruncompy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:01:21.159414 speedruncompy-0.0.1/speedruncompy/
--rw-rw-rw-   0        0        0       85 2023-08-06 20:03:50.000000 speedruncompy-0.0.1/speedruncompy/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-08-06 18:57:24.000000 speedruncompy-0.0.1/speedruncompy/api.py
--rw-rw-rw-   0        0        0     1668 2023-08-06 20:06:01.000000 speedruncompy-0.0.1/speedruncompy/auth.py
--rw-rw-rw-   0        0        0     1640 2023-07-25 23:57:13.000000 speedruncompy-0.0.1/speedruncompy/data_structures.py
--rw-rw-rw-   0        0        0     6754 2023-08-06 20:04:38.000000 speedruncompy-0.0.1/speedruncompy/endpoints.py
--rw-rw-rw-   0        0        0      523 2023-08-02 20:55:14.000000 speedruncompy-0.0.1/speedruncompy/enums.py
--rw-rw-rw-   0        0        0      222 2023-07-25 10:49:33.000000 speedruncompy-0.0.1/speedruncompy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-08-07 17:01:21.169915 speedruncompy-0.0.1/speedruncompy.egg-info/
--rw-rw-rw-   0        0        0     1753 2023-08-07 17:01:21.000000 speedruncompy-0.0.1/speedruncompy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-08-07 17:01:21.000000 speedruncompy-0.0.1/speedruncompy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 17:01:21.000000 speedruncompy-0.0.1/speedruncompy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-07 17:01:21.000000 speedruncompy-0.0.1/speedruncompy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-07 17:01:21.000000 speedruncompy-0.0.1/speedruncompy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 20:19:23.011218 speedruncompy-0.0.2/
+-rw-rw-rw-   0        0        0     1943 2023-08-08 20:19:23.010717 speedruncompy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1358 2023-08-08 19:35:01.000000 speedruncompy-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 20:19:23.011218 speedruncompy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-08-08 20:18:25.000000 speedruncompy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:19:22.998715 speedruncompy-0.0.2/speedruncompy/
+-rw-rw-rw-   0        0        0       85 2023-08-06 20:03:50.000000 speedruncompy-0.0.2/speedruncompy/__init__.py
+-rw-rw-rw-   0        0        0     3898 2023-08-08 19:13:50.000000 speedruncompy-0.0.2/speedruncompy/api.py
+-rw-rw-rw-   0        0        0     1637 2023-08-08 19:33:43.000000 speedruncompy-0.0.2/speedruncompy/auth.py
+-rw-rw-rw-   0        0        0     1943 2023-08-08 19:45:22.000000 speedruncompy-0.0.2/speedruncompy/data_structures.py
+-rw-rw-rw-   0        0        0     6754 2023-08-06 20:04:38.000000 speedruncompy-0.0.2/speedruncompy/endpoints.py
+-rw-rw-rw-   0        0        0      523 2023-08-02 20:55:14.000000 speedruncompy-0.0.2/speedruncompy/enums.py
+-rw-rw-rw-   0        0        0     1290 2023-08-08 15:39:25.000000 speedruncompy-0.0.2/speedruncompy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:19:23.009717 speedruncompy-0.0.2/speedruncompy.egg-info/
+-rw-rw-rw-   0        0        0     1943 2023-08-08 20:19:22.000000 speedruncompy-0.0.2/speedruncompy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-08-08 20:19:22.000000 speedruncompy-0.0.2/speedruncompy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 20:19:22.000000 speedruncompy-0.0.2/speedruncompy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 20:19:22.000000 speedruncompy-0.0.2/speedruncompy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-08 20:19:22.000000 speedruncompy-0.0.2/speedruncompy.egg-info/top_level.txt
```

### Comparing `speedruncompy-0.0.1/setup.py` & `speedruncompy-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as f:
     desc = f.read()
 
 setup(
     name='speedruncompy',
-    version="0.0.1",
+    version="0.0.2",
     author="Jamie",
     author_email="jamiebloomfield8@gmail.com",
     description="A wrapper for speedrun.com's new v2 API, as used by their new site",
     long_description=desc,
     long_description_content_type="text/markdown",
     url="https://github.com/ManicJamie/speedruncompy",
     project_urls={
```

### Comparing `speedruncompy-0.0.1/speedruncompy/auth.py` & `speedruncompy-0.0.2/speedruncompy/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import api
 from .endpoints import PutAuthLogin, PutAuthLogout, GetSession
 
-def login(username: str, pwd: str, token:str = None):
+def login(username: str, pwd: str):
     """Quick workflow to set sessid using username & pwd. Will prompt for auth token if required."""
-    result: dict = PutAuthLogin(username, pwd, token=token).perform()
+    result: dict = PutAuthLogin(username, pwd).perform()
     if result.get("loggedIn"):
         api._log.info("Logged in using username & password")
         return True
     if result.get("tokenChallengeSent"):
         api._log.warning("2FA is enabled - Not logged in!")
         key = input("Enter 2FA token: ")
         result: dict = PutAuthLogin(username, pwd, key).perform()
```

### Comparing `speedruncompy-0.0.1/speedruncompy/endpoints.py` & `speedruncompy-0.0.2/speedruncompy/endpoints.py`

 * *Files identical despite different names*

### Comparing `speedruncompy-0.0.1/speedruncompy/enums.py` & `speedruncompy-0.0.2/speedruncompy/enums.py`

 * *Files identical despite different names*


# Comparing `tmp/user-context-local-0.0.1.tar.gz` & `tmp/user-context-local-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-context-local-0.0.1.tar", last modified: Mon Aug  7 22:52:32 2023, max compression
+gzip compressed data, was "user-context-local-0.0.2.tar", last modified: Tue Aug  8 07:40:24 2023, max compression
```

## Comparing `user-context-local-0.0.1.tar` & `user-context-local-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:32.691568 user-context-local-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 22:52:32.691568 user-context-local-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-07 22:52:19.000000 user-context-local-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:32.691568 user-context-local-0.0.1/context_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:19.000000 user-context-local-0.0.1/context_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:32.691568 user-context-local-0.0.1/context_user/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:19.000000 user-context-local-0.0.1/context_user/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-07 22:52:19.000000 user-context-local-0.0.1/context_user/src/getIdByJwt.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 22:52:19.000000 user-context-local-0.0.1/context_user/src/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-07 22:52:19.000000 user-context-local-0.0.1/context_user/src/userContext.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-07 22:52:19.000000 user-context-local-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 22:52:32.691568 user-context-local-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-07 22:52:19.000000 user-context-local-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:52:32.691568 user-context-local-0.0.1/user_context_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-07 22:52:32.000000 user-context-local-0.0.1/user_context_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-07 22:52:32.000000 user-context-local-0.0.1/user_context_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:52:32.000000 user-context-local-0.0.1/user_context_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-07 22:52:32.000000 user-context-local-0.0.1/user_context_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:24.627764 user-context-local-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 07:40:24.623764 user-context-local-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-08 07:40:08.000000 user-context-local-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 07:40:08.000000 user-context-local-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:40:24.627764 user-context-local-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 07:40:08.000000 user-context-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:24.623764 user-context-local-0.0.2/user_context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:08.000000 user-context-local-0.0.2/user_context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:24.623764 user-context-local-0.0.2/user_context/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:08.000000 user-context-local-0.0.2/user_context/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-08 07:40:08.000000 user-context-local-0.0.2/user_context/src/getIdByJwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 07:40:08.000000 user-context-local-0.0.2/user_context/src/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-08 07:40:08.000000 user-context-local-0.0.2/user_context/src/userContext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:40:24.623764 user-context-local-0.0.2/user_context_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-08 07:40:24.000000 user-context-local-0.0.2/user_context_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-08 07:40:24.000000 user-context-local-0.0.2/user_context_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:40:24.000000 user-context-local-0.0.2/user_context_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 07:40:24.000000 user-context-local-0.0.2/user_context_local.egg-info/top_level.txt
```

### Comparing `user-context-local-0.0.1/README.md` & `user-context-local-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `user-context-local-0.0.1/context_user/src/getIdByJwt.py` & `user-context-local-0.0.2/user_context/src/getIdByJwt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import jwt
 import os
+import sys
 from dotenv import load_dotenv
 load_dotenv()
 
 def get_profile_and_user_id_from_jwt(jwt_token):
     try:
         secret_key = os.getenv("JWT_SECRET_KEY")
         decoded_payload = jwt.decode(jwt_token, secret_key, algorithms=['HS256'])
 
         profile_id = decoded_payload.get('profileId')  # Use 'profileId' instead of 'profile_id'
         user_id = decoded_payload.get('userId')  # Use 'userId' instead of 'user_id'
 
         return user_id,profile_id
     except jwt.ExpiredSignatureError:
         # Handle token expiration
-        print("JWT token has expired.")
+        print("JWT token has expired.",sys.stderr)
         return None, None
     except jwt.InvalidTokenError:
         # Handle invalid token
-        print("Invalid JWT token.")
+        print("Invalid JWT token.",sys.stderr)
         return None, None
```

### Comparing `user-context-local-0.0.1/context_user/src/userContext.py` & `user-context-local-0.0.2/user_context/src/userContext.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         return self.profile_id
     def set_fields_by_jwt(self,jwt):
         try:
             user_id,profile_id=get_profile_and_user_id_from_jwt(jwt)
             self.user_id=int(user_id)
             self.profile_id=int(profile_id)
         except Exception as e:
-            print(e)
+            print(e,sys.stderr)
```

### Comparing `user-context-local-0.0.1/pyproject.toml` & `user-context-local-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-context-local-0.0.1/setup.py` & `user-context-local-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 # The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
      # TODO: Please update the name and delete this line i.e. XXX-local or XXX-remote (without the -python-package suffix). Only lower case
      name='user-context-local',  
      # TODO: Please update the URL bellow
-     version='0.0.1', # https://pypi.org/project/<project-name>/
+     version='0.0.2', # https://pypi.org/project/<project-name>/
      author="Circles",
      author_email="info@circles.life",
      # TODO: Please update the description and delete this line
      description="PyPI Package for Circles <project-name> Local/Remote Python",
      # TODO: Please update the long description and delete this line    
      long_description="This is a package for sharing common XXX function used in different repositories",
      long_description_content_type="text/markdown",
```


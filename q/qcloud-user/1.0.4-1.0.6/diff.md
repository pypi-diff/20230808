# Comparing `tmp/qcloud_user-1.0.4.tar.gz` & `tmp/qcloud_user-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_user-1.0.4.tar", last modified: Thu Jul 27 12:15:53 2023, max compression
+gzip compressed data, was "qcloud_user-1.0.6.tar", last modified: Tue Aug  8 20:56:51 2023, max compression
```

## Comparing `qcloud_user-1.0.4.tar` & `qcloud_user-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.320183 qcloud_user-1.0.4/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.4/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-27 12:15:53.320062 qcloud_user-1.0.4/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.4/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      721 2023-07-27 12:15:04.000000 qcloud_user-1.0.4/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.319684 qcloud_user-1.0.4/qcloud_user.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      316 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       44 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      153 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       12 2023-07-27 12:15:53.000000 qcloud_user-1.0.4/qcloud_user.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-27 12:15:53.320219 qcloud_user-1.0.4/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      793 2023-07-27 12:15:22.000000 qcloud_user-1.0.4/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.318510 qcloud_user-1.0.4/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-27 12:15:53.319890 qcloud_user-1.0.4/src/qcloud_user/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.4/src/qcloud_user/__init__.py
--rwxr-x---   0 agilbert   (501) staff       (20)    22893 2023-07-27 11:01:31.000000 qcloud_user-1.0.4/src/qcloud_user/qcloud_user.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:56:51.222469 qcloud_user-1.0.6/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.6/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-08-08 20:56:51.222308 qcloud_user-1.0.6/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.6/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      721 2023-08-08 20:56:38.000000 qcloud_user-1.0.6/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:56:51.221261 qcloud_user-1.0.6/qcloud_user.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      316 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       44 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      153 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       12 2023-08-08 20:56:51.000000 qcloud_user-1.0.6/qcloud_user.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-08-08 20:56:51.222511 qcloud_user-1.0.6/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      793 2023-08-08 20:56:46.000000 qcloud_user-1.0.6/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:56:51.220094 qcloud_user-1.0.6/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-08-08 20:56:51.221480 qcloud_user-1.0.6/src/qcloud_user/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.6/src/qcloud_user/__init__.py
+-rwxr-x---   0 agilbert   (501) staff       (20)    23128 2023-07-31 02:10:00.000000 qcloud_user-1.0.6/src/qcloud_user/qcloud_user.py
```

### Comparing `qcloud_user-1.0.4/LICENSE.txt` & `qcloud_user-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.4/PKG-INFO` & `qcloud_user-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_user
-Version: 1.0.4
+Version: 1.0.6
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.4/README.md` & `qcloud_user-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.4/pyproject.toml` & `qcloud_user-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_user"
-version = "1.0.4"
+version = "1.0.6"
 description = "Q-Cloud CLI for users" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_user-1.0.4/qcloud_user.egg-info/PKG-INFO` & `qcloud_user-1.0.6/qcloud_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-user
-Version: 1.0.4
+Version: 1.0.6
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.4/setup.py` & `qcloud_user-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="qcloud_user",
     python_requires='>=3.7',
-    version="1.0.4",
+    version="1.0.6",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="CLI for interacting with Q-Cloud clusters",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['qcloud_user'],
```

### Comparing `qcloud_user-1.0.4/src/qcloud_user/qcloud_user.py` & `qcloud_user-1.0.6/src/qcloud_user/qcloud_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
     debug("----------------------------------")
 
     token = None
     region = config.get("AWS", "region")
     userpool = config.get("AWS", "userpoolid")
 
     if 'AuthenticationResult' in response:
+
        id_token = response['AuthenticationResult']['IdToken']
        if check_token(id_token, region, userpool):
           config.set("USER", "IdToken", id_token)
 
        access_token = response['AuthenticationResult']['AccessToken']
        if check_token(access_token, region, userpool):
           config.set("USER", "AccessToken", access_token)
@@ -280,14 +281,15 @@
 
 
 def get_token(session, config):
     region = config.get("AWS", "region")
     userpool = config.get("AWS", "userpoolid")
 
     token = None
+
     if config.has_option("USER", "IdToken"):
        token = config.get("USER", "IdToken")
 
     if token is not None:
        if check_token(token, region, userpool): return token
 
     token = get_new_token(session, config)
@@ -382,20 +384,24 @@
             body = file.read(); 
         if not filename.endswith('.json'):
            inp = body.splitlines()
            body = json.dumps({ "input_file": inp })
 
         response = requests.post(url, headers=headers, data=body)
         if "Submitted job id" in response.text: 
+           debug(response.headers)
            job_id   = response.text.replace("Submitted job id ","")
            job_name = pathlib.Path(filename).stem
            db.set_job(job_id, job_name)
            checklist("{}: ".format(response.text), job_name, True)
         else:
            print("[x] Problem submitting job: {}".format(response.text))
+           debug("Request headers: {}".format(json.dumps(headers)))
+           debug("Request Body:    {}".format(json.dumps(body)))
+           debug("Response headers {}".format(response.headers))
 
 
 
 def tail(token, job_ids, config, db):
     if not job_ids: return ""
     headers = {'Authorization': token}
     job_id = ",".join(job_ids)
```


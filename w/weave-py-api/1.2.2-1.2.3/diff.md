# Comparing `tmp/weave-py-api-1.2.2.tar.gz` & `tmp/weave-py-api-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-py-api-1.2.2.tar", last modified: Thu Jul  6 14:29:41 2023, max compression
+gzip compressed data, was "weave-py-api-1.2.3.tar", last modified: Tue Aug  8 12:12:05 2023, max compression
```

## Comparing `weave-py-api-1.2.2.tar` & `weave-py-api-1.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 14:29:41.472709 weave-py-api-1.2.2/
--rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2642 2023-07-06 14:29:41.472709 weave-py-api-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-06-08 14:14:22.000000 weave-py-api-1.2.2/README.md
--rw-rw-rw-   0        0        0     1436 2023-07-06 14:28:35.000000 weave-py-api-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 14:29:41.473710 weave-py-api-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-06 14:29:41.440709 weave-py-api-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 14:29:41.456707 weave-py-api-1.2.2/src/weave_py_api.egg-info/
--rw-rw-rw-   0        0        0     2642 2023-07-06 14:29:41.000000 weave-py-api-1.2.2/src/weave_py_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-07-06 14:29:41.000000 weave-py-api-1.2.2/src/weave_py_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 14:29:41.000000 weave-py-api-1.2.2/src/weave_py_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-07-06 14:29:41.000000 weave-py-api-1.2.2/src/weave_py_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 14:29:41.000000 weave-py-api-1.2.2/src/weave_py_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 14:29:41.471710 weave-py-api-1.2.2/src/weaveapi/
--rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.2.2/src/weaveapi/__init__.py
--rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.2.2/src/weaveapi/apicontext.py
--rw-rw-rw-   0        0        0    34883 2023-07-06 14:28:18.000000 weave-py-api-1.2.2/src/weaveapi/clienthttp.py
--rw-rw-rw-   0        0        0    41583 2023-07-06 14:28:11.000000 weave-py-api-1.2.2/src/weaveapi/clientws.py
--rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.2.2/src/weaveapi/filter.py
--rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.2.2/src/weaveapi/futures.py
--rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.2.2/src/weaveapi/javarandom.py
--rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.2.2/src/weaveapi/keys.py
--rw-rw-rw-   0        0        0    15106 2023-07-06 14:27:57.000000 weave-py-api-1.2.2/src/weaveapi/nodeapi.py
--rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.2.2/src/weaveapi/options.py
--rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.2.2/src/weaveapi/records.py
--rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.2.2/src/weaveapi/session.py
--rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.2.2/src/weaveapi/setup.py
--rw-rw-rw-   0        0        0     4302 2023-07-06 11:46:23.000000 weave-py-api-1.2.2/src/weaveapi/utils.py
--rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.2.2/src/weaveapi/weaveapi.py
--rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.2.2/src/weaveapi/weaveh.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:12:05.336840 weave-py-api-1.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2642 2023-08-08 12:12:05.323812 weave-py-api-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-06-08 14:14:22.000000 weave-py-api-1.2.3/README.md
+-rw-rw-rw-   0        0        0     1436 2023-08-08 12:10:18.000000 weave-py-api-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:12:05.336840 weave-py-api-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 12:12:05.109572 weave-py-api-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 12:12:05.180571 weave-py-api-1.2.3/src/weave_py_api.egg-info/
+-rw-rw-rw-   0        0        0     2642 2023-08-08 12:12:05.000000 weave-py-api-1.2.3/src/weave_py_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-08-08 12:12:05.000000 weave-py-api-1.2.3/src/weave_py_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:12:05.000000 weave-py-api-1.2.3/src/weave_py_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-08-08 12:12:05.000000 weave-py-api-1.2.3/src/weave_py_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 12:12:05.000000 weave-py-api-1.2.3/src/weave_py_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 12:12:05.323812 weave-py-api-1.2.3/src/weaveapi/
+-rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.2.3/src/weaveapi/__init__.py
+-rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.2.3/src/weaveapi/apicontext.py
+-rw-rw-rw-   0        0        0    34887 2023-07-16 11:46:10.000000 weave-py-api-1.2.3/src/weaveapi/clienthttp.py
+-rw-rw-rw-   0        0        0    41655 2023-07-16 11:46:10.000000 weave-py-api-1.2.3/src/weaveapi/clientws.py
+-rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.2.3/src/weaveapi/filter.py
+-rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.2.3/src/weaveapi/futures.py
+-rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.2.3/src/weaveapi/javarandom.py
+-rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.2.3/src/weaveapi/keys.py
+-rw-rw-rw-   0        0        0    15144 2023-07-16 11:46:10.000000 weave-py-api-1.2.3/src/weaveapi/nodeapi.py
+-rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.2.3/src/weaveapi/options.py
+-rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.2.3/src/weaveapi/records.py
+-rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.2.3/src/weaveapi/session.py
+-rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.2.3/src/weaveapi/setup.py
+-rw-rw-rw-   0        0        0     4302 2023-07-06 11:46:23.000000 weave-py-api-1.2.3/src/weaveapi/utils.py
+-rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.2.3/src/weaveapi/weaveapi.py
+-rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.2.3/src/weaveapi/weaveh.py
```

### Comparing `weave-py-api-1.2.2/LICENSE` & `weave-py-api-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/PKG-INFO` & `weave-py-api-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.2.2
+Version: 1.2.3
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `weave-py-api-1.2.2/README.md` & `weave-py-api-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/pyproject.toml` & `weave-py-api-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "weave-py-api"
-version = "1.2.2"
+version = "1.2.3"
 description = "Weavechain Python API"
 readme = "README.md"
 authors = [{ name = "Weavechain", email = "support@weavechain.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `weave-py-api-1.2.2/src/weave_py_api.egg-info/PKG-INFO` & `weave-py-api-1.2.3/src/weave_py_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.2.2
+Version: 1.2.3
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `weave-py-api-1.2.2/src/weave_py_api.egg-info/SOURCES.txt` & `weave-py-api-1.2.3/src/weave_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/apicontext.py` & `weave-py-api-1.2.3/src/weaveapi/apicontext.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/clienthttp.py` & `weave-py-api-1.2.3/src/weaveapi/clienthttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             self.serverSigKey,
             clientPublicKey,
             clientPrivateKey,
         )
         self.secretKey = self.keyExchange.sharedSecret(
             self.apiContext.clientPrivateKey, self.apiContext.serverPublicKey
         )
-        # print([b if b < 128 else b-256 for b in self.secretKey])
 
     def close(self):
         pass
 
     def version(self):
         reply = requests.get(self.apiUrl + "/version")
         return reply.content.decode("utf-8")
@@ -623,17 +622,18 @@
         data = {
             "image": image,
             "options": None if flOptions is None else flOptions.toJson(),
         }
 
         return self.authPost(session, "f_learn", data)
 
-    def splitLearn(self, session, image, slOptions):
+    def splitLearn(self, session, serverImage, clientImage, slOptions):
         data = {
-            "image": image,
+            "serverImage": serverImage,
+            "clientImage": clientImage,
             "options": None if slOptions is None else slOptions.toJson(),
         }
 
         return self.authPost(session, "split_learn", data)
 
     def balance(self, session, accountAddress, scope, token):
         toSign = (
```

### Comparing `weave-py-api-1.2.2/src/weaveapi/clientws.py` & `weave-py-api-1.2.3/src/weaveapi/clientws.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,20 +721,21 @@
             "account": session.account,
             "image": image,
             "options": None if flOptions is None else flOptions.toJson()
         }
 
         return self.authPost(session, data)
     
-    def splitLearn(self, session, image, slOptions):
+    def splitLearn(self, session, serverImage, clientImage, slOptions):
         data = {
             "type": "split_learn",
             "organization": session.organization,
             "account": session.account,
-            "image": image,
+            "serverImage": serverImage,
+            "clientImage": clientImage,
             "options": None if slOptions is None else slOptions.toJson()
         }
 
         return self.authPost(session, data)
 
 
     def balance(self, session, accountAddress, scope, token):
```

### Comparing `weave-py-api-1.2.2/src/weaveapi/filter.py` & `weave-py-api-1.2.3/src/weaveapi/filter.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/javarandom.py` & `weave-py-api-1.2.3/src/weaveapi/javarandom.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/keys.py` & `weave-py-api-1.2.3/src/weaveapi/keys.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/nodeapi.py` & `weave-py-api-1.2.3/src/weaveapi/nodeapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,16 @@
     
     def getImage(self, session, image, localOutputFolder, computeOptions):
         return self.client.getImage(session, image, localOutputFolder, computeOptions)
 
     def flearn(self, session, image, flOptions):
         return self.client.flearn(session, image, flOptions)
     
-    def splitLearn(self, session, image, slOptions):
-        return self.client.splitLearn(session, image, slOptions)
+    def splitLearn(self, session, serverImage, clientImage, slOptions):
+        return self.client.splitLearn(session, serverImage, clientImage, slOptions)
 
     def forwardApi(self, session, feedId, params):
         return self.client.forwardApi(session, feedId, params)
 
     def uploadApi(self, session, params):
         return self.client.uploadApi(session, params)
```

### Comparing `weave-py-api-1.2.2/src/weaveapi/options.py` & `weave-py-api-1.2.3/src/weaveapi/options.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/records.py` & `weave-py-api-1.2.3/src/weaveapi/records.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/session.py` & `weave-py-api-1.2.3/src/weaveapi/session.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/setup.py` & `weave-py-api-1.2.3/src/weaveapi/setup.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/utils.py` & `weave-py-api-1.2.3/src/weaveapi/utils.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.2/src/weaveapi/weaveh.py` & `weave-py-api-1.2.3/src/weaveapi/weaveh.py`

 * *Files identical despite different names*


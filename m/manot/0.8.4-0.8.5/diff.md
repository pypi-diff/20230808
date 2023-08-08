# Comparing `tmp/manot-0.8.4.tar.gz` & `tmp/manot-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manot-0.8.4.tar", last modified: Thu Jul 20 08:31:07 2023, max compression
+gzip compressed data, was "manot-0.8.5.tar", last modified: Tue Aug  8 08:25:28 2023, max compression
```

## Comparing `manot-0.8.4.tar` & `manot-0.8.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/
--rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.4/LICENSE
--rw-rw-r--   0 armen     (1000) armen     (1000)     7264 2023-07-20 08:31:07.203016 manot-0.8.4/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)     6300 2023-07-18 11:34:28.000000 manot-0.8.4/README.md
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/manot.egg-info/
--rw-rw-r--   0 armen     (1000) armen     (1000)     7264 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/SOURCES.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/dependency_links.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/requires.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/top_level.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-07-18 11:34:28.000000 manot-0.8.4/pyproject.toml
--rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-07-20 08:31:07.203016 manot-0.8.4/setup.cfg
--rw-rw-r--   0 armen     (1000) armen     (1000)      819 2023-07-18 11:34:28.000000 manot-0.8.4/setup.py
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/src/
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/src/manot/
--rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.4/src/manot/__init__.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.4/src/manot/logger.py
--rw-rw-r--   0 armen     (1000) armen     (1000)    12155 2023-07-20 08:29:25.000000 manot-0.8.4/src/manot/manot.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     4895 2023-07-20 08:29:21.000000 manot-0.8.4/src/manot/upload_manager.py
+drwxrwxr-x   0 manot     (1000) manot     (1000)        0 2023-08-08 08:25:28.278383 manot-0.8.5/
+-rw-rw-r--   0 manot     (1000) manot     (1000)     1061 2023-08-08 08:23:04.000000 manot-0.8.5/LICENSE
+-rw-rw-r--   0 manot     (1000) manot     (1000)     7264 2023-08-08 08:25:28.278383 manot-0.8.5/PKG-INFO
+-rw-rw-r--   0 manot     (1000) manot     (1000)     6300 2023-08-08 08:23:04.000000 manot-0.8.5/README.md
+drwxrwxr-x   0 manot     (1000) manot     (1000)        0 2023-08-08 08:25:28.278383 manot-0.8.5/manot.egg-info/
+-rw-rw-r--   0 manot     (1000) manot     (1000)     7264 2023-08-08 08:25:28.000000 manot-0.8.5/manot.egg-info/PKG-INFO
+-rw-rw-r--   0 manot     (1000) manot     (1000)      274 2023-08-08 08:25:28.000000 manot-0.8.5/manot.egg-info/SOURCES.txt
+-rw-rw-r--   0 manot     (1000) manot     (1000)        1 2023-08-08 08:25:28.000000 manot-0.8.5/manot.egg-info/dependency_links.txt
+-rw-rw-r--   0 manot     (1000) manot     (1000)       59 2023-08-08 08:25:28.000000 manot-0.8.5/manot.egg-info/requires.txt
+-rw-rw-r--   0 manot     (1000) manot     (1000)        6 2023-08-08 08:25:28.000000 manot-0.8.5/manot.egg-info/top_level.txt
+-rw-rw-r--   0 manot     (1000) manot     (1000)     1074 2023-08-08 08:25:17.000000 manot-0.8.5/pyproject.toml
+-rw-rw-r--   0 manot     (1000) manot     (1000)       38 2023-08-08 08:25:28.278383 manot-0.8.5/setup.cfg
+-rw-rw-r--   0 manot     (1000) manot     (1000)      819 2023-08-08 08:25:17.000000 manot-0.8.5/setup.py
+drwxrwxr-x   0 manot     (1000) manot     (1000)        0 2023-08-08 08:25:28.278383 manot-0.8.5/src/
+drwxrwxr-x   0 manot     (1000) manot     (1000)        0 2023-08-08 08:25:28.278383 manot-0.8.5/src/manot/
+-rw-rw-r--   0 manot     (1000) manot     (1000)       78 2023-08-08 08:23:04.000000 manot-0.8.5/src/manot/__init__.py
+-rw-rw-r--   0 manot     (1000) manot     (1000)     1358 2023-08-08 08:23:04.000000 manot-0.8.5/src/manot/logger.py
+-rw-rw-r--   0 manot     (1000) manot     (1000)    12229 2023-08-08 08:23:04.000000 manot-0.8.5/src/manot/manot.py
+-rw-rw-r--   0 manot     (1000) manot     (1000)     4895 2023-08-08 08:23:04.000000 manot-0.8.5/src/manot/upload_manager.py
```

### Comparing `manot-0.8.4/LICENSE` & `manot-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `manot-0.8.4/PKG-INFO` & `manot-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.4
+Version: 0.8.5
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
```

### Comparing `manot-0.8.4/README.md` & `manot-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `manot-0.8.4/manot.egg-info/PKG-INFO` & `manot-0.8.5/manot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.4
+Version: 0.8.5
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
```

### Comparing `manot-0.8.4/pyproject.toml` & `manot-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "manot"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
     { name = "manot", email = "engineering@manot.ai" },
 ]
 license = {text = "MIT"}
 description = "manot AI is a model observability platform to monitor computer vision performance in real-time."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `manot-0.8.4/setup.py` & `manot-0.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name='manot',
-    version='0.8.4',
+    version='0.8.5',
     description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the evaluation method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
     author='manot',
     author_email='engineering@manot.ai',
     url='https://www.manot.ai',
     packages=['manot'],
     package_dir={'manot': 'src/manot'},
     project_urls={
```

### Comparing `manot-0.8.4/src/manot/logger.py` & `manot-0.8.5/src/manot/logger.py`

 * *Files identical despite different names*

### Comparing `manot-0.8.4/src/manot/manot.py` & `manot-0.8.5/src/manot/manot.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,18 +314,20 @@
     def __process(self, image_id: int, deeplake_token: str = None, with_inference=False,huggingface_model=None):
 
         url = f"{self.__url}/api/v1/image/{image_id}?deeplake_token={deeplake_token}&with_inference={with_inference}&huggingface_model={huggingface_model}&time={time.time()}"
         return url
 
     def __check_progress(self, process_method, id):
         progress = 0
+        status = 'started'
         progress_bar = tqdm(desc="Progress", total=100)
-        while progress < 100:
+        while status == 'started':
             result = process_method(id)
             if result:
+                status = result['status']
                 if result["status"] != "failure":
                     progress_bar.update(int(result['progress'] - progress))
                     progress = result['progress']
                 if result["status"] in ["finished", "failure"]:
                     progress_bar.close()
                     return result
             else:
```

### Comparing `manot-0.8.4/src/manot/upload_manager.py` & `manot-0.8.5/src/manot/upload_manager.py`

 * *Files identical despite different names*


# Comparing `tmp/rubbrband-0.2.8.tar.gz` & `tmp/rubbrband-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.8.tar", last modified: Tue Jul 25 23:05:41 2023, max compression
+gzip compressed data, was "rubbrband-0.2.9.tar", last modified: Thu Jul 27 22:30:33 2023, max compression
```

## Comparing `rubbrband-0.2.8.tar` & `rubbrband-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.239253 rubbrband-0.2.8/
--rw-r--r--   0 darren     (501) staff       (20)    11357 2023-06-13 23:04:48.000000 rubbrband-0.2.8/LICENSE
--rw-r--r--   0 darren     (501) staff       (20)       48 2023-06-13 23:04:48.000000 rubbrband-0.2.8/MANIFEST.in
--rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-25 23:05:41.239318 rubbrband-0.2.8/PKG-INFO
--rw-r--r--   0 darren     (501) staff       (20)       54 2023-06-13 23:22:30.000000 rubbrband-0.2.8/README.md
--rw-r--r--   0 darren     (501) staff       (20)      103 2023-07-25 21:52:43.000000 rubbrband-0.2.8/pyproject.toml
-drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.238263 rubbrband-0.2.8/rubbrband/
--rw-r--r--   0 darren     (501) staff       (20)       61 2023-06-13 23:28:05.000000 rubbrband-0.2.8/rubbrband/__init__.py
--rw-r--r--   0 darren     (501) staff       (20)     1613 2023-07-25 23:05:10.000000 rubbrband-0.2.8/rubbrband/main.py
-drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-25 23:05:41.239087 rubbrband-0.2.8/rubbrband.egg-info/
--rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 darren     (501) staff       (20)      267 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 darren     (501) staff       (20)        1 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 darren     (501) staff       (20)       16 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/requires.txt
--rw-r--r--   0 darren     (501) staff       (20)       10 2023-07-25 23:05:41.000000 rubbrband-0.2.8/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 darren     (501) staff       (20)      259 2023-07-25 23:05:41.239615 rubbrband-0.2.8/setup.cfg
--rw-r--r--   0 darren     (501) staff       (20)      182 2023-07-25 21:52:43.000000 rubbrband-0.2.8/setup.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-27 22:30:33.365834 rubbrband-0.2.9/
+-rw-r--r--   0 darren     (501) staff       (20)    11357 2023-06-13 23:04:48.000000 rubbrband-0.2.9/LICENSE
+-rw-r--r--   0 darren     (501) staff       (20)       48 2023-06-13 23:04:48.000000 rubbrband-0.2.9/MANIFEST.in
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-27 22:30:33.365899 rubbrband-0.2.9/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)     1075 2023-07-27 22:26:56.000000 rubbrband-0.2.9/README.md
+-rw-r--r--   0 darren     (501) staff       (20)      103 2023-07-25 21:52:43.000000 rubbrband-0.2.9/pyproject.toml
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-27 22:30:33.364421 rubbrband-0.2.9/rubbrband/
+-rw-r--r--   0 darren     (501) staff       (20)       61 2023-06-13 23:28:05.000000 rubbrband-0.2.9/rubbrband/__init__.py
+-rw-r--r--   0 darren     (501) staff       (20)     1985 2023-07-27 22:30:08.000000 rubbrband-0.2.9/rubbrband/main.py
+drwxr-xr-x   0 darren     (501) staff       (20)        0 2023-07-27 22:30:33.365671 rubbrband-0.2.9/rubbrband.egg-info/
+-rw-r--r--   0 darren     (501) staff       (20)      125 2023-07-27 22:30:33.000000 rubbrband-0.2.9/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 darren     (501) staff       (20)      267 2023-07-27 22:30:33.000000 rubbrband-0.2.9/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 darren     (501) staff       (20)        1 2023-07-27 22:30:33.000000 rubbrband-0.2.9/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 darren     (501) staff       (20)       16 2023-07-27 22:30:33.000000 rubbrband-0.2.9/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 darren     (501) staff       (20)       10 2023-07-27 22:30:33.000000 rubbrband-0.2.9/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 darren     (501) staff       (20)      259 2023-07-27 22:30:33.366206 rubbrband-0.2.9/setup.cfg
+-rw-r--r--   0 darren     (501) staff       (20)      182 2023-07-25 21:52:43.000000 rubbrband-0.2.9/setup.py
```

### Comparing `rubbrband-0.2.8/LICENSE` & `rubbrband-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rubbrband-0.2.8/rubbrband/main.py` & `rubbrband-0.2.9/rubbrband/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
+import os
 import re
 
-import PIL
-import PIL.PngImagePlugin
 import requests
+from PIL import Image
 
 api_key = None
 
 
 def init(apikey):
     global api_key
     api_key = apikey
@@ -18,31 +18,44 @@
     imgByteArr = io.BytesIO()
     # image.save expects a file-like as a argument
     image.save(imgByteArr, format=image.format)
     # Turn the BytesIO object back into a bytes object
     imgByteArr = imgByteArr.getvalue()
     return imgByteArr
 
+
 def is_url(string):
     regex_pattern = r"^(https?|ftp):\/\/([^\s/$.?#].[^\s]*)$"
     return bool(re.match(regex_pattern, string))
 
+
 def upload(image, prompt, metadata={}):
     if api_key is None:
         print("Provide an API key in the init function")
         return False
 
+    # Handle image input
     if type(image) == str and is_url(image):
+        # If image is a url, download it
         image_url_response = requests.get(image)
         if image_url_response.status_code != 200 or image_url_response.content is None:
             return False
         image = image_url_response.content
-
-    if type(image) == PIL.PngImagePlugin.PngImageFile:
+    elif isinstance(image, Image.Image):
+        # If image is a PIL, convert it to bytes
         image = image_to_byte_array(image)
+    elif type(image) == str and os.path.isfile(image):
+        # If image is a file path, read it
+        with open(image, "rb") as f:
+            image = f.read()
+    elif type(image) == bytes:
+        pass
+    else:
+        print("Invalid image type")
+        return False
 
     metadata["prompt"] = prompt
 
     response = requests.post(
         "https://block.rubbrband.com/upload_img?api_key=" + api_key,
         json={"metadata": metadata},
     )
```


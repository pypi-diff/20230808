# Comparing `tmp/gm2m_relations-1.0.0.tar.gz` & `tmp/gm2m_relations-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gm2m_relations-1.0.0.tar", last modified: Tue Aug  8 08:00:50 2023, max compression
+gzip compressed data, was "gm2m_relations-1.0.1.tar", last modified: Tue Aug  8 08:03:04 2023, max compression
```

## Comparing `gm2m_relations-1.0.0.tar` & `gm2m_relations-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:00:50.034997 gm2m_relations-1.0.0/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1066 2023-08-08 07:28:47.000000 gm2m_relations-1.0.0/LICENCE
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:00:50.034997 gm2m_relations-1.0.0/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     2778 2023-08-08 07:59:42.000000 gm2m_relations-1.0.0/README.md
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:00:50.034997 gm2m_relations-1.0.0/gm2m_relations/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 07:28:47.000000 gm2m_relations-1.0.0/gm2m_relations/__init__.py
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1790 2023-08-08 07:34:39.000000 gm2m_relations-1.0.0/gm2m_relations/serializers.py
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:00:50.034997 gm2m_relations-1.0.0/gm2m_relations.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:00:49.000000 gm2m_relations-1.0.0/gm2m_relations.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      272 2023-08-08 08:00:49.000000 gm2m_relations-1.0.0/gm2m_relations.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-08-08 08:00:49.000000 gm2m_relations-1.0.0/gm2m_relations.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       33 2023-08-08 08:00:49.000000 gm2m_relations-1.0.0/gm2m_relations.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       15 2023-08-08 08:00:49.000000 gm2m_relations-1.0.0/gm2m_relations.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-08-08 08:00:50.034997 gm2m_relations-1.0.0/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      664 2023-08-08 07:33:48.000000 gm2m_relations-1.0.0/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1066 2023-08-08 07:28:47.000000 gm2m_relations-1.0.1/LICENCE
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     2778 2023-08-08 08:02:46.000000 gm2m_relations-1.0.1/README.md
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/gm2m_relations/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 07:28:47.000000 gm2m_relations-1.0.1/gm2m_relations/__init__.py
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1790 2023-08-08 07:34:39.000000 gm2m_relations-1.0.1/gm2m_relations/serializers.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/gm2m_relations.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      272 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       33 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       15 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      664 2023-08-08 08:02:54.000000 gm2m_relations-1.0.1/setup.py
```

### Comparing `gm2m_relations-1.0.0/LICENCE` & `gm2m_relations-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `gm2m_relations-1.0.0/PKG-INFO` & `gm2m_relations-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm2m_relations
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library implements Django REST Framework serializers to handle generic many to many relations.
 Home-page: https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations
 Author: mojtaba akbari
 Author-email: mojtaba.akbari.221b@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
 
 Install using `pip` :
 ```sh
-pip install gm2m_relations
+pip install gm2m-relations
 ```
 
 # API Reference
 
 ## GM2MSerializer
 
 serializes django generic many-to-many field. For a primer on generic many-to-many field, first see: https://github.com/tkhyn/django-gm2m
```

### Comparing `gm2m_relations-1.0.0/README.md` & `gm2m_relations-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
 
 Install using `pip` :
 ```sh
-pip install gm2m_relations
+pip install gm2m-relations
 ```
 
 # API Reference
 
 ## GM2MSerializer
 
 serializes django generic many-to-many field. For a primer on generic many-to-many field, first see: https://github.com/tkhyn/django-gm2m
```

### Comparing `gm2m_relations-1.0.0/gm2m_relations/serializers.py` & `gm2m_relations-1.0.1/gm2m_relations/serializers.py`

 * *Files identical despite different names*

### Comparing `gm2m_relations-1.0.0/gm2m_relations.egg-info/PKG-INFO` & `gm2m_relations-1.0.1/gm2m_relations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm2m-relations
-Version: 1.0.0
+Version: 1.0.1
 Summary: This library implements Django REST Framework serializers to handle generic many to many relations.
 Home-page: https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations
 Author: mojtaba akbari
 Author-email: mojtaba.akbari.221b@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
 
 Install using `pip` :
 ```sh
-pip install gm2m_relations
+pip install gm2m-relations
 ```
 
 # API Reference
 
 ## GM2MSerializer
 
 serializes django generic many-to-many field. For a primer on generic many-to-many field, first see: https://github.com/tkhyn/django-gm2m
```

### Comparing `gm2m_relations-1.0.0/setup.py` & `gm2m_relations-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setuptools.setup(
     name="gm2m_relations",
-    version="1.0.0",
+    version="1.0.1",
     author="mojtaba akbari",
     author_email="mojtaba.akbari.221b@gmail.com",
     packages=["gm2m_relations"],
     description="This library implements Django REST Framework serializers to handle generic many to many relations.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations",
```


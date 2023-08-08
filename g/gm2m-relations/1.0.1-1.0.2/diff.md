# Comparing `tmp/gm2m_relations-1.0.1.tar.gz` & `tmp/gm2m_relations-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gm2m_relations-1.0.1.tar", last modified: Tue Aug  8 08:03:04 2023, max compression
+gzip compressed data, was "gm2m_relations-1.0.2.tar", last modified: Tue Aug  8 08:31:36 2023, max compression
```

## Comparing `gm2m_relations-1.0.1.tar` & `gm2m_relations-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1066 2023-08-08 07:28:47.000000 gm2m_relations-1.0.1/LICENCE
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     2778 2023-08-08 08:02:46.000000 gm2m_relations-1.0.1/README.md
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/gm2m_relations/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 07:28:47.000000 gm2m_relations-1.0.1/gm2m_relations/__init__.py
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1790 2023-08-08 07:34:39.000000 gm2m_relations-1.0.1/gm2m_relations/serializers.py
-drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/gm2m_relations.egg-info/
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/PKG-INFO
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      272 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/SOURCES.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/dependency_links.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       33 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/requires.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       15 2023-08-08 08:03:04.000000 gm2m_relations-1.0.1/gm2m_relations.egg-info/top_level.txt
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-08-08 08:03:04.434362 gm2m_relations-1.0.1/setup.cfg
--rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      664 2023-08-08 08:02:54.000000 gm2m_relations-1.0.1/setup.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:31:36.038571 gm2m_relations-1.0.2/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1066 2023-08-08 07:28:47.000000 gm2m_relations-1.0.2/LICENCE
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:31:36.038571 gm2m_relations-1.0.2/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     2778 2023-08-08 08:28:36.000000 gm2m_relations-1.0.2/README.md
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:31:36.022571 gm2m_relations-1.0.2/gm2m_relations/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 07:28:47.000000 gm2m_relations-1.0.2/gm2m_relations/__init__.py
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     1790 2023-08-08 07:34:39.000000 gm2m_relations-1.0.2/gm2m_relations/serializers.py
+drwxrwxr-x   0 mojtaba   (1000) mojtaba   (1000)        0 2023-08-08 08:31:36.034571 gm2m_relations-1.0.2/gm2m_relations.egg-info/
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)     3189 2023-08-08 08:31:35.000000 gm2m_relations-1.0.2/gm2m_relations.egg-info/PKG-INFO
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      272 2023-08-08 08:31:35.000000 gm2m_relations-1.0.2/gm2m_relations.egg-info/SOURCES.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)        1 2023-08-08 08:31:35.000000 gm2m_relations-1.0.2/gm2m_relations.egg-info/dependency_links.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       33 2023-08-08 08:31:35.000000 gm2m_relations-1.0.2/gm2m_relations.egg-info/requires.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       15 2023-08-08 08:31:35.000000 gm2m_relations-1.0.2/gm2m_relations.egg-info/top_level.txt
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)       38 2023-08-08 08:31:36.038571 gm2m_relations-1.0.2/setup.cfg
+-rw-rw-r--   0 mojtaba   (1000) mojtaba   (1000)      664 2023-08-08 08:28:54.000000 gm2m_relations-1.0.2/setup.py
```

### Comparing `gm2m_relations-1.0.1/LICENCE` & `gm2m_relations-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `gm2m_relations-1.0.1/PKG-INFO` & `gm2m_relations-1.0.2/gm2m_relations.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: gm2m_relations
-Version: 1.0.1
+Name: gm2m-relations
+Version: 1.0.2
 Summary: This library implements Django REST Framework serializers to handle generic many to many relations.
 Home-page: https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations
 Author: mojtaba akbari
 Author-email: mojtaba.akbari.221b@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # gm2m_relations
 
-This library implements [Django REST Framework](http://www.django-rest-framework.org/) serializers to handle generic many to many relations.
+The `rest-framework-gm2m-relations` library provides read/write serialization for [django-gm2m](https://github.com/tkhyn/django-gm2m) field.
 
 # Requirements
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
```

### Comparing `gm2m_relations-1.0.1/README.md` & `gm2m_relations-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gm2m_relations
 
-This library implements [Django REST Framework](http://www.django-rest-framework.org/) serializers to handle generic many to many relations.
+The `rest-framework-gm2m-relations` library provides read/write serialization for [django-gm2m](https://github.com/tkhyn/django-gm2m) field.
 
 # Requirements
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
```

### Comparing `gm2m_relations-1.0.1/gm2m_relations/serializers.py` & `gm2m_relations-1.0.2/gm2m_relations/serializers.py`

 * *Files identical despite different names*

### Comparing `gm2m_relations-1.0.1/gm2m_relations.egg-info/PKG-INFO` & `gm2m_relations-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: gm2m-relations
-Version: 1.0.1
+Name: gm2m_relations
+Version: 1.0.2
 Summary: This library implements Django REST Framework serializers to handle generic many to many relations.
 Home-page: https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations
 Author: mojtaba akbari
 Author-email: mojtaba.akbari.221b@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # gm2m_relations
 
-This library implements [Django REST Framework](http://www.django-rest-framework.org/) serializers to handle generic many to many relations.
+The `rest-framework-gm2m-relations` library provides read/write serialization for [django-gm2m](https://github.com/tkhyn/django-gm2m) field.
 
 # Requirements
 
 Any currently-supported combination of [rest-framework-generic-relations](https://github.com/LilyFoote/rest-framework-generic-relations), Django REST Framework, Python, and Django.
 
 # Installation
```

### Comparing `gm2m_relations-1.0.1/setup.py` & `gm2m_relations-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setuptools.setup(
     name="gm2m_relations",
-    version="1.0.1",
+    version="1.0.2",
     author="mojtaba akbari",
     author_email="mojtaba.akbari.221b@gmail.com",
     packages=["gm2m_relations"],
     description="This library implements Django REST Framework serializers to handle generic many to many relations.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/mojtabaakbari221b/rest-framework-gm2m-relations",
```


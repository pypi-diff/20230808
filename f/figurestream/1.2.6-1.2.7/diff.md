# Comparing `tmp/figurestream-1.2.6.tar.gz` & `tmp/figurestream-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurestream-1.2.6.tar", last modified: Tue Jun  7 00:48:49 2022, max compression
+gzip compressed data, was "figurestream-1.2.7.tar", last modified: Tue Aug  8 17:16:52 2023, max compression
```

## Comparing `figurestream-1.2.6.tar` & `figurestream-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2022-06-07 00:48:49.333279 figurestream-1.2.6/
--rw-r--r--   0 yeison    (1000) users      (984)     1315 2021-05-25 23:59:33.000000 figurestream-1.2.6/LICENSE
--rw-r--r--   0 yeison    (1000) users      (984)      151 2021-05-25 23:59:33.000000 figurestream-1.2.6/MANIFEST.in
--rw-r--r--   0 yeison    (1000) users      (984)     5406 2022-06-07 00:48:49.333279 figurestream-1.2.6/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)     3968 2021-05-25 23:59:33.000000 figurestream-1.2.6/README.md
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2022-06-07 00:48:49.333279 figurestream-1.2.6/figurestream/
--rw-r--r--   0 yeison    (1000) users      (984)     9224 2021-09-22 04:17:42.000000 figurestream-1.2.6/figurestream/__init__.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2022-06-07 00:48:49.333279 figurestream-1.2.6/figurestream.egg-info/
--rw-r--r--   0 yeison    (1000) users      (984)     5406 2022-06-07 00:48:48.000000 figurestream-1.2.6/figurestream.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)      242 2022-06-07 00:48:49.000000 figurestream-1.2.6/figurestream.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2022-06-07 00:48:48.000000 figurestream-1.2.6/figurestream.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (984)       17 2022-06-07 00:48:49.000000 figurestream-1.2.6/figurestream.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) users      (984)       13 2022-06-07 00:48:49.000000 figurestream-1.2.6/figurestream.egg-info/top_level.txt
--rw-r--r--   0 yeison    (1000) users      (984)       38 2022-06-07 00:48:49.333279 figurestream-1.2.6/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (984)     2083 2022-06-07 00:48:31.000000 figurestream-1.2.6/setup.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 17:16:52.282112 figurestream-1.2.7/
+-rw-r--r--   0 yeison    (1000) users      (984)     1315 2021-05-25 23:59:33.000000 figurestream-1.2.7/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)      151 2021-05-25 23:59:33.000000 figurestream-1.2.7/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) users      (984)     5386 2023-08-08 17:16:52.278778 figurestream-1.2.7/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)     3968 2021-05-25 23:59:33.000000 figurestream-1.2.7/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 17:16:52.278778 figurestream-1.2.7/figurestream/
+-rw-r--r--   0 yeison    (1000) users      (984)     9224 2021-09-22 04:17:42.000000 figurestream-1.2.7/figurestream/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 17:16:52.278778 figurestream-1.2.7/figurestream.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)     5386 2023-08-08 17:16:52.000000 figurestream-1.2.7/figurestream.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)      242 2023-08-08 17:16:52.000000 figurestream-1.2.7/figurestream.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-08-08 17:16:52.000000 figurestream-1.2.7/figurestream.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       17 2023-08-08 17:16:52.000000 figurestream-1.2.7/figurestream.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       13 2023-08-08 17:16:52.000000 figurestream-1.2.7/figurestream.egg-info/top_level.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-08-08 17:16:52.282112 figurestream-1.2.7/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     2083 2023-08-08 17:15:42.000000 figurestream-1.2.7/setup.py
```

### Comparing `figurestream-1.2.6/LICENSE` & `figurestream-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `figurestream-1.2.6/PKG-INFO` & `figurestream-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: figurestream
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Matplotlib.Figure fork with real-time plot streaming features.
 Download-URL: https://github.com/UN-GCPDS/matplotlib-figurestream
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -141,9 +140,7 @@
 
 ```python
 FigureStream(host='0.0.0.0', port='5500', endpoint='figure.jpeg')
 ```
 
 Now the stream will serve on http://localhost:5500/figure.jpeg and due the `0.0.0.0` host is accesible for any device on network.  
 By default `host` is `localhost`, `port` is `5000` and endopoint is empty.
-
-
```

### Comparing `figurestream-1.2.6/README.md` & `figurestream-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `figurestream-1.2.6/figurestream/__init__.py` & `figurestream-1.2.7/figurestream/__init__.py`

 * *Files identical despite different names*

### Comparing `figurestream-1.2.6/figurestream.egg-info/PKG-INFO` & `figurestream-1.2.7/figurestream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: figurestream
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Matplotlib.Figure fork with real-time plot streaming features.
 Download-URL: https://github.com/UN-GCPDS/matplotlib-figurestream
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -141,9 +140,7 @@
 
 ```python
 FigureStream(host='0.0.0.0', port='5500', endpoint='figure.jpeg')
 ```
 
 Now the stream will serve on http://localhost:5500/figure.jpeg and due the `0.0.0.0` host is accesible for any device on network.  
 By default `host` is `localhost`, `port` is `5000` and endopoint is empty.
-
-
```

### Comparing `figurestream-1.2.6/setup.py` & `figurestream-1.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 setup(
     name='figurestream',
-    version='1.2.6',
+    version='1.2.7',
     packages=['figurestream'],
 
     author='Yeison Cardona',
     author_email='yencardonaal@unal.edu.co',
     maintainer='Yeison Cardona',
     maintainer_email='yencardonaal@unal.edu.co',
```


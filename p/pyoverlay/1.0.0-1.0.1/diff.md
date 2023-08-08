# Comparing `tmp/pyoverlay-1.0.0.tar.gz` & `tmp/pyoverlay-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoverlay-1.0.0.tar", last modified: Tue Aug  8 12:04:50 2023, max compression
+gzip compressed data, was "pyoverlay-1.0.1.tar", last modified: Tue Aug  8 12:10:12 2023, max compression
```

## Comparing `pyoverlay-1.0.0.tar` & `pyoverlay-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 12:04:50.448000 pyoverlay-1.0.0/
--rw-rw-rw-   0        0        0        0 2023-08-08 10:44:42.000000 pyoverlay-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      541 2023-08-08 12:04:50.441000 pyoverlay-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-08 10:45:01.000000 pyoverlay-1.0.0/README.md
--rw-rw-rw-   0        0        0      703 2023-08-08 12:04:28.000000 pyoverlay-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-08 12:04:50.446000 pyoverlay-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-08 12:04:50.302000 pyoverlay-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-08 12:04:50.370000 pyoverlay-1.0.0/src/pyoverlay/
--rw-rw-rw-   0        0        0       74 2023-08-07 16:12:45.000000 pyoverlay-1.0.0/src/pyoverlay/__init__.py
--rw-rw-rw-   0        0        0     2264 2023-08-07 21:05:21.000000 pyoverlay-1.0.0/src/pyoverlay/helper.py
--rw-rw-rw-   0        0        0    15459 2023-08-07 22:03:48.000000 pyoverlay-1.0.0/src/pyoverlay/overlay.py
-drwxrwxrwx   0        0        0        0 2023-08-08 12:04:50.429000 pyoverlay-1.0.0/src/pyoverlay.egg-info/
--rw-rw-rw-   0        0        0      541 2023-08-08 12:04:50.000000 pyoverlay-1.0.0/src/pyoverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-08-08 12:04:50.000000 pyoverlay-1.0.0/src/pyoverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 12:04:50.000000 pyoverlay-1.0.0/src/pyoverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-08-08 12:04:50.000000 pyoverlay-1.0.0/src/pyoverlay.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-08 12:04:50.000000 pyoverlay-1.0.0/src/pyoverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 12:10:12.902000 pyoverlay-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-08-08 10:44:42.000000 pyoverlay-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      585 2023-08-08 12:10:12.896000 pyoverlay-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-08 10:45:01.000000 pyoverlay-1.0.1/README.md
+-rw-rw-rw-   0        0        0      742 2023-08-08 12:09:55.000000 pyoverlay-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 12:10:12.901000 pyoverlay-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 12:10:12.769000 pyoverlay-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 12:10:12.831000 pyoverlay-1.0.1/src/pyoverlay/
+-rw-rw-rw-   0        0        0       74 2023-08-07 16:12:45.000000 pyoverlay-1.0.1/src/pyoverlay/__init__.py
+-rw-rw-rw-   0        0        0     2264 2023-08-07 21:05:21.000000 pyoverlay-1.0.1/src/pyoverlay/helper.py
+-rw-rw-rw-   0        0        0    15459 2023-08-07 22:03:48.000000 pyoverlay-1.0.1/src/pyoverlay/overlay.py
+drwxrwxrwx   0        0        0        0 2023-08-08 12:10:12.890000 pyoverlay-1.0.1/src/pyoverlay.egg-info/
+-rw-rw-rw-   0        0        0      585 2023-08-08 12:10:12.000000 pyoverlay-1.0.1/src/pyoverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-08-08 12:10:12.000000 pyoverlay-1.0.1/src/pyoverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 12:10:12.000000 pyoverlay-1.0.1/src/pyoverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-08-08 12:10:12.000000 pyoverlay-1.0.1/src/pyoverlay.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 12:10:12.000000 pyoverlay-1.0.1/src/pyoverlay.egg-info/top_level.txt
```

### Comparing `pyoverlay-1.0.0/PKG-INFO` & `pyoverlay-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pyoverlay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easily create overlay on top of any game/application
 Author-email: majvax <majvax.contact@gmail.com>
 Project-URL: Homepage, https://github.com/majvax/pyoverlay
 Project-URL: Bug Tracker, https://github.com/majvax/pyoverlay/issues
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyoverlay-1.0.0/pyproject.toml` & `pyoverlay-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoverlay"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="majvax", email="majvax.contact@gmail.com" },
 ]
 description = "Easily create overlay on top of any game/application"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows"
 ]
 dependencies = [
   "rich",
   "pywin32",
```

### Comparing `pyoverlay-1.0.0/src/pyoverlay/helper.py` & `pyoverlay-1.0.1/src/pyoverlay/helper.py`

 * *Files identical despite different names*

### Comparing `pyoverlay-1.0.0/src/pyoverlay/overlay.py` & `pyoverlay-1.0.1/src/pyoverlay/overlay.py`

 * *Files identical despite different names*

### Comparing `pyoverlay-1.0.0/src/pyoverlay.egg-info/PKG-INFO` & `pyoverlay-1.0.1/src/pyoverlay.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pyoverlay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easily create overlay on top of any game/application
 Author-email: majvax <majvax.contact@gmail.com>
 Project-URL: Homepage, https://github.com/majvax/pyoverlay
 Project-URL: Bug Tracker, https://github.com/majvax/pyoverlay/issues
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


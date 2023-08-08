# Comparing `tmp/sphinx-versioning-0.0.1.tar.gz` & `tmp/sphinx-versioning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-versioning-0.0.1.tar", last modified: Tue Aug  8 18:06:46 2023, max compression
+gzip compressed data, was "sphinx-versioning-0.0.2.tar", last modified: Tue Aug  8 18:51:38 2023, max compression
```

## Comparing `sphinx-versioning-0.0.1.tar` & `sphinx-versioning-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 18:06:46.181486 sphinx-versioning-0.0.1/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-06-05 07:14:29.000000 sphinx-versioning-0.0.1/LICENSE
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2412 2023-08-08 18:06:46.181369 sphinx-versioning-0.0.1/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1606 2023-08-08 18:06:36.000000 sphinx-versioning-0.0.1/README.md
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 18:06:46.180139 sphinx-versioning-0.0.1/scripts/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1730 2023-08-08 18:04:03.000000 sphinx-versioning-0.0.1/scripts/sphinx-version
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-08-08 18:06:46.181526 sphinx-versioning-0.0.1/setup.cfg
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1042 2023-08-08 18:04:03.000000 sphinx-versioning-0.0.1/setup.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 18:06:46.180475 sphinx-versioning-0.0.1/sphinx_versioning/
--rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-08-08 18:04:03.000000 sphinx-versioning-0.0.1/sphinx_versioning/__init__.py
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1952 2023-08-08 18:04:03.000000 sphinx-versioning-0.0.1/sphinx_versioning/sphinx_versioning.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-08-08 18:06:46.181168 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2412 2023-08-08 18:06:46.000000 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)      322 2023-08-08 18:06:46.000000 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-08-08 18:06:46.000000 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        7 2023-08-08 18:06:46.000000 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/requires.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       18 2023-08-08 18:06:46.000000 sphinx-versioning-0.0.1/sphinx_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 yixiong  (51614) staff       (20)        0 2023-08-08 18:51:38.073203 sphinx-versioning-0.0.2/
+-rw-r--r--   0 yixiong  (51614) staff       (20)     1069 2023-08-08 18:20:32.000000 sphinx-versioning-0.0.2/LICENSE
+-rw-r--r--   0 yixiong  (51614) staff       (20)     2412 2023-08-08 18:51:38.073074 sphinx-versioning-0.0.2/PKG-INFO
+-rw-r--r--   0 yixiong  (51614) staff       (20)     1606 2023-08-08 18:44:57.000000 sphinx-versioning-0.0.2/README.md
+drwxr-xr-x   0 yixiong  (51614) staff       (20)        0 2023-08-08 18:51:38.071353 sphinx-versioning-0.0.2/scripts/
+-rw-r--r--   0 yixiong  (51614) staff       (20)     1730 2023-08-08 18:50:13.000000 sphinx-versioning-0.0.2/scripts/sphinx-version.py
+-rw-r--r--   0 yixiong  (51614) staff       (20)       38 2023-08-08 18:51:38.073247 sphinx-versioning-0.0.2/setup.cfg
+-rw-r--r--   0 yixiong  (51614) staff       (20)     1045 2023-08-08 18:50:46.000000 sphinx-versioning-0.0.2/setup.py
+drwxr-xr-x   0 yixiong  (51614) staff       (20)        0 2023-08-08 18:51:38.071907 sphinx-versioning-0.0.2/sphinx_versioning/
+-rw-r--r--   0 yixiong  (51614) staff       (20)       37 2023-08-08 18:20:32.000000 sphinx-versioning-0.0.2/sphinx_versioning/__init__.py
+-rw-r--r--   0 yixiong  (51614) staff       (20)     1952 2023-08-08 18:20:32.000000 sphinx-versioning-0.0.2/sphinx_versioning/sphinx_versioning.py
+drwxr-xr-x   0 yixiong  (51614) staff       (20)        0 2023-08-08 18:51:38.072859 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/
+-rw-r--r--   0 yixiong  (51614) staff       (20)     2412 2023-08-08 18:51:38.000000 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 yixiong  (51614) staff       (20)      325 2023-08-08 18:51:38.000000 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 yixiong  (51614) staff       (20)        1 2023-08-08 18:51:38.000000 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 yixiong  (51614) staff       (20)        7 2023-08-08 18:51:38.000000 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/requires.txt
+-rw-r--r--   0 yixiong  (51614) staff       (20)       18 2023-08-08 18:51:38.000000 sphinx-versioning-0.0.2/sphinx_versioning.egg-info/top_level.txt
```

### Comparing `sphinx-versioning-0.0.1/LICENSE` & `sphinx-versioning-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-versioning-0.0.1/PKG-INFO` & `sphinx-versioning-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx-versioning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Sphinx extension to manage versioned documentation
-Home-page: https://github.com/Yihengxiong6/sphinx-versioning
+Home-page: https://github.com/Yihengxiong6/sphinx_versioning
 Author: Yiheng Xiong
 Author-email: georgex8866@gmail.com
 License: MIT
 Keywords: sphinx documentation versioning
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sphinx-versioning-0.0.1/README.md` & `sphinx-versioning-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-versioning-0.0.1/scripts/sphinx-version` & `sphinx-versioning-0.0.2/scripts/sphinx-version.py`

 * *Files identical despite different names*

### Comparing `sphinx-versioning-0.0.1/setup.py` & `sphinx-versioning-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sphinx-versioning',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
-    scripts=['scripts/sphinx-version'],
-    url='https://github.com/Yihengxiong6/sphinx-versioning',
+    scripts=['scripts/sphinx-version.py'],
+    url='https://github.com/Yihengxiong6/sphinx_versioning',
     author='Yiheng Xiong',
     author_email='georgex8866@gmail.com',
     description='A Sphinx extension to manage versioned documentation',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',
     classifiers=[
```

### Comparing `sphinx-versioning-0.0.1/sphinx_versioning/sphinx_versioning.py` & `sphinx-versioning-0.0.2/sphinx_versioning/sphinx_versioning.py`

 * *Files identical despite different names*

### Comparing `sphinx-versioning-0.0.1/sphinx_versioning.egg-info/PKG-INFO` & `sphinx-versioning-0.0.2/sphinx_versioning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx-versioning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Sphinx extension to manage versioned documentation
-Home-page: https://github.com/Yihengxiong6/sphinx-versioning
+Home-page: https://github.com/Yihengxiong6/sphinx_versioning
 Author: Yiheng Xiong
 Author-email: georgex8866@gmail.com
 License: MIT
 Keywords: sphinx documentation versioning
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


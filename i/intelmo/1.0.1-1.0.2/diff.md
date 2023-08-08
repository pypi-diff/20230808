# Comparing `tmp/intelmo-1.0.1.tar.gz` & `tmp/intelmo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelmo-1.0.1.tar", last modified: Mon Aug  7 23:20:28 2023, max compression
+gzip compressed data, was "intelmo-1.0.2.tar", last modified: Mon Aug  7 23:39:34 2023, max compression
```

## Comparing `intelmo-1.0.1.tar` & `intelmo-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.564512 intelmo-1.0.1/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:20:28.564360 intelmo-1.0.1/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      376 2023-08-07 18:59:23.000000 intelmo-1.0.1/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.556784 intelmo-1.0.1/intelmo/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      218 2023-07-27 01:07:04.000000 intelmo-1.0.1/intelmo/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.559924 intelmo-1.0.1/intelmo/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6828 2023-08-05 20:52:12.000000 intelmo-1.0.1/intelmo/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 01:10:19.000000 intelmo-1.0.1/intelmo/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.561964 intelmo-1.0.1/intelmo/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      520 2023-08-03 23:26:35.000000 intelmo-1.0.1/intelmo/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2199 2023-07-29 22:24:21.000000 intelmo-1.0.1/intelmo/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 intelmo-1.0.1/intelmo/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1027 2023-08-07 21:56:20.000000 intelmo-1.0.1/intelmo/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5260 2023-08-05 20:51:38.000000 intelmo-1.0.1/intelmo/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1034 2023-07-29 20:32:23.000000 intelmo-1.0.1/intelmo/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.562940 intelmo-1.0.1/intelmo/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2579 2023-07-29 21:07:20.000000 intelmo-1.0.1/intelmo/types/model.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 intelmo-1.0.1/intelmo/types/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.563930 intelmo-1.0.1/intelmo/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.1/intelmo/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 01:11:10.000000 intelmo-1.0.1/intelmo/utils/extraction.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:20:28.559184 intelmo-1.0.1/intelmo.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      593 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        8 2023-08-07 23:20:28.000000 intelmo-1.0.1/intelmo.egg-info/top_level.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-08-07 23:20:28.564597 intelmo-1.0.1/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1327 2023-08-07 23:20:25.000000 intelmo-1.0.1/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.077908 intelmo-1.0.2/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:39:34.077766 intelmo-1.0.2/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      376 2023-08-07 18:59:23.000000 intelmo-1.0.2/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.072415 intelmo-1.0.2/intelmo/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      218 2023-07-27 01:07:04.000000 intelmo-1.0.2/intelmo/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.074288 intelmo-1.0.2/intelmo/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.2/intelmo/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6828 2023-08-05 20:52:12.000000 intelmo-1.0.2/intelmo/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 01:10:19.000000 intelmo-1.0.2/intelmo/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.076035 intelmo-1.0.2/intelmo/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.2/intelmo/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      520 2023-08-03 23:26:35.000000 intelmo-1.0.2/intelmo/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2199 2023-07-29 22:24:21.000000 intelmo-1.0.2/intelmo/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 intelmo-1.0.2/intelmo/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1027 2023-08-07 21:56:20.000000 intelmo-1.0.2/intelmo/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5260 2023-08-05 20:51:38.000000 intelmo-1.0.2/intelmo/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1034 2023-07-29 20:32:23.000000 intelmo-1.0.2/intelmo/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.077079 intelmo-1.0.2/intelmo/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.2/intelmo/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2579 2023-07-29 21:07:20.000000 intelmo-1.0.2/intelmo/types/model.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 intelmo-1.0.2/intelmo/types/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.077444 intelmo-1.0.2/intelmo/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 intelmo-1.0.2/intelmo/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 01:11:10.000000 intelmo-1.0.2/intelmo/utils/extraction.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-08-07 23:39:34.073476 intelmo-1.0.2/intelmo.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      661 2023-08-07 23:39:34.000000 intelmo-1.0.2/intelmo.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      593 2023-08-07 23:39:34.000000 intelmo-1.0.2/intelmo.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-08-07 23:39:34.000000 intelmo-1.0.2/intelmo.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-08-07 23:39:34.000000 intelmo-1.0.2/intelmo.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        8 2023-08-07 23:39:34.000000 intelmo-1.0.2/intelmo.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-08-07 23:39:34.077962 intelmo-1.0.2/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1004 2023-08-07 23:39:27.000000 intelmo-1.0.2/setup.py
```

### Comparing `intelmo-1.0.1/PKG-INFO` & `intelmo-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelmo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interface Toolkit for Extensive Language Models
 Author: Chunxu Yang
 Author-email: chunxuyang@ucla.edu
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `intelmo-1.0.1/intelmo/controllers/reader_controller.py` & `intelmo-1.0.2/intelmo/controllers/reader_controller.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/controllers/rss_controller.py` & `intelmo-1.0.2/intelmo/controllers/rss_controller.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/models/article.py` & `intelmo-1.0.2/intelmo/models/article.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/models/block.py` & `intelmo-1.0.2/intelmo/models/block.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/models/form.py` & `intelmo-1.0.2/intelmo/models/form.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/models/rss.py` & `intelmo-1.0.2/intelmo/models/rss.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/models/task.py` & `intelmo-1.0.2/intelmo/models/task.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/server.py` & `intelmo-1.0.2/intelmo/server.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/types/model.py` & `intelmo-1.0.2/intelmo/types/model.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo/utils/extraction.py` & `intelmo-1.0.2/intelmo/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/intelmo.egg-info/PKG-INFO` & `intelmo-1.0.2/intelmo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelmo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interface Toolkit for Extensive Language Models
 Author: Chunxu Yang
 Author-email: chunxuyang@ucla.edu
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `intelmo-1.0.1/intelmo.egg-info/SOURCES.txt` & `intelmo-1.0.2/intelmo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intelmo-1.0.1/setup.py` & `intelmo-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 from setuptools import find_packages
 from setuptools import setup
-from setuptools.command.install import install
-
-
-class PostInstallCommand(install):
-    """Post-installation for installation mode."""
-
-    def run(self):
-        install.run(self)
-        # Install nltk punkt
-        import nltk
-        nltk.download('punkt')
-
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
 print(find_packages(
     exclude=["examples", "tests", "docs"],
 ))
 
 
 setup(
     name='intelmo',
-    version='1.0.1',
+    version='1.0.2',
     description='Interface Toolkit for Extensive Language Models',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     # include_package_data=True,
     packages=find_packages(
         exclude=["examples", "tests"],
@@ -48,11 +36,8 @@
     ],
     license='MIT',
     platforms=["all"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
-    cmdclass={
-        'install': PostInstallCommand,
-    },
 )
```


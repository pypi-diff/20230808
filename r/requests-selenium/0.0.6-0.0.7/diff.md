# Comparing `tmp/requests_selenium-0.0.6.tar.gz` & `tmp/requests_selenium-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_selenium-0.0.6.tar", last modified: Sun Aug  6 15:45:41 2023, max compression
+gzip compressed data, was "requests_selenium-0.0.7.tar", last modified: Tue Aug  8 20:21:42 2023, max compression
```

## Comparing `requests_selenium-0.0.6.tar` & `requests_selenium-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 15:45:41.518606 requests_selenium-0.0.6/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 15:45:41.518430 requests_selenium-0.0.6/PKG-INFO
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 15:45:41.517232 requests_selenium-0.0.6/requests_selenium/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      464 2023-08-06 15:43:43.000000 requests_selenium-0.0.6/requests_selenium/__init__.py
--rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-06 15:38:26.000000 requests_selenium-0.0.6/requests_selenium/tempCodeRunnerFile.py
--rw-r--r--   0 benbavonese1   (502) staff       (20)      113 2023-08-06 15:44:52.000000 requests_selenium-0.0.6/requests_selenium/test2.py
--rw-r--r--   0 benbavonese1   (502) staff       (20)     1309 2023-08-03 16:22:41.000000 requests_selenium-0.0.6/requests_selenium/utils.py
-drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-06 15:45:41.518232 requests_selenium-0.0.6/requests_selenium.egg-info/
--rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-06 15:45:41.000000 requests_selenium-0.0.6/requests_selenium.egg-info/PKG-INFO
--rw-r--r--   0 benbavonese1   (502) staff       (20)      336 2023-08-06 15:45:41.000000 requests_selenium-0.0.6/requests_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-06 15:45:41.000000 requests_selenium-0.0.6/requests_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       60 2023-08-06 15:45:41.000000 requests_selenium-0.0.6/requests_selenium.egg-info/requires.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       18 2023-08-06 15:45:41.000000 requests_selenium-0.0.6/requests_selenium.egg-info/top_level.txt
--rw-r--r--   0 benbavonese1   (502) staff       (20)       38 2023-08-06 15:45:41.518677 requests_selenium-0.0.6/setup.cfg
--rw-r--r--   0 benbavonese1   (502) staff       (20)      918 2023-08-06 15:45:39.000000 requests_selenium-0.0.6/setup.py
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-08 20:21:42.934887 requests_selenium-0.0.7/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-08 20:21:42.934720 requests_selenium-0.0.7/PKG-INFO
+-rw-r--r--   0 benbavonese1   (502) staff       (20)     1804 2023-08-08 20:12:18.000000 requests_selenium-0.0.7/README.rst
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-08 20:21:42.933903 requests_selenium-0.0.7/requests_selenium/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      464 2023-08-06 15:43:43.000000 requests_selenium-0.0.7/requests_selenium/__init__.py
+-rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-06 15:38:26.000000 requests_selenium-0.0.7/requests_selenium/tempCodeRunnerFile.py
+-rw-r--r--   0 benbavonese1   (502) staff       (20)     1309 2023-08-03 16:22:41.000000 requests_selenium-0.0.7/requests_selenium/utils.py
+drwxr-xr-x   0 benbavonese1   (502) staff       (20)        0 2023-08-08 20:21:42.934544 requests_selenium-0.0.7/requests_selenium.egg-info/
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      679 2023-08-08 20:21:42.000000 requests_selenium-0.0.7/requests_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      320 2023-08-08 20:21:42.000000 requests_selenium-0.0.7/requests_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)        1 2023-08-08 20:21:42.000000 requests_selenium-0.0.7/requests_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       60 2023-08-08 20:21:42.000000 requests_selenium-0.0.7/requests_selenium.egg-info/requires.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       18 2023-08-08 20:21:42.000000 requests_selenium-0.0.7/requests_selenium.egg-info/top_level.txt
+-rw-r--r--   0 benbavonese1   (502) staff       (20)       38 2023-08-08 20:21:42.934932 requests_selenium-0.0.7/setup.cfg
+-rw-r--r--   0 benbavonese1   (502) staff       (20)      918 2023-08-08 20:21:01.000000 requests_selenium-0.0.7/setup.py
```

### Comparing `requests_selenium-0.0.6/PKG-INFO` & `requests_selenium-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests_selenium
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for fetching page source using Selenium
 Author: Ben Bavonese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `requests_selenium-0.0.6/requests_selenium/utils.py` & `requests_selenium-0.0.7/requests_selenium/utils.py`

 * *Files identical despite different names*

### Comparing `requests_selenium-0.0.6/requests_selenium.egg-info/PKG-INFO` & `requests_selenium-0.0.7/requests_selenium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-selenium
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for fetching page source using Selenium
 Author: Ben Bavonese
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `requests_selenium-0.0.6/setup.py` & `requests_selenium-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='requests_selenium',
-    version='0.0.6',
+    version='0.0.7',
     description='A Python package for fetching page source using Selenium',
     author='Ben Bavonese',
     packages=find_packages(), 
     install_requires=[
         'requests',
         'beautifulsoup4',
         'chromedriver_autoinstaller',
```


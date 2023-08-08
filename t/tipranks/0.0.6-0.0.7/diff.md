# Comparing `tmp/tipranks-0.0.6.tar.gz` & `tmp/tipranks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipranks-0.0.6.tar", last modified: Tue Sep 27 00:23:54 2022, max compression
+gzip compressed data, was "tipranks-0.0.7.tar", last modified: Tue Aug  8 17:47:19 2023, max compression
```

## Comparing `tipranks-0.0.6.tar` & `tipranks-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:23:54.423287 tipranks-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-27 00:23:44.000000 tipranks-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-09-27 00:23:54.423287 tipranks-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-09-27 00:23:44.000000 tipranks-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 00:23:54.423287 tipranks-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-27 00:23:44.000000 tipranks-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:23:54.423287 tipranks-0.0.6/tipranks/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-27 00:23:44.000000 tipranks-0.0.6/tipranks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-09-27 00:23:44.000000 tipranks-0.0.6/tipranks/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-27 00:23:44.000000 tipranks-0.0.6/tipranks/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 00:23:54.423287 tipranks-0.0.6/tipranks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-09-27 00:23:54.000000 tipranks-0.0.6/tipranks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-27 00:23:54.000000 tipranks-0.0.6/tipranks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 00:23:54.000000 tipranks-0.0.6/tipranks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-27 00:23:54.000000 tipranks-0.0.6/tipranks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-27 00:23:54.000000 tipranks-0.0.6/tipranks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:47:19.393609 tipranks-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-08 17:47:07.000000 tipranks-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-08 17:47:19.393609 tipranks-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 17:47:07.000000 tipranks-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:47:19.393609 tipranks-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-08 17:47:07.000000 tipranks-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:47:19.393609 tipranks-0.0.7/tipranks/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 17:47:07.000000 tipranks-0.0.7/tipranks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-08 17:47:07.000000 tipranks-0.0.7/tipranks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 17:47:07.000000 tipranks-0.0.7/tipranks/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:47:19.393609 tipranks-0.0.7/tipranks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-08 17:47:19.000000 tipranks-0.0.7/tipranks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-08 17:47:19.000000 tipranks-0.0.7/tipranks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:47:19.000000 tipranks-0.0.7/tipranks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 17:47:19.000000 tipranks-0.0.7/tipranks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 17:47:19.000000 tipranks-0.0.7/tipranks.egg-info/top_level.txt
```

### Comparing `tipranks-0.0.6/LICENSE` & `tipranks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tipranks-0.0.6/PKG-INFO` & `tipranks-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipranks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python interface to communicate with TipRanks API.
 Home-page: UNKNOWN
 Author: visuxls
 License: UNKNOWN
 Description: # TipRanks
         
         Python module to interact with TipRanks API.
```

### Comparing `tipranks-0.0.6/README.md` & `tipranks-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tipranks-0.0.6/setup.py` & `tipranks-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="tipranks",
-	version="0.0.6",
+	version="0.0.7",
 	author="visuxls",
 	description="Python interface to communicate with TipRanks API.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
```

### Comparing `tipranks-0.0.6/tipranks/base.py` & `tipranks-0.0.7/tipranks/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from errors import (
+from .errors import (
 	TipRanksStatusCodeError,
 	TipRanksArgumentError,
 	TipRanksRequestError
 )
 from typing import Optional, Any
 import requests
 import time
```

### Comparing `tipranks-0.0.6/tipranks.egg-info/PKG-INFO` & `tipranks-0.0.7/tipranks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipranks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python interface to communicate with TipRanks API.
 Home-page: UNKNOWN
 Author: visuxls
 License: UNKNOWN
 Description: # TipRanks
         
         Python module to interact with TipRanks API.
```


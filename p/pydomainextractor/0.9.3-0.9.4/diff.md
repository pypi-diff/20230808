# Comparing `tmp/PyDomainExtractor-0.9.3.tar.gz` & `tmp/PyDomainExtractor-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDomainExtractor-0.9.3.tar", last modified: Tue Jan 25 12:35:33 2022, max compression
+gzip compressed data, was "PyDomainExtractor-0.9.4.tar", last modified: Tue Jan 25 14:29:38 2022, max compression
```

## Comparing `PyDomainExtractor-0.9.3.tar` & `PyDomainExtractor-0.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.165628 PyDomainExtractor-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-01-25 12:35:33.165628 PyDomainExtractor-0.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.161628 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-01-25 12:35:33.000000 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-01-25 12:35:33.000000 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 12:35:33.000000 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 12:35:33.000000 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-25 12:35:33.000000 PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.161628 PyDomainExtractor-0.9.3/images/
--rw-r--r--   0 runner    (1001) docker     (121)    20408 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.161628 PyDomainExtractor-0.9.3/pydomainextractor/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/pydomainextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/pydomainextractor/pydomainextractor.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-25 12:35:33.165628 PyDomainExtractor-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.161628 PyDomainExtractor-0.9.3/src/
--rw-r--r--   0 runner    (1001) docker     (121)    19495 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/src/extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (121)   237091 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/src/public_suffix_list.h
--rw-r--r--   0 runner    (1001) docker     (121)    94949 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/src/robin_hood.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:33.161628 PyDomainExtractor-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26687 2022-01-25 12:35:30.000000 PyDomainExtractor-0.9.3/tests/test_pydomainextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6283 2022-01-25 14:29:38.000000 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-01-25 14:29:38.000000 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 14:29:38.000000 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 14:29:38.000000 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-01-25 14:29:38.000000 PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    20408 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/pydomainextractor/
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/pydomainextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/pydomainextractor/pydomainextractor.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/src/
+-rw-r--r--   0 runner    (1001) docker     (121)    19495 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/src/extractor.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)   237091 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/src/public_suffix_list.h
+-rw-r--r--   0 runner    (1001) docker     (121)    94949 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/src/robin_hood.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:38.439467 PyDomainExtractor-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26687 2022-01-25 14:29:32.000000 PyDomainExtractor-0.9.4/tests/test_pydomainextractor.py
```

### Comparing `PyDomainExtractor-0.9.3/LICENSE` & `PyDomainExtractor-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/PKG-INFO` & `PyDomainExtractor-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDomainExtractor
-Version: 0.9.3
+Version: 0.9.4
 Summary: Highly optimized Domain Name Extraction library written in C++
 Home-page: https://github.com/Intsights/PyDomainExtractor
 Author: Gal Ben David
 Author-email: gal@intsights.com
 License: MIT
 Project-URL: Source, https://github.com/Intsights/PyDomainExtractor
 Keywords: domain extraction tld suffix psl c++
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDomainExtractor Version: 0.9.3 Summary: Highly
+Metadata-Version: 2.1 Name: PyDomainExtractor Version: 0.9.4 Summary: Highly
 optimized Domain Name Extraction library written in C++ Home-page: https://
 github.com/Intsights/PyDomainExtractor Author: Gal Ben David Author-email:
 gal@intsights.com License: MIT Project-URL: Source, https://github.com/
 Intsights/PyDomainExtractor Keywords: domain extraction tld suffix psl c++
 Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyDomainExtractor-0.9.3/PyDomainExtractor.egg-info/PKG-INFO` & `PyDomainExtractor-0.9.4/PyDomainExtractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDomainExtractor
-Version: 0.9.3
+Version: 0.9.4
 Summary: Highly optimized Domain Name Extraction library written in C++
 Home-page: https://github.com/Intsights/PyDomainExtractor
 Author: Gal Ben David
 Author-email: gal@intsights.com
 License: MIT
 Project-URL: Source, https://github.com/Intsights/PyDomainExtractor
 Keywords: domain extraction tld suffix psl c++
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyDomainExtractor Version: 0.9.3 Summary: Highly
+Metadata-Version: 2.1 Name: PyDomainExtractor Version: 0.9.4 Summary: Highly
 optimized Domain Name Extraction library written in C++ Home-page: https://
 github.com/Intsights/PyDomainExtractor Author: Gal Ben David Author-email:
 gal@intsights.com License: MIT Project-URL: Source, https://github.com/
 Intsights/PyDomainExtractor Keywords: domain extraction tld suffix psl c++
 Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `PyDomainExtractor-0.9.3/README.md` & `PyDomainExtractor-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/images/logo.png` & `PyDomainExtractor-0.9.4/images/logo.png`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/pydomainextractor/__init__.py` & `PyDomainExtractor-0.9.4/pydomainextractor/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/setup.py` & `PyDomainExtractor-0.9.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import os
 import glob
 
 
 setuptools.setup(
     name='PyDomainExtractor',
-    version='0.9.3',
+    version='0.9.4',
     author='Gal Ben David',
     author_email='gal@intsights.com',
     url='https://github.com/Intsights/PyDomainExtractor',
     project_urls={
         'Source': 'https://github.com/Intsights/PyDomainExtractor',
     },
     license='MIT',
@@ -42,15 +42,15 @@
             ),
             language='c++',
             extra_compile_args=[
                 '-std=c++17',
             ],
             extra_link_args=[
                 '-lidn2',
-                '-Wl,--strip-all',
+                '-Wl,-s',
             ],
             include_dirs=[
                 'src',
             ]
         ),
     ],
 )
```

### Comparing `PyDomainExtractor-0.9.3/src/extractor.cpp` & `PyDomainExtractor-0.9.4/src/extractor.cpp`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/src/public_suffix_list.h` & `PyDomainExtractor-0.9.4/src/public_suffix_list.h`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/src/robin_hood.h` & `PyDomainExtractor-0.9.4/src/robin_hood.h`

 * *Files identical despite different names*

### Comparing `PyDomainExtractor-0.9.3/tests/test_pydomainextractor.py` & `PyDomainExtractor-0.9.4/tests/test_pydomainextractor.py`

 * *Files identical despite different names*


# Comparing `tmp/mriphysio-2023.4.10.tar.gz` & `tmp/mriphysio-2023.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mriphysio-2023.4.10.tar", last modified: Mon Apr 10 15:00:42 2023, max compression
+gzip compressed data, was "mriphysio-2023.8.8.tar", last modified: Tue Aug  8 19:16:25 2023, max compression
```

## Comparing `mriphysio-2023.4.10.tar` & `mriphysio-2023.8.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-04-10 15:00:42.720064 mriphysio-2023.4.10/
--rw-r--r--   0 jmt        (501) staff       (20)     1104 2022-12-20 23:58:31.000000 mriphysio-2023.4.10/LICENSE
--rw-r--r--   0 jmt        (501) staff       (20)     1327 2023-04-10 15:00:42.719769 mriphysio-2023.4.10/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      545 2022-12-20 23:58:31.000000 mriphysio-2023.4.10/README.md
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-04-10 15:00:42.717002 mriphysio-2023.4.10/mriphysio/
--rw-r--r--   0 jmt        (501) staff       (20)       63 2022-12-20 23:58:31.000000 mriphysio-2023.4.10/mriphysio/__init__.py
--rw-r--r--   0 jmt        (501) staff       (20)     6190 2023-04-10 14:05:10.000000 mriphysio-2023.4.10/mriphysio/ecg.py
--rwxr-xr-x   0 jmt        (501) staff       (20)     2944 2023-04-10 14:50:36.000000 mriphysio-2023.4.10/mriphysio/physio2bids.py
--rw-r--r--   0 jmt        (501) staff       (20)    14554 2023-04-10 14:49:34.000000 mriphysio-2023.4.10/mriphysio/physiodicom.py
-drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-04-10 15:00:42.719217 mriphysio-2023.4.10/mriphysio.egg-info/
--rw-r--r--   0 jmt        (501) staff       (20)     1327 2023-04-10 15:00:42.000000 mriphysio-2023.4.10/mriphysio.egg-info/PKG-INFO
--rw-r--r--   0 jmt        (501) staff       (20)      315 2023-04-10 15:00:42.000000 mriphysio-2023.4.10/mriphysio.egg-info/SOURCES.txt
--rw-r--r--   0 jmt        (501) staff       (20)        1 2023-04-10 15:00:42.000000 mriphysio-2023.4.10/mriphysio.egg-info/dependency_links.txt
--rw-r--r--   0 jmt        (501) staff       (20)       59 2023-04-10 15:00:42.000000 mriphysio-2023.4.10/mriphysio.egg-info/entry_points.txt
--rw-r--r--   0 jmt        (501) staff       (20)        1 2022-12-20 23:58:31.000000 mriphysio-2023.4.10/mriphysio.egg-info/not-zip-safe
--rw-r--r--   0 jmt        (501) staff       (20)       10 2023-04-10 15:00:42.000000 mriphysio-2023.4.10/mriphysio.egg-info/top_level.txt
--rw-r--r--   0 jmt        (501) staff       (20)       38 2023-04-10 15:00:42.720145 mriphysio-2023.4.10/setup.cfg
--rw-r--r--   0 jmt        (501) staff       (20)     8652 2023-04-10 14:58:50.000000 mriphysio-2023.4.10/setup.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-08-08 19:16:25.904979 mriphysio-2023.8.8/
+-rw-r--r--   0 jmt        (501) staff       (20)     1104 2022-12-13 20:32:48.000000 mriphysio-2023.8.8/LICENSE
+-rw-r--r--   0 jmt        (501) staff       (20)     1376 2023-08-08 19:16:25.904650 mriphysio-2023.8.8/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      545 2022-12-13 20:32:48.000000 mriphysio-2023.8.8/README.md
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-08-08 19:16:25.902310 mriphysio-2023.8.8/mriphysio/
+-rw-r--r--   0 jmt        (501) staff       (20)       63 2023-03-08 00:41:41.000000 mriphysio-2023.8.8/mriphysio/__init__.py
+-rw-r--r--   0 jmt        (501) staff       (20)     6190 2023-08-08 19:15:36.000000 mriphysio-2023.8.8/mriphysio/ecg.py
+-rwxr-xr-x   0 jmt        (501) staff       (20)     2944 2023-08-08 19:15:36.000000 mriphysio-2023.8.8/mriphysio/physio2bids.py
+-rw-r--r--   0 jmt        (501) staff       (20)    14554 2023-08-08 19:15:36.000000 mriphysio-2023.8.8/mriphysio/physiodicom.py
+drwxr-xr-x   0 jmt        (501) staff       (20)        0 2023-08-08 19:16:25.904167 mriphysio-2023.8.8/mriphysio.egg-info/
+-rw-r--r--   0 jmt        (501) staff       (20)     1376 2023-08-08 19:16:25.000000 mriphysio-2023.8.8/mriphysio.egg-info/PKG-INFO
+-rw-r--r--   0 jmt        (501) staff       (20)      315 2023-08-08 19:16:25.000000 mriphysio-2023.8.8/mriphysio.egg-info/SOURCES.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        1 2023-08-08 19:16:25.000000 mriphysio-2023.8.8/mriphysio.egg-info/dependency_links.txt
+-rw-r--r--   0 jmt        (501) staff       (20)       59 2023-08-08 19:16:25.000000 mriphysio-2023.8.8/mriphysio.egg-info/entry_points.txt
+-rw-r--r--   0 jmt        (501) staff       (20)        1 2022-12-14 23:49:35.000000 mriphysio-2023.8.8/mriphysio.egg-info/not-zip-safe
+-rw-r--r--   0 jmt        (501) staff       (20)       10 2023-08-08 19:16:25.000000 mriphysio-2023.8.8/mriphysio.egg-info/top_level.txt
+-rw-r--r--   0 jmt        (501) staff       (20)       38 2023-08-08 19:16:25.905121 mriphysio-2023.8.8/setup.cfg
+-rw-r--r--   0 jmt        (501) staff       (20)     8700 2023-08-08 19:15:46.000000 mriphysio-2023.8.8/setup.py
```

### Comparing `mriphysio-2023.4.10/LICENSE` & `mriphysio-2023.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mriphysio-2023.4.10/PKG-INFO` & `mriphysio-2023.8.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mriphysio
-Version: 2023.4.10
+Version: 2023.8.8
 Summary: Siemens physiology DICOM and MPCU log conversion
 Home-page: https://github.com/jmtyszka/mriphysio
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/thermalfit/issues
 Project-URL: Funding, http://cbic.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/thermalfit/
 Keywords: Siemens CMRR physiology conversion MRI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mriphysio
 MRI physiological DICOM and MPCU log handling functions
```

### Comparing `mriphysio-2023.4.10/README.md` & `mriphysio-2023.8.8/README.md`

 * *Files identical despite different names*

### Comparing `mriphysio-2023.4.10/mriphysio/ecg.py` & `mriphysio-2023.8.8/mriphysio/ecg.py`

 * *Files identical despite different names*

### Comparing `mriphysio-2023.4.10/mriphysio/physio2bids.py` & `mriphysio-2023.8.8/mriphysio/physio2bids.py`

 * *Files identical despite different names*

### Comparing `mriphysio-2023.4.10/mriphysio/physiodicom.py` & `mriphysio-2023.8.8/mriphysio/physiodicom.py`

 * *Files identical despite different names*

### Comparing `mriphysio-2023.4.10/mriphysio.egg-info/PKG-INFO` & `mriphysio-2023.8.8/mriphysio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mriphysio
-Version: 2023.4.10
+Version: 2023.8.8
 Summary: Siemens physiology DICOM and MPCU log conversion
 Home-page: https://github.com/jmtyszka/mriphysio
 Author: Julian Michael Tyszka
 Author-email: jmt@caltech.edu
 Project-URL: Bug Reports, https://github.com/jmtyszka/thermalfit/issues
 Project-URL: Funding, http://cbic.caltech.edu/
 Project-URL: Source, https://github.com/jmtyszka/thermalfit/
 Keywords: Siemens CMRR physiology conversion MRI
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mriphysio
 MRI physiological DICOM and MPCU log handling functions
```

### Comparing `mriphysio-2023.4.10/setup.py` & `mriphysio-2023.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2023.4.10',  # Required
+    version='2023.8.8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Siemens physiology DICOM and MPCU log conversion',  # Optional
 
     # This is an optional longer description of your project that represents
@@ -105,14 +105,15 @@
         # Pick your license as you wish
         'License :: OSI Approved :: MIT License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         # These classifiers are *not* checked by 'pip install'. See instead
         # 'python_requires' below.
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
```


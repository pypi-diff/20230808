# Comparing `tmp/BIDSit-0.0.8.tar.gz` & `tmp/BIDSit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.8.tar", last modified: Mon Jul 31 22:55:34 2023, max compression
+gzip compressed data, was "BIDSit-0.0.9.tar", last modified: Mon Jul 31 22:58:38 2023, max compression
```

## Comparing `BIDSit-0.0.8.tar` & `BIDSit-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:55:34.153636 BIDSit-0.0.8/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:55:34.153178 BIDSit-0.0.8/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.8/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:55:34.153783 BIDSit-0.0.8/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.8/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:55:34.146410 BIDSit-0.0.8/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:55:34.150376 BIDSit-0.0.8/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.8/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.8/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)       85 2023-07-31 22:54:09.000000 BIDSit-0.0.8/src/BIDSit/__main__.py
--rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.8/src/BIDSit/dicom_to_bids2.py
--rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 21:09:49.000000 BIDSit-0.0.8/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 22:52:59.000000 BIDSit-0.0.8/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:55:34.152616 BIDSit-0.0.8/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:55:34.000000 BIDSit-0.0.8/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      328 2023-07-31 22:55:34.000000 BIDSit-0.0.8/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:55:34.000000 BIDSit-0.0.8/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:55:34.000000 BIDSit-0.0.8/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:55:34.000000 BIDSit-0.0.8/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.179807 BIDSit-0.0.9/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:58:38.179470 BIDSit-0.0.9/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.9/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:58:38.179923 BIDSit-0.0.9/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.9/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.173698 BIDSit-0.0.9/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.176659 BIDSit-0.0.9/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.9/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.9/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)       87 2023-07-31 22:57:25.000000 BIDSit-0.0.9/src/BIDSit/__main__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.9/src/BIDSit/dicom_to_bids2.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 22:57:05.000000 BIDSit-0.0.9/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 22:57:44.000000 BIDSit-0.0.9/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.178948 BIDSit-0.0.9/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      328 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.8/PKG-INFO` & `BIDSit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BIDSit-0.0.8/README.rst` & `BIDSit-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.8/setup.py` & `BIDSit-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.8/src/BIDSit/Test_script.py` & `BIDSit-0.0.9/src/BIDSit/Test_script.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.8/src/BIDSit/dicom_to_bids2.py` & `BIDSit-0.0.9/src/BIDSit/dicom_to_bids2.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.8/src/BIDSit/go.py` & `BIDSit-0.0.9/src/BIDSit/go.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import filecmp
 import glob
 import shutil
 import json
 import errno
 
 
-def main():
+def DOit():
     # - get user input - #
     sg.theme('GreenTan')
     user_info = start_gui()
     
     # - define variables in use - #
     in_dir = user_info['in_dir'] # in_dir is where the input files are
     out_dir = user_info['out_dir'] # out_dir is where the output files will go
@@ -1347,8 +1347,8 @@
         shutil.copytree(src, dst)
     except OSError as exc:
         if exc.errno in (errno.ENOTDIR, errno.EINVAL):
             shutil.copy(src, dst)
         else: raise
     
 if __name__ == '__main__':
-    main()
+    DOit()
```

### Comparing `BIDSit-0.0.8/src/BIDSit/version.py` & `BIDSit-0.0.9/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `BIDSit-0.0.8/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.9/src/BIDSit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.8
+Version: 0.0.9
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```


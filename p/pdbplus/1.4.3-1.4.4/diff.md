# Comparing `tmp/pdbplus-1.4.3.tar.gz` & `tmp/pdbplus-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.4.3.tar", last modified: Mon Jul 17 22:28:50 2023, max compression
+gzip compressed data, was "pdbplus-1.4.4.tar", last modified: Tue Aug  8 18:56:44 2023, max compression
```

## Comparing `pdbplus-1.4.3.tar` & `pdbplus-1.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:28:50.990539 pdbplus-1.4.3/
--rw-r--r--   0 michael    (501) staff       (20)     7195 2023-07-17 22:28:50.990428 pdbplus-1.4.3/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     5242 2023-07-17 22:14:22.000000 pdbplus-1.4.3/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:28:50.990275 pdbplus-1.4.3/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     7195 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:28:50.000000 pdbplus-1.4.3/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-17 22:28:50.990575 pdbplus-1.4.3/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5607 2023-07-17 22:12:51.000000 pdbplus-1.4.3/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-08 18:56:44.946903 pdbplus-1.4.4/
+-rw-r--r--   0 michael    (501) staff       (20)     7246 2023-08-08 18:56:44.946799 pdbplus-1.4.4/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     5242 2023-07-17 22:14:22.000000 pdbplus-1.4.4/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-08 18:56:44.946650 pdbplus-1.4.4/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     7246 2023-08-08 18:56:44.000000 pdbplus-1.4.4/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-08-08 18:56:44.000000 pdbplus-1.4.4/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-08-08 18:56:44.000000 pdbplus-1.4.4/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-08-08 18:56:44.000000 pdbplus-1.4.4/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-08-08 18:56:44.000000 pdbplus-1.4.4/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-08-08 18:56:44.946935 pdbplus-1.4.4/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5657 2023-08-08 17:13:12.000000 pdbplus-1.4.4/setup.py
```

### Comparing `pdbplus-1.4.3/PKG-INFO` & `pdbplus-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.3
+Version: 1.4.4
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
```

### Comparing `pdbplus-1.4.3/README.md` & `pdbplus-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pdbplus-1.4.3/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.4.4/pdbplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.4.3
+Version: 1.4.4
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
```

### Comparing `pdbplus-1.4.3/setup.py` & `pdbplus-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     reply = str(input_method(
         '>>> Confirm release PUBLISH to PyPI? (yes/no): ')).lower().strip()
     if reply == 'yes':
         if sys.version_info < (3, 9):
             print("\nERROR! Publishing to PyPI requires Python>=3.9")
             sys.exit()
         print("\n*** Checking code health with flake8:\n")
-        os.system("python -m pip install 'flake8==6.0.0'")
+        os.system("python -m pip install 'flake8==6.1.0'")
         flake8_status = os.system("flake8 --exclude=.eggs,temp")
         if flake8_status != 0:
             print("\nERROR! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
@@ -64,15 +64,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.4.3',
+    version='1.4.4',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -99,26 +99,27 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Topic :: Software Development :: Debuggers",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
     python_requires=">=3.6",
     install_requires=[
-        'pdbp>=1.4.3',
+        'pdbp>=1.4.4',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```


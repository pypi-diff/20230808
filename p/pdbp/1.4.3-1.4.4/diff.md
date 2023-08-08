# Comparing `tmp/pdbp-1.4.3.tar.gz` & `tmp/pdbp-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.4.3.tar", last modified: Mon Jul 17 22:27:07 2023, max compression
+gzip compressed data, was "pdbp-1.4.4.tar", last modified: Tue Aug  8 18:51:23 2023, max compression
```

## Comparing `pdbp-1.4.3.tar` & `pdbp-1.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104875 pdbp-1.4.3/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.3/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.3/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.3/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.3/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.3/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6964 2023-07-17 22:27:07.104927 pdbp-1.4.3/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4948 2023-07-17 22:26:34.000000 pdbp-1.4.3/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.3/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-07-17 22:27:07.105103 pdbp-1.4.3/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5954 2023-07-17 22:26:34.000000 pdbp-1.4.3/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104149 pdbp-1.4.3/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.3/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-17 22:27:07.104755 pdbp-1.4.3/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6964 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      109 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-17 22:27:07.000000 pdbp-1.4.3/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    57871 2023-07-17 22:26:34.000000 pdbp-1.4.3/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-08 18:51:23.932467 pdbp-1.4.4/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.4/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.4/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.4/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.4/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.4/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     7015 2023-08-08 18:51:23.932518 pdbp-1.4.4/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4948 2023-07-17 22:26:34.000000 pdbp-1.4.4/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.4/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-08-08 18:51:23.932676 pdbp-1.4.4/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     6004 2023-08-08 18:50:45.000000 pdbp-1.4.4/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-08 18:51:23.931806 pdbp-1.4.4/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.4/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-08-08 18:51:23.932374 pdbp-1.4.4/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     7015 2023-08-08 18:51:23.000000 pdbp-1.4.4/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-08-08 18:51:23.000000 pdbp-1.4.4/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-08-08 18:51:23.000000 pdbp-1.4.4/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      109 2023-08-08 18:51:23.000000 pdbp-1.4.4/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-08-08 18:51:23.000000 pdbp-1.4.4/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    57871 2023-07-17 22:26:34.000000 pdbp-1.4.4/src/pdbp.py
```

### Comparing `pdbp-1.4.3/.gitignore` & `pdbp-1.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.3/CODE_OF_CONDUCT.md` & `pdbp-1.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.3/CONTRIBUTING.md` & `pdbp-1.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.3/LICENSE` & `pdbp-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.3/PKG-INFO` & `pdbp-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.3
+Version: 1.4.4
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -29,14 +29,15 @@
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

### Comparing `pdbp-1.4.3/README.md` & `pdbp-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.4.3/setup.py` & `pdbp-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     confirm_text = ">>> Confirm release PUBLISH to PyPI? (yes/no): "
     reply = str(input_method(confirm_text)).lower().strip()
     if reply == "yes":
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
@@ -67,15 +67,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.4.3",
+    version="1.4.4",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
@@ -105,28 +105,29 @@
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
         'pygments>=2.14.0;python_version<"3.7"',
-        'pygments>=2.15.1;python_version>="3.7"',
+        'pygments>=2.16.1;python_version>="3.7"',
         "tabcompleter>=1.2.1",
     ],
     setup_requires=[],
     include_package_data=True,
 )
 
 print("\n*** pdbp (Pdb+) Installation Complete! ***\n")
```

### Comparing `pdbp-1.4.3/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.4.4/src/pdbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.4.3
+Version: 1.4.4
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -29,14 +29,15 @@
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

### Comparing `pdbp-1.4.3/src/pdbp.py` & `pdbp-1.4.4/src/pdbp.py`

 * *Files identical despite different names*


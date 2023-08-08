# Comparing `tmp/pytest_deduplicate-0.1.3.tar.gz` & `tmp/pytest_deduplicate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_deduplicate-0.1.3.tar", last modified: Mon Aug  7 21:27:59 2023, max compression
+gzip compressed data, was "pytest_deduplicate-0.1.4.tar", last modified: Tue Aug  8 19:16:32 2023, max compression
```

## Comparing `pytest_deduplicate-0.1.3.tar` & `pytest_deduplicate-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-07 21:27:59.926736 pytest_deduplicate-0.1.3/
--rw-rw-r--   0 xor       (1000) xor       (1000)    35149 2023-08-06 12:07:32.000000 pytest_deduplicate-0.1.3/LICENSE
--rw-rw-r--   0 xor       (1000) xor       (1000)     2055 2023-08-07 21:27:59.926736 pytest_deduplicate-0.1.3/PKG-INFO
--rw-rw-r--   0 xor       (1000) xor       (1000)     1291 2023-08-07 20:57:45.000000 pytest_deduplicate-0.1.3/README.md
--rw-rw-r--   0 xor       (1000) xor       (1000)     1051 2023-08-07 21:27:37.000000 pytest_deduplicate-0.1.3/pyproject.toml
-drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-07 21:27:59.922737 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/
--rw-rw-r--   0 xor       (1000) xor       (1000)     2055 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/PKG-INFO
--rw-rw-r--   0 xor       (1000) xor       (1000)      308 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/SOURCES.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)        1 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/dependency_links.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)       63 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/entry_points.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)       16 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/requires.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)       19 2023-08-07 21:27:59.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/top_level.txt
--rw-rw-r--   0 xor       (1000) xor       (1000)     4814 2023-08-07 21:27:37.000000 pytest_deduplicate-0.1.3/pytest_deduplicate.py
--rw-rw-r--   0 xor       (1000) xor       (1000)       38 2023-08-07 21:27:59.926736 pytest_deduplicate-0.1.3/setup.cfg
+drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-08 19:16:32.372176 pytest_deduplicate-0.1.4/
+-rw-rw-r--   0 xor       (1000) xor       (1000)    35149 2023-08-06 12:07:32.000000 pytest_deduplicate-0.1.4/LICENSE
+-rw-rw-r--   0 xor       (1000) xor       (1000)     2226 2023-08-08 19:16:32.372176 pytest_deduplicate-0.1.4/PKG-INFO
+-rw-rw-r--   0 xor       (1000) xor       (1000)     1291 2023-08-07 20:57:45.000000 pytest_deduplicate-0.1.4/README.md
+-rw-rw-r--   0 xor       (1000) xor       (1000)     1206 2023-08-08 19:15:49.000000 pytest_deduplicate-0.1.4/pyproject.toml
+drwxrwxr-x   0 xor       (1000) xor       (1000)        0 2023-08-08 19:16:32.372176 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/
+-rw-rw-r--   0 xor       (1000) xor       (1000)     2226 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/PKG-INFO
+-rw-rw-r--   0 xor       (1000) xor       (1000)      308 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/SOURCES.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)        1 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/dependency_links.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)       63 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/entry_points.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)       16 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/requires.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)       19 2023-08-08 19:16:32.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/top_level.txt
+-rw-rw-r--   0 xor       (1000) xor       (1000)     4814 2023-08-07 21:27:37.000000 pytest_deduplicate-0.1.4/pytest_deduplicate.py
+-rw-rw-r--   0 xor       (1000) xor       (1000)       38 2023-08-08 19:16:32.372176 pytest_deduplicate-0.1.4/setup.cfg
```

### Comparing `pytest_deduplicate-0.1.3/LICENSE` & `pytest_deduplicate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_deduplicate-0.1.3/PKG-INFO` & `pytest_deduplicate-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest_deduplicate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Identifies duplicate unit tests
 Author-email: xor2003 <xor2003@gmx.com>
 License: GPL
 Project-URL: Homepage, https://github.com/xor2003/pytest_deduplicate
 Keywords: pytest,deduplicate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Testing :: Unit
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest_deduplicate
 
 The pytest_deduplicate is designed to identify duplicate or superseeding unit tests that have the same or bigger code coverage.
```

### Comparing `pytest_deduplicate-0.1.3/README.md` & `pytest_deduplicate-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytest_deduplicate-0.1.3/pyproject.toml` & `pytest_deduplicate-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest_deduplicate"
-version = "0.1.3"
+version = "0.1.4"
 description = "Identifies duplicate unit tests"
 authors = [
     {name = "xor2003", email = "xor2003@gmx.com"},
 ]
 dependencies = ["pytest","coverage"]
 requires-python = ">=3.8"
 readme = "README.md"
@@ -19,14 +19,17 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Topic :: Software Development :: Testing :: Unit",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Quality Assurance"
 ]
 
 [project.urls]
 Homepage = "https://github.com/xor2003/pytest_deduplicate"
 
 [tool.distutils.egg_info]
 tag-build = ""
```

### Comparing `pytest_deduplicate-0.1.3/pytest_deduplicate.egg-info/PKG-INFO` & `pytest_deduplicate-0.1.4/pytest_deduplicate.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-deduplicate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Identifies duplicate unit tests
 Author-email: xor2003 <xor2003@gmx.com>
 License: GPL
 Project-URL: Homepage, https://github.com/xor2003/pytest_deduplicate
 Keywords: pytest,deduplicate
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Testing :: Unit
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest_deduplicate
 
 The pytest_deduplicate is designed to identify duplicate or superseeding unit tests that have the same or bigger code coverage.
```

### Comparing `pytest_deduplicate-0.1.3/pytest_deduplicate.py` & `pytest_deduplicate-0.1.4/pytest_deduplicate.py`

 * *Files identical despite different names*


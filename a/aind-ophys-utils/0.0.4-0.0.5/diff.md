# Comparing `tmp/aind-ophys-utils-0.0.4.tar.gz` & `tmp/aind-ophys-utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-ophys-utils-0.0.4.tar", last modified: Tue Aug  8 15:58:05 2023, max compression
+gzip compressed data, was "aind-ophys-utils-0.0.5.tar", last modified: Tue Aug  8 16:17:20 2023, max compression
```

## Comparing `aind-ophys-utils-0.0.4.tar` & `aind-ophys-utils-0.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.318275 aind-ophys-utils-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.322275 aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.322275 aind-ophys-utils-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.322275 aind-ophys-utils-0.0.4/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.322275 aind-ophys-utils-0.0.4/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.322275 aind-ophys-utils-0.0.4/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.318275 aind-ophys-utils-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/src/aind_ophys_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 15:57:42.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils/array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils/video_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-08 15:58:05.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 15:58:05.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:58:05.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 15:58:05.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 15:58:05.000000 aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:58:05.326275 aind-ophys-utils-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/tests/test_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-08 15:57:41.000000 aind-ophys-utils-0.0.4/tests/test_video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.899362 aind-ophys-utils-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.891362 aind-ophys-utils-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.891362 aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.891362 aind-ophys-utils-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-08-08 16:17:20.899362 aind-ophys-utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.895362 aind-ophys-utils-0.0.5/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.895362 aind-ophys-utils-0.0.5/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.895362 aind-ophys-utils-0.0.5/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:17:20.899362 aind-ophys-utils-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.891362 aind-ophys-utils-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.895362 aind-ophys-utils-0.0.5/src/aind_ophys_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 16:17:03.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils/array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils/video_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.895362 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-08-08 16:17:20.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-08 16:17:20.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:17:20.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 16:17:20.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 16:17:20.000000 aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:17:20.899362 aind-ophys-utils-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/tests/test_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-08-08 16:17:02.000000 aind-ophys-utils-0.0.5/tests/test_video_utils.py
```

### Comparing `aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/.github/ISSUE_TEMPLATE/user-story.md` & `aind-ophys-utils-0.0.5/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/.github/workflows/tag_and_publish.yml` & `aind-ophys-utils-0.0.5/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/.github/workflows/test_and_lint.yml` & `aind-ophys-utils-0.0.5/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/.gitignore` & `aind-ophys-utils-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/LICENSE` & `aind-ophys-utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/PKG-INFO` & `aind-ophys-utils-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ophys-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -19,15 +19,17 @@
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.7-blue?logo=python)
 
 This repository contains python utility methods for processing optical physiology data. Methods in this repository have simple, standard data interfaces and are generally applicable to optical physiology data. As much as possible think arrays and dataframes rather than complex project-specific data structures. 
 
 ## Installation
 
-`pip install aind-ophys-utils`
+```bash
+pip install aind-ophys-utils
+```
 
 To use the software from source, clone the repository and in the root directory run
 ```bash
 pip install -e .
 ```
 
 To develop the code in place, run
```

### Comparing `aind-ophys-utils-0.0.4/README.md` & `aind-ophys-utils-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.7-blue?logo=python)
 
 This repository contains python utility methods for processing optical physiology data. Methods in this repository have simple, standard data interfaces and are generally applicable to optical physiology data. As much as possible think arrays and dataframes rather than complex project-specific data structures. 
 
 ## Installation
 
-`pip install aind-ophys-utils`
+```bash
+pip install aind-ophys-utils
+```
 
 To use the software from source, clone the repository and in the root directory run
 ```bash
 pip install -e .
 ```
 
 To develop the code in place, run
```

### Comparing `aind-ophys-utils-0.0.4/doc_template/Makefile` & `aind-ophys-utils-0.0.5/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/doc_template/make.bat` & `aind-ophys-utils-0.0.5/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/doc_template/source/_static/dark-logo.svg` & `aind-ophys-utils-0.0.5/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/doc_template/source/_static/favicon.ico` & `aind-ophys-utils-0.0.5/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/doc_template/source/_static/light-logo.svg` & `aind-ophys-utils-0.0.5/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/doc_template/source/conf.py` & `aind-ophys-utils-0.0.5/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/pyproject.toml` & `aind-ophys-utils-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/src/aind_ophys_utils/array_utils.py` & `aind-ophys-utils-0.0.5/src/aind_ophys_utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/src/aind_ophys_utils/video_utils.py` & `aind-ophys-utils-0.0.5/src/aind_ophys_utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/PKG-INFO` & `aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ophys-utils
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -19,15 +19,17 @@
 ![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?logo=codecov)
 ![Python](https://img.shields.io/badge/python->=3.7-blue?logo=python)
 
 This repository contains python utility methods for processing optical physiology data. Methods in this repository have simple, standard data interfaces and are generally applicable to optical physiology data. As much as possible think arrays and dataframes rather than complex project-specific data structures. 
 
 ## Installation
 
-`pip install aind-ophys-utils`
+```bash
+pip install aind-ophys-utils
+```
 
 To use the software from source, clone the repository and in the root directory run
 ```bash
 pip install -e .
 ```
 
 To develop the code in place, run
```

### Comparing `aind-ophys-utils-0.0.4/src/aind_ophys_utils.egg-info/SOURCES.txt` & `aind-ophys-utils-0.0.5/src/aind_ophys_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/tests/test_array_utils.py` & `aind-ophys-utils-0.0.5/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `aind-ophys-utils-0.0.4/tests/test_video_utils.py` & `aind-ophys-utils-0.0.5/tests/test_video_utils.py`

 * *Files identical despite different names*


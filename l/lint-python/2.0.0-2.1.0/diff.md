# Comparing `tmp/lint-python-2.0.0.tar.gz` & `tmp/lint-python-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lint-python-2.0.0.tar", last modified: Tue Aug  2 11:17:37 2022, max compression
+gzip compressed data, was "lint-python-2.1.0.tar", last modified: Tue Aug  8 16:32:32 2023, max compression
```

## Comparing `lint-python-2.0.0.tar` & `lint-python-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 11:17:37.334101 lint-python-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-08-02 11:17:37.334101 lint-python-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-08-02 11:17:29.000000 lint-python-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 11:17:37.330101 lint-python-2.0.0/lint_python/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-02 11:17:29.000000 lint-python-2.0.0/lint_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 11:17:29.000000 lint-python-2.0.0/lint_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-02 11:17:29.000000 lint-python-2.0.0/lint_python/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6092 2022-08-02 11:17:29.000000 lint-python-2.0.0/lint_python/lint_python.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 11:17:37.334101 lint-python-2.0.0/lint_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-02 11:17:37.000000 lint-python-2.0.0/lint_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-08-02 11:17:29.000000 lint-python-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 11:17:37.334101 lint-python-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:32.125290 lint-python-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-08 16:32:32.125290 lint-python-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-08-08 16:32:24.000000 lint-python-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:32.125290 lint-python-2.1.0/lint_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 16:32:24.000000 lint-python-2.1.0/lint_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:32:24.000000 lint-python-2.1.0/lint_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-08 16:32:24.000000 lint-python-2.1.0/lint_python/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-08-08 16:32:24.000000 lint-python-2.1.0/lint_python/lint_python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:32:32.125290 lint-python-2.1.0/lint_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 16:32:32.000000 lint-python-2.1.0/lint_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 16:32:24.000000 lint-python-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 16:32:32.125290 lint-python-2.1.0/setup.cfg
```

### Comparing `lint-python-2.0.0/PKG-INFO` & `lint-python-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lint-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI tool used for running linter on project configured with CERT-Polska/lint-python-action
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # lint-python-action
```

### Comparing `lint-python-2.0.0/README.md` & `lint-python-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lint-python-2.0.0/lint_python/lint_python.py` & `lint-python-2.1.0/lint_python/lint_python.py`

 * *Files identical despite different names*

### Comparing `lint-python-2.0.0/lint_python.egg-info/PKG-INFO` & `lint-python-2.1.0/lint_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lint-python
-Version: 2.0.0
+Version: 2.1.0
 Summary: CLI tool used for running linter on project configured with CERT-Polska/lint-python-action
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 # lint-python-action
```

### Comparing `lint-python-2.0.0/pyproject.toml` & `lint-python-2.1.0/pyproject.toml`

 * *Files identical despite different names*


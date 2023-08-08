# Comparing `tmp/pynavio-0.2.2.tar.gz` & `tmp/pynavio-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynavio-0.2.2.tar", last modified: Mon Apr  3 13:49:46 2023, max compression
+gzip compressed data, was "pynavio-0.2.3.tar", last modified: Tue Aug  8 20:55:17 2023, max compression
```

## Comparing `pynavio-0.2.2.tar` & `pynavio-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.594224 pynavio-0.2.2/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      146 2023-01-16 14:05:21.000000 pynavio-0.2.2/AUTHORS.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1727 2023-01-16 14:05:21.000000 pynavio-0.2.2/HISTORY.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1069 2023-01-16 14:05:21.000000 pynavio-0.2.2/LICENSE
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      237 2023-01-16 14:05:21.000000 pynavio-0.2.2/MANIFEST.in
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     4324 2023-04-03 13:49:46.594224 pynavio-0.2.2/PKG-INFO
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1928 2023-01-16 14:05:21.000000 pynavio-0.2.2/README.rst
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.586224 pynavio-0.2.2/docs/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      608 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/Makefile
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       28 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/authors.rst
--rwxrwxr-x   0 tatevik   (1000) tatevik   (1000)     4772 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/conf.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       33 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/contributing.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       28 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/history.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      304 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/index.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1138 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/installation.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      769 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/make.bat
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       27 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/readme.rst
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       69 2023-01-16 14:05:21.000000 pynavio-0.2.2/docs/usage.rst
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.590224 pynavio-0.2.2/pynavio/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      774 2023-04-03 11:32:14.000000 pynavio-0.2.2/pynavio/__init__.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     4136 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/_code.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)    17751 2023-03-30 16:34:52.000000 pynavio-0.2.2/pynavio/_mlflow.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     7750 2023-03-15 09:20:40.000000 pynavio-0.2.2/pynavio/client.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3790 2023-03-30 14:08:30.000000 pynavio-0.2.2/pynavio/dependencies.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1008 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/image.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1885 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/model_helpers.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3025 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/schema.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2258 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/traits.py
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.590224 pynavio-0.2.2/pynavio/utils/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      182 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/utils/__init__.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      983 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/utils/common.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1193 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/utils/conda.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      215 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/utils/json_encoder.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2512 2023-03-30 16:34:52.000000 pynavio-0.2.2/pynavio/utils/schemas.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       99 2023-01-16 14:05:21.000000 pynavio-0.2.2/pynavio/utils/styling.py
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.590224 pynavio-0.2.2/pynavio.egg-info/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     4324 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/PKG-INFO
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1023 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/SOURCES.txt
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        1 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/dependency_links.txt
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        1 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/not-zip-safe
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       75 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/requires.txt
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        8 2023-04-03 13:49:46.000000 pynavio-0.2.2/pynavio.egg-info/top_level.txt
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      424 2023-04-03 13:49:46.594224 pynavio-0.2.2/setup.cfg
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1289 2023-04-03 11:32:14.000000 pynavio-0.2.2/setup.py
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.594224 pynavio-0.2.2/tests/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       37 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/__init__.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      111 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/conftest.py
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.594224 pynavio-0.2.2/tests/test_pynavio/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     6615 2023-03-15 09:20:40.000000 pynavio-0.2.2/tests/test_pynavio/test_client.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2145 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/test_pynavio/test_dependencies.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      905 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/test_pynavio/test_dependencies_file_only.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1996 2023-03-30 16:34:52.000000 pynavio-0.2.2/tests/test_pynavio/test_mlflow.py
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3424 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/test_pynavio/test_schema.py
-drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-04-03 13:49:46.594224 pynavio-0.2.2/tests/test_pynavio/test_utils/
--rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1682 2023-01-16 14:05:21.000000 pynavio-0.2.2/tests/test_pynavio/test_utils/test_conda.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      146 2023-04-17 14:52:01.000000 pynavio-0.2.3/AUTHORS.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3580 2023-07-31 15:10:29.000000 pynavio-0.2.3/HISTORY.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1069 2023-01-16 14:05:21.000000 pynavio-0.2.3/LICENSE
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      237 2023-04-17 14:52:01.000000 pynavio-0.2.3/MANIFEST.in
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     6473 2023-08-08 20:55:17.878419 pynavio-0.2.3/PKG-INFO
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2184 2023-07-31 15:10:29.000000 pynavio-0.2.3/README.rst
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/docs/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      608 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/Makefile
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       28 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/authors.rst
+-rwxrwxr-x   0 tatevik   (1000) tatevik   (1000)     4772 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/conf.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       33 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/contributing.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       28 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/history.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      304 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/index.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1138 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/installation.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      769 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/make.bat
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       27 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/readme.rst
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       69 2023-01-16 14:05:21.000000 pynavio-0.2.3/docs/usage.rst
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/pynavio/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      774 2023-08-08 20:37:43.000000 pynavio-0.2.3/pynavio/__init__.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     4136 2023-04-17 14:52:01.000000 pynavio-0.2.3/pynavio/_code.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)    24226 2023-08-08 13:52:32.000000 pynavio-0.2.3/pynavio/_mlflow.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     7750 2023-04-17 14:52:01.000000 pynavio-0.2.3/pynavio/client.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3823 2023-08-08 13:52:32.000000 pynavio-0.2.3/pynavio/dependencies.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1008 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/image.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1935 2023-07-31 15:32:08.000000 pynavio-0.2.3/pynavio/model_helpers.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3025 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/schema.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2258 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/traits.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/pynavio/utils/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      182 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/utils/__init__.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      983 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/utils/common.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1193 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/utils/conda.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      215 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/utils/json_encoder.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3488 2023-08-08 13:52:32.000000 pynavio-0.2.3/pynavio/utils/schemas.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       99 2023-01-16 14:05:21.000000 pynavio-0.2.3/pynavio/utils/styling.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/pynavio.egg-info/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     6473 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/PKG-INFO
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1144 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/SOURCES.txt
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        1 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/dependency_links.txt
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        1 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/not-zip-safe
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       75 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/requires.txt
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)        8 2023-08-08 20:55:17.000000 pynavio-0.2.3/pynavio.egg-info/top_level.txt
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      424 2023-08-08 20:55:17.878419 pynavio-0.2.3/setup.cfg
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1341 2023-08-08 20:54:54.000000 pynavio-0.2.3/setup.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/tests/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)       37 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/__init__.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      111 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/conftest.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/tests/test_pynavio/
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.874418 pynavio-0.2.3/tests/test_pynavio/fixtures/
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/tests/test_pynavio/fixtures/schemas/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      984 2023-04-18 17:03:47.000000 pynavio-0.2.3/tests/test_pynavio/fixtures/schemas/example_request.json
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      987 2023-04-18 17:03:47.000000 pynavio-0.2.3/tests/test_pynavio/fixtures/schemas/example_request_nested.json
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     6615 2023-04-17 14:52:01.000000 pynavio-0.2.3/tests/test_pynavio/test_client.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     2145 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/test_pynavio/test_dependencies.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)      905 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/test_pynavio/test_dependencies_file_only.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     5402 2023-08-08 13:52:32.000000 pynavio-0.2.3/tests/test_pynavio/test_mlflow.py
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     3424 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/test_pynavio/test_schema.py
+drwxrwxr-x   0 tatevik   (1000) tatevik   (1000)        0 2023-08-08 20:55:17.878419 pynavio-0.2.3/tests/test_pynavio/test_utils/
+-rw-rw-r--   0 tatevik   (1000) tatevik   (1000)     1682 2023-01-16 14:05:21.000000 pynavio-0.2.3/tests/test_pynavio/test_utils/test_conda.py
```

### Comparing `pynavio-0.2.2/LICENSE` & `pynavio-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/PKG-INFO` & `pynavio-0.2.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynavio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python lib for navio
 Home-page: https://github.com/craftworksgmbh/craftworks-pynavio
 Author: craftworks
 Author-email: dev-accounts@craftworks.at
 License: MIT license
 Keywords: pynavio
 Platform: UNKNOWN
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =======
 pynavio
 =======
 
@@ -32,14 +33,16 @@
 * Free software: MIT license
 
 
 Features
 --------
 * Pynavio.Client, navio API client, allows to upload models and data, deploy and retrain models etc.
 * Pynavio.mlflow.to_navio function calls mlflow.pyfunc.save_model function, saving a model zip file as required by navio.
+    * it also validated the models with Pynavio.mlflow.ModelValidator by default
+* Pynavio.mlflow.ModelValidator is a class that validates the model (prediction/example request/MLmodel metadata schema checks, warnings related nested types/big model sizes)
 * Pynavio.infer_external_dependencies is a helper function that infers the external dependencies based on the file path. For its limitations please refer to its doc string.
 * Pynavio.infer_imported_code_path is a helper function that  infers the imported code paths based on the file path and the root path. For its limitations please refer to its doc string.
 * Pynavio.make_example_request generates a request schema for a navio model from data.
 
 Documentation
 -------------
 
@@ -123,13 +126,67 @@
 * sets protobuf version to fix failing tests
 * fixes to_navio() to support kedro path
 
 0.1.5 (2022-09-15)
 ------------------
 
 * fixes the documentation link
-* attempts to remove the build badgegi
+* attempts to remove the build badge
 * removes installation for development section form readme
 * fixes repository on the pypi page
 * adds history
 
+0.1.6 (2022-09-15)
+------------------
+
+* final touches/refactoring to make the repo ready for becoming public
+
+0.1.7 (2022-11-16)
+------------------
+
+* fixes mlflow version to be <2.0 as it introduces breaking changes in the api
+* wraps navio's model deletion api
+
+
+0.2.0 (2022-11-30)
+------------------
+
+* resolves mlflow2 incompatibility
+* brings model validation checks:prediction, example request and MLmodel metadata schema validation
+* makes check_model_serving function public
+* adds jsonschema to requirements
+* bump tensorflow from 2.9.1 to 2.9.3
+* bump pillow from 9.2.0 to 9.3.0
+* refactors example tests
+
+0.2.1 (2022-12-07)
+------------------
+
+* loosens version requirement for jsonschema
+* improves and fixes typos in error message texts
+* prevents the exception traceback from prediction_call when checking if it is used, to not confuse the user
+* brings a descriptive error if model path in code_path
+* brings a descriptive error if code_path is not a list
+
+0.2.2 (2023-04-03 )
+------------------
+
+* bump tensorflow from 2.9.3 to 2.11.1
+* updates torch version and adds onnx as requirement
+* fixes torch, pyarrow and onnxrutime versions
+* fixes the prediction schema to only expect a list as prediction
+* bump ipython from 8.4.0 to 8.10.0
+* improves the docstring of to_navio function
+* bump wheel from 0.37.1 to 0.38.1
+
+0.2.3 (2023-04-xx )
+------------------
+
+* adds warnings related to limitations for nested inputs and big model.zip size
+* make ModelValidator a public class
+* adds docstrings to ModelValidator
+* makes model validation optional in to_navio(), so one can disable it
+* adds (pynavio model validation) to the validation messages so it is clear where they come from
+* adds messages for pynavio model validation checks failed(how to disable)/succeeded(how to check model serving)
+* updates readme with model validation info
+
```

### Comparing `pynavio-0.2.2/README.rst` & `pynavio-0.2.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 * Free software: MIT license
 
 
 Features
 --------
 * Pynavio.Client, navio API client, allows to upload models and data, deploy and retrain models etc.
 * Pynavio.mlflow.to_navio function calls mlflow.pyfunc.save_model function, saving a model zip file as required by navio.
+    * it also validated the models with Pynavio.mlflow.ModelValidator by default
+* Pynavio.mlflow.ModelValidator is a class that validates the model (prediction/example request/MLmodel metadata schema checks, warnings related nested types/big model sizes)
 * Pynavio.infer_external_dependencies is a helper function that infers the external dependencies based on the file path. For its limitations please refer to its doc string.
 * Pynavio.infer_imported_code_path is a helper function that  infers the imported code paths based on the file path and the root path. For its limitations please refer to its doc string.
 * Pynavio.make_example_request generates a request schema for a navio model from data.
 
 Documentation
 -------------
```

### Comparing `pynavio-0.2.2/docs/Makefile` & `pynavio-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/docs/conf.py` & `pynavio-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/docs/installation.rst` & `pynavio-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/docs/make.bat` & `pynavio-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/__init__.py` & `pynavio-0.2.3/pynavio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for pynavio."""
 
 __author__ = """craftworks"""
 __email__ = 'dev-accounts@craftworks.at'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 from . import _code as code
 from . import _mlflow as mlflow
 from . import dependencies, image, model_helpers, schema, traits, utils
 from ._code import infer_imported_code_path
 from .dependencies import infer_external_dependencies
 from .model_helpers import assert_gpu_available, prediction_call
```

### Comparing `pynavio-0.2.2/pynavio/_code.py` & `pynavio-0.2.3/pynavio/_code.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/_mlflow.py` & `pynavio-0.2.3/pynavio/_mlflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,73 @@
+import copy
 import json
 import shutil
-from pathlib import Path, PosixPath
-from tempfile import TemporaryDirectory
-from typing import Any, Dict, List, Optional, Union
 import subprocess
 import time
-import requests
 from collections.abc import Mapping
+from pathlib import Path, PosixPath
+from tempfile import TemporaryDirectory
+from typing import Any, Dict, List, Optional, Union
 
+import jsonschema
 import mlflow
-import copy
 import pandas as pd
+import requests
 import yaml
-import jsonschema
 
 from pynavio.utils import ExampleRequestType, make_env
 from pynavio.utils.json_encoder import JSONEncoder
-from pynavio.utils.schemas import PREDICTION_SCHEMA, \
-    METADATA_SCHEMA, REQUEST_SCHEMA_SCHEMA
+from pynavio.utils.schemas import (METADATA_SCHEMA, PREDICTION_SCHEMA,
+                                   REQUEST_SCHEMA_SCHEMA,
+                                   not_nested_request_schema)
 
+MODEL_SIZE_LIMIT_IN_BYTES = 1000_000_000
 EXAMPLE_REQUEST = 'example_request'
 ARTIFACTS = 'artifacts'
 ArtifactsType = Optional[Dict[str, str]]
 ERROR_KEYS = {'error_code', 'message', 'stack_trace'}
 PREDICTION_KEY = 'prediction'
+pynavio_model_validation = '(pynavio model validation)'
+
+METADATA = 'metadata'
+OOD_DETECTION = 'oodDetection'
+MLMODEL = 'MLmodel'
+REQUEST_SCHEMA = 'request_schema'
+DATASET = 'dataset'
+EXPLANATIONS = 'explanations'
+
+
+def _is_ood_set_to_default_in_metadata(metadata: dict) -> bool:
+    return metadata.get(OOD_DETECTION, '') == 'default'
+
+
+def _is_explanation_set_to_default_in_metadata(metadata: dict) -> bool:
+    return metadata.get(EXPLANATIONS, '') == 'default'
+
+
+def _is_data_provided_in_metadata(metadata: dict) -> bool:
+    return DATASET in metadata
+
+
+def _is_default_ood_enabled_in_metadata(metadata: dict) -> bool:
+    return _is_ood_set_to_default_in_metadata(metadata) and \
+           _is_data_provided_in_metadata(metadata)
+
+
+def _is_default_explanation_enabled_in_metadata(metadata: dict) -> bool:
+    return _is_explanation_set_to_default_in_metadata(metadata) and \
+           _is_data_provided_in_metadata(metadata)
+
+
+def check_zip_size(model_zip, model_size_in_bytes):
+    if Path(model_zip).stat().st_size > model_size_in_bytes:
+        print(f"Warning: the default model.zip size limit is"
+              f" {model_size_in_bytes} bytes. Please reduce the"
+              f" size or contact craftworks support team to"
+              f" increase the default size")
 
 
 def _get_field(yml: dict, path: str) -> Optional[Any]:
     keys = path.split('.')
     assert keys, 'Path must not be empty'
 
     value = yml.get(keys[0])
@@ -163,20 +203,17 @@
 
     data_path = _get_field(yml, 'metadata.dataset.path')
     data_path = Path(model_path) / data_path if data_path is not None else None
 
     example_request = _read_example_request(model_path, yml)
 
     return {
-        'dataset':
-            pd.read_csv(data_path) if data_path is not None else None,
-        'explanation_format':
-            _get_field(yml, 'metadata.explanations.format'),
-        'example_request':
-            example_request
+        'dataset': pd.read_csv(data_path) if data_path is not None else None,
+        'explanation_format': _get_field(yml, 'metadata.explanations.format'),
+        'example_request': example_request
     }
 
 
 def _fetch_data(model_path: str) -> dict:
     meta = _read_metadata(model_path)
     data = meta['example_request']
 
@@ -207,95 +244,176 @@
 
 
 def _get_example_request_df(model_path):
     data = _fetch_data(model_path)[0]
     return pd.DataFrame(data['data'], columns=data['columns'])
 
 
-class _ModelValidator:
+def _validate_schema(data, schema, name='', raise_exception=True):
+    """
+    Validate the given data against the specified JSON schema.
+
+    @param data: The data to validate.
+    @param schema: The jsonschema schema to validate against.
+    @param name: A descriptive name for the data being validated,
+        used in error message
+    @param raise_exception: Whether to raise an exception if the
+        validation fails. If True (default), the function raises a
+        jsonschema ValidationError exception with a
+        descriptive error message.
+    @return: True if the validation passes, False otherwise.
+     Only returned if raise_exception is False.
+    """
+    is_valid = True
+    try:
+        jsonschema.validate(data, schema)
+    except jsonschema.exceptions.ValidationError:
+        if raise_exception:
+            print(f"Error: {pynavio_model_validation} "
+                  f"Error during {name} validation")
+            raise
+        else:
+            is_valid = False
+    return is_valid
+
+
+def is_input_nested(example_request, not_nested_schema):
+    is_not_nested = _validate_schema(example_request,
+                                     not_nested_schema,
+                                     '',
+                                     raise_exception=False)
+    return not is_not_nested
+
+
+def _is_wrapped_by_prediction_call(func):
+    return getattr(func, '__wrapped_by_prediction_call__', False)
+
+
+def _is_model_predict_wrapped_by_prediction_call(model):
+    return _is_wrapped_by_prediction_call(
+        model._model_impl.python_model.predict)
+
+
+class ModelValidator:
+    """
+    A utility class for validating navio mlflow models.
+    Raises jsonschema.exceptions.ValidationError and AssertionError if
+    there are errors in validation.
+    Example usage:
+        >>> ModelValidator()(model_path = '/path/to/my/model')
+
+    """
+
     @staticmethod
     def validate_metadata(model_path):
+        """
+        Validate the metadata: example request file and MLmodel file
+        of the given navio mlflow model.
+
+        @param model_path: The directory path of the model to validate.
+        @raises jsonschema.exceptions.ValidationError:
+        If there is an error during the validation process.
+        @return: None
+        """
         config = _read_mlmodel_yaml(model_path)
-        try:
-            jsonschema.validate(config.get('metadata'), METADATA_SCHEMA)
-        except jsonschema.exceptions.ValidationError:
-            print("Error during MLmodel validation")
-            raise
+        metadata = config.get('metadata')
+        _validate_schema(metadata, METADATA_SCHEMA, "MLmodel")
 
         example_request = _read_example_request(model_path, config)
-        try:
-            jsonschema.validate(example_request, REQUEST_SCHEMA_SCHEMA)
-        except jsonschema.exceptions.ValidationError:
-            print("Error during example request validation")
-            raise
+        _validate_schema(example_request, REQUEST_SCHEMA_SCHEMA,
+                         "example request")
+        if is_input_nested(example_request, not_nested_request_schema()):
+            print('Warning: {pynavio_model_validation} the nested'
+                  ' model input is not supported'
+                  ' by frontend rendering, it will only be possible'
+                  ' to see the example request as plain json in the'
+                  ' try-out or deployment views. Consider using'
+                  ' string representation of nested example in the'
+                  ' example request json.')
+            if _is_default_ood_enabled_in_metadata(metadata) or \
+                    _is_default_explanation_enabled_in_metadata(metadata):
+                print("Warning: {pynavio_model_validation} default"
+                      " ood and explanations"
+                      " are not supported for nested model inputs.")
 
     @staticmethod
     def run_model_io(model_path, model_input=None, **kwargs):
+        """
+        Run the given navio mlflow model file with the given input.
+
+        @param model_path: The directory path of the model to run.
+        @param model_input: optional, the input data for the model's
+        predict method. If None, the example request specified in
+        the model metadata will be used as input.
+        @param kwargs: Additional keyword arguments.
+
+        @return: The input data and the prediction output.
+        """
         model = mlflow.pyfunc.load_model(model_path)
         if model_input is None:
             model_input = _get_example_request_df(model_path)
         return model_input, model.predict(model_input)
 
     @staticmethod
     def _check_if_prediction_call_is_used(model_path):
-        # In order to check if the pynavio.prediction_call
-        # is used to decorate the predict method of the model,
-        # a corrupt input is provided. If there is an exception
-        # or the expected keys are not present in the model output,
-        # then that means that the decorator is not applied
-
         model = mlflow.pyfunc.load_model(model_path)
-        corrupt_model_input = pd.DataFrame(
-            {'corrupt_model_input_123': [1, 2, 3]})
-
-        import logging
-        logger = logging.getLogger('gunicorn.error')
-        current_loglevel = logger.level
-        logger.setLevel(logging.CRITICAL)  # this is done to prevent
-        # logging the exception traceback from prediction call
-        # as it will be confusing for the user
-
-        error_msg = \
-            "Please use pynavio.prediction_call to decorate " \
-            "the predict method of the model, which will add the " \
-            "needed error keys for error case"
+        used = True  # do not print warning if not sure
+        # try checking the original model's predict function
         try:
-            model_output = model.predict(corrupt_model_input)
-        except Exception:
-            raise KeyError(error_msg)
-        finally:
-            logger.setLevel(current_loglevel)
-
-        assert isinstance(model_output, Mapping), "Model " \
-            "output has to be a dictionary"
+            used = _is_model_predict_wrapped_by_prediction_call(model)
+        except AttributeError:
+            pass
+        if not used:
+            print(f"Warning: {pynavio_model_validation} Please use"
+                  f" pynavio.prediction_call to decorate"
+                  f" the predict method of the model, which will add the"
+                  f" needed error keys({ERROR_KEYS}) for error"
+                  f" case to see descriptive"
+                  f" errors from navio for ease of debugging.")
 
-        if PREDICTION_KEY not in model_output:  # precaution
-            # to allow for models that always return prediction
-
-            assert set(model_output.keys()) == ERROR_KEYS, error_msg
+    @staticmethod
+    def check_zip_size(model_zip, model_size_in_bytes):
+        if Path(model_zip).stat().st_size > model_size_in_bytes:
+            print(f"Warning: {pynavio_model_validation} "
+                  f"the default model.zip size limit is"
+                  f" {model_size_in_bytes} bytes. Please reduce the"
+                  f" size or contact craftworks support team to"
+                  f" increase the default size")
 
     @staticmethod
     def verify_model_output(model_output, **kwargs):
+        """
+        Verify the output of the navio mlflow model.
+
+        @param model_output: The output of the model.
+        @param kwargs: Additional keyword arguments.
+
+        @raises AssertionError: If the output is not valid.
+        @return: None
+        """
+
         def _validate_prediction_schema(model_prediction):
             try:
                 jsonschema.validate(model_prediction, PREDICTION_SCHEMA)
             except jsonschema.exceptions.ValidationError:
-                print(f"Error: The value of model_output['{PREDICTION_KEY}']"
+                print(f"ERROR: {pynavio_model_validation} The value of "
+                      f"model_output['{PREDICTION_KEY}']"
                       " must be one of the following types "
                       "(cannot be nested or mixed type): "
                       "'array','boolean', 'integer', 'number', 'string'")
                 raise
 
         assert isinstance(model_output, Mapping), "Model " \
-            "output has to be a dictionary"
+            f"ERROR: {pynavio_model_validation} output has to be a dictionary"
 
         if PREDICTION_KEY in model_output:
             _validate_prediction_schema(model_output)
         else:
             assert set(model_output.keys()) == ERROR_KEYS, \
+                f"ERROR: {pynavio_model_validation}" \
                 f"The model output has to contain '{PREDICTION_KEY}'" \
                 f" for prediction" \
                 f" as key for the target, independent of" \
                 f" the target name in the example request" \
                 f". There can be other keys, " \
                 f" that will be listed under " \
                 f" 'additionalFields' in the response of the model " \
@@ -308,38 +426,51 @@
                 f" to navio."\
                 f" Or The model output has to contain the following" \
                 f" keys [{ERROR_KEYS}] if error occurs."\
                 f"Please use pynavio.prediction_call to decorate " \
                 f"the predict method of the model, which will add the " \
                 f"needed error keys for error case"
 
-    def __call__(self, model_path, **kwargs):
+    def _run(self, model_path, model_zip, model_zip_size_limit, **kwargs):
         self.validate_metadata(model_path)
         model_input, model_output = self.run_model_io(model_path)
         self._check_if_prediction_call_is_used(model_path)
         self.verify_model_output(model_output)
+        self.check_zip_size(model_zip, model_zip_size_limit)
+
+    def __call__(self, model_path, model_zip, model_zip_size_limit, **kwargs):
+        try:
+            self._run(model_path, model_zip, model_zip_size_limit, **kwargs)
+        except (jsonschema.exceptions.ValidationError, AssertionError):
+            print(f'{pynavio_model_validation}: Validation failed. Please fix'
+                  f' the identified issues before uploading the model.'
+                  f'{kwargs.get("append_to_failed_msg", "")}')
+            raise
+        print(f'{pynavio_model_validation}: Validation succeeded.'
+              f'{kwargs.get("append_to_succeeded_msg", "")}')
 
 
 def _is_mlflow2():
-    from packaging import version
     import mlflow
+    from packaging import version
     return version.parse(mlflow.__version__) >= version.parse("2.0.0")
 
 
 def _convert_to_mlflow2_format(request_data):
     dataframe_records = pd.DataFrame.from_records(
         columns=request_data['columns'],
         data=request_data['data']).\
         to_json(orient='records')
     request_data = {"dataframe_records": json.loads(dataframe_records)}
     return request_data
 
 
 def check_model_serving(model_path: Union[str, Path],
-                        port=5001, request_bodies=None):
+                        port=5001,
+                        request_bodies=None):
     """
     checks model serving with mlflow. This has limitations, e.g.
     the 'conda.env' setup will not be checked.
     Note: Please refer to
     https://navio.craftworks.io/docs/guides/navio-models/model_creation/#3-test-model-serving
     for testing the model serving.
 
@@ -382,16 +513,16 @@
              conda_packages: List[str] = None,
              conda_channels: List[str] = None,
              conda_env: str = None,
              artifacts: ArtifactsType = None,
              dataset: Optional[dict] = None,
              explanations: Optional[str] = None,
              oodd: Optional[str] = None,
-             num_gpus: Optional[int] = 0
-             ) -> Path:
+             num_gpus: Optional[int] = 0,
+             validate_model: Optional[bool] = True) -> Path:
     """
     create a .zip mlflow model file for navio
     Usage: either pip_packages or conda_env need to be set.
 
     @param model: model to save
     @param path: path of where model .zip file needs to be saved
     @param example_request: example_request for the given model.
@@ -411,14 +542,16 @@
     @param artifacts: If not set, need to set example_request
     @param dataset:
     @param explanations: expected values are ['disabled', 'default', 'plotly']
      If not set, 'default' is used
     @param oodd: expected values are ['disabled', 'default'].
      If not set, 'default' is used
     @param num_gpus:
+    @param validate_model: if the output model should be validated by
+     ModelValidator. On by default(True), to disable set to False.
 
     Note: Please refer to check_model_serving() method and
     https://navio.craftworks.io/docs/guides/navio-models/model_creation/#3-test-model-serving
     for testing the model serving.
 
     @return: path to the .zip model file
     """
@@ -427,16 +560,17 @@
     if code_path:
         if not isinstance(code_path, list):
             raise TypeError("'code_path' argument must be a"
                             " list (of local filesystem paths to Python file"
                             "dependencies (or directories containing file "
                             "dependencies)), but is not a list")
 
-        if any(Path(code_p).resolve() in Path(path).resolve().parents
-               for code_p in code_path):
+        if any(
+                Path(code_p).resolve() in Path(path).resolve().parents
+                for code_p in code_path):
             raise ValueError("any of 'code_path' argument paths cannot"
                              " be a parent of 'path' argument,"
                              f" please change the 'path': {path} to be"
                              f" outside of the 'code_path' paths:{code_path}")
 
     artifacts = artifacts or dict()
     artifacts = {key: process_path(value) for key, value in artifacts.items()}
@@ -463,11 +597,28 @@
 
         _add_metadata(path,
                       dataset=dataset,
                       explanations=explanations,
                       oodd=oodd,
                       num_gpus=num_gpus)
 
-    _ModelValidator()(path)
+        shutil.make_archive(path, 'zip', path)
+        model_zip = Path(path + '.zip')
+
+    if validate_model:
+        msg_kwargs = {
+            'append_to_failed_msg': ' To disable validation set '
+                                    'validate_model to False',
+            'append_to_succeeded_msg': ' Note: Please refer to '
+                                       'check_model_serving()'
+                                       ' method and '
+                                       'https://navio.craftworks.io/'
+                                       'docs/guides/navio-models/'
+                                       'model_creation/'
+                                       '#3-test-model-serving'
+                                       ' for testing the model '
+                                       'serving.',
+        }
+        ModelValidator()(path, model_zip, MODEL_SIZE_LIMIT_IN_BYTES,
+                         **msg_kwargs)
 
-    shutil.make_archive(path, 'zip', path)
-    return Path(path + '.zip')
+    return model_zip
```

### Comparing `pynavio-0.2.2/pynavio/client.py` & `pynavio-0.2.3/pynavio/client.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/dependencies.py` & `pynavio-0.2.3/pynavio/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,17 @@
 
     yes = subprocess.Popen(('yes', 'Y'), stdout=subprocess.PIPE)
 
     module_path = _get_file_or_module_path(module_path, file_only, tmp_dir)
 
     ignore_dirs_args = _generate_ignore_dirs_args(module_path, to_ignore_dirs)
 
-    result = subprocess.call(
-        ('pigar', '-P', f'{module_path}', '-p', f'{requirements_txt_file}',
-         *ignore_dirs_args),
-        stdin=yes.stdout)
+    result = subprocess.call(('pigar', '-P', f'{module_path}', '-p',
+                              f'{requirements_txt_file}', *ignore_dirs_args),
+                             stdin=yes.stdout)
     if result != 0:
         logging.error("please create and provide requirements.txt, as "
                       "there was an error using pigar to auto-generate "
                       "requirements.txt")
         raise AssertionError
```

### Comparing `pynavio-0.2.2/pynavio/image.py` & `pynavio-0.2.3/pynavio/image.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/model_helpers.py` & `pynavio-0.2.3/pynavio/model_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             logger.exception('Prediction call failed')
             return {
                 'error_code': exc.__class__.__name__,
                 'message': str(exc),
                 'stack_trace': traceback.format_exc()
             }
 
+    wrapper.__wrapped_by_prediction_call__ = True
     return wrapper
 
 
 def assert_gpu_available() -> None:
     """ Helper for ensuring GPU models actually register the GPU
 
     Only triggers an error if NVIDIA_VISIBLE_DEVICES env. var. is defined
```

### Comparing `pynavio-0.2.2/pynavio/schema.py` & `pynavio-0.2.3/pynavio/schema.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/traits.py` & `pynavio-0.2.3/pynavio/traits.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/utils/common.py` & `pynavio-0.2.3/pynavio/utils/common.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio/utils/conda.py` & `pynavio-0.2.3/pynavio/utils/conda.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/pynavio.egg-info/PKG-INFO` & `pynavio-0.2.3/pynavio.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynavio
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python lib for navio
 Home-page: https://github.com/craftworksgmbh/craftworks-pynavio
 Author: craftworks
 Author-email: dev-accounts@craftworks.at
 License: MIT license
 Keywords: pynavio
 Platform: UNKNOWN
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 =======
 pynavio
 =======
 
@@ -32,14 +33,16 @@
 * Free software: MIT license
 
 
 Features
 --------
 * Pynavio.Client, navio API client, allows to upload models and data, deploy and retrain models etc.
 * Pynavio.mlflow.to_navio function calls mlflow.pyfunc.save_model function, saving a model zip file as required by navio.
+    * it also validated the models with Pynavio.mlflow.ModelValidator by default
+* Pynavio.mlflow.ModelValidator is a class that validates the model (prediction/example request/MLmodel metadata schema checks, warnings related nested types/big model sizes)
 * Pynavio.infer_external_dependencies is a helper function that infers the external dependencies based on the file path. For its limitations please refer to its doc string.
 * Pynavio.infer_imported_code_path is a helper function that  infers the imported code paths based on the file path and the root path. For its limitations please refer to its doc string.
 * Pynavio.make_example_request generates a request schema for a navio model from data.
 
 Documentation
 -------------
 
@@ -123,13 +126,67 @@
 * sets protobuf version to fix failing tests
 * fixes to_navio() to support kedro path
 
 0.1.5 (2022-09-15)
 ------------------
 
 * fixes the documentation link
-* attempts to remove the build badgegi
+* attempts to remove the build badge
 * removes installation for development section form readme
 * fixes repository on the pypi page
 * adds history
 
+0.1.6 (2022-09-15)
+------------------
+
+* final touches/refactoring to make the repo ready for becoming public
+
+0.1.7 (2022-11-16)
+------------------
+
+* fixes mlflow version to be <2.0 as it introduces breaking changes in the api
+* wraps navio's model deletion api
+
+
+0.2.0 (2022-11-30)
+------------------
+
+* resolves mlflow2 incompatibility
+* brings model validation checks:prediction, example request and MLmodel metadata schema validation
+* makes check_model_serving function public
+* adds jsonschema to requirements
+* bump tensorflow from 2.9.1 to 2.9.3
+* bump pillow from 9.2.0 to 9.3.0
+* refactors example tests
+
+0.2.1 (2022-12-07)
+------------------
+
+* loosens version requirement for jsonschema
+* improves and fixes typos in error message texts
+* prevents the exception traceback from prediction_call when checking if it is used, to not confuse the user
+* brings a descriptive error if model path in code_path
+* brings a descriptive error if code_path is not a list
+
+0.2.2 (2023-04-03 )
+------------------
+
+* bump tensorflow from 2.9.3 to 2.11.1
+* updates torch version and adds onnx as requirement
+* fixes torch, pyarrow and onnxrutime versions
+* fixes the prediction schema to only expect a list as prediction
+* bump ipython from 8.4.0 to 8.10.0
+* improves the docstring of to_navio function
+* bump wheel from 0.37.1 to 0.38.1
+
+0.2.3 (2023-04-xx )
+------------------
+
+* adds warnings related to limitations for nested inputs and big model.zip size
+* make ModelValidator a public class
+* adds docstrings to ModelValidator
+* makes model validation optional in to_navio(), so one can disable it
+* adds (pynavio model validation) to the validation messages so it is clear where they come from
+* adds messages for pynavio model validation checks failed(how to disable)/succeeded(how to check model serving)
+* updates readme with model validation info
+
```

### Comparing `pynavio-0.2.2/pynavio.egg-info/SOURCES.txt` & `pynavio-0.2.3/pynavio.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -39,8 +39,10 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_pynavio/test_client.py
 tests/test_pynavio/test_dependencies.py
 tests/test_pynavio/test_dependencies_file_only.py
 tests/test_pynavio/test_mlflow.py
 tests/test_pynavio/test_schema.py
+tests/test_pynavio/fixtures/schemas/example_request.json
+tests/test_pynavio/fixtures/schemas/example_request_nested.json
 tests/test_pynavio/test_utils/test_conda.py
```

### Comparing `pynavio-0.2.2/setup.py` & `pynavio-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,18 +27,20 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="Python lib for navio",
     install_requires=requirements,
     license="MIT license",
+    long_description_content_type='text/markdown',
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='pynavio',
     name='pynavio',
     packages=find_packages(include=['pynavio', 'pynavio.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/craftworksgmbh/craftworks-pynavio',
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
+
 )
```

### Comparing `pynavio-0.2.2/tests/test_pynavio/test_client.py` & `pynavio-0.2.3/tests/test_pynavio/test_client.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/tests/test_pynavio/test_dependencies.py` & `pynavio-0.2.3/tests/test_pynavio/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/tests/test_pynavio/test_dependencies_file_only.py` & `pynavio-0.2.3/tests/test_pynavio/test_dependencies_file_only.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/tests/test_pynavio/test_schema.py` & `pynavio-0.2.3/tests/test_pynavio/test_schema.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.2.2/tests/test_pynavio/test_utils/test_conda.py` & `pynavio-0.2.3/tests/test_pynavio/test_utils/test_conda.py`

 * *Files identical despite different names*


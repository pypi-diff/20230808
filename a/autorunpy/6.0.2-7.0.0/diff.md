# Comparing `tmp/autorunpy-6.0.2.tar.gz` & `tmp/autorunpy-7.0.0.tar.gz`

## Comparing `autorunpy-6.0.2.tar` & `autorunpy-7.0.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autorunpy-6.0.2/.gitattributes
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-6.0.2/.github/workflows/publish-on-pip-on-release.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/auto.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/dl_and_ret_dirpath.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/github_release.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/make_venv.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/ret_module_2_run_name.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 autorunpy-6.0.2/src/autorunpy/util.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-6.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-6.0.2/LICENSE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-6.0.2/README.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 autorunpy-6.0.2/pyproject.toml
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 autorunpy-6.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 autorunpy-7.0.0/.github/workflows/publish-on-pip-on-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/make_venv.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/ret_module_2_run.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/ret_pkg_name.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/rm_venv.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 autorunpy-7.0.0/src/autorunpy/util.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 autorunpy-7.0.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 autorunpy-7.0.0/LICENSE
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autorunpy-7.0.0/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 autorunpy-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 autorunpy-7.0.0/PKG-INFO
```

### Comparing `autorunpy-6.0.2/.github/workflows/publish-on-pip-on-release.yml` & `autorunpy-7.0.0/.github/workflows/publish-on-pip-on-release.yml`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.2/.gitignore` & `autorunpy-7.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.2/LICENSE` & `autorunpy-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autorunpy-6.0.2/PKG-INFO` & `autorunpy-7.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: autorunpy
-Version: 6.0.2
+Version: 7.0.0
 Summary: Tools for auto running python scripts
-Project-URL: Homepage, https://github.com/imahdimir/pyautorun
-Project-URL: Bug Tracker, https://github.com/imahdimir/pyautorun/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,11 +21,10 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
-Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 Tools for auto running Python scripts.
```


# Comparing `tmp/preamble-0.0.1.tar.gz` & `tmp/preamble-0.0.2.tar.gz`

## Comparing `preamble-0.0.1.tar` & `preamble-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 preamble-0.0.1/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 preamble-0.0.1/src/preamble/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 preamble-0.0.1/src/preamble/preamble.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 preamble-0.0.1/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 preamble-0.0.1/README.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 preamble-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 preamble-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 preamble-0.0.2/src/.DS_Store
+-rwxr-xr-x   0        0        0     5488 2020-02-02 00:00:00.000000 preamble-0.0.2/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 preamble-0.0.2/src/preamble/__init__.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 preamble-0.0.2/src/preamble/preamble_core.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 preamble-0.0.2/src/preamble/preamble_nemo.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 preamble-0.0.2/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 preamble-0.0.2/README.md
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 preamble-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 preamble-0.0.2/PKG-INFO
```

### Comparing `preamble-0.0.1/src/.DS_Store` & `preamble-0.0.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `preamble-0.0.1/LICENSE` & `preamble-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `preamble-0.0.1/pyproject.toml` & `preamble-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "preamble"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jonathan Cefalu", email="jon@preamble.com" },
 ]
 description = "APIs for connecting to the preamble.com AI safety backend"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `preamble-0.0.1/PKG-INFO` & `preamble-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preamble
-Version: 0.0.1
+Version: 0.0.2
 Summary: APIs for connecting to the preamble.com AI safety backend
 Project-URL: Homepage, https://github.com/preambleai/preamble_pypi
 Project-URL: Bug Tracker, https://github.com/preambleai/preamble_pypi/issues
 Author-email: Jonathan Cefalu <jon@preamble.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


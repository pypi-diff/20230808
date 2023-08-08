# Comparing `tmp/kraken_build-0.30.4.tar.gz` & `tmp/kraken_build-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_build-0.30.4.tar", max compression
+gzip compressed data, was "kraken_build-0.31.0.tar", max compression
```

## Comparing `kraken_build-0.30.4.tar` & `kraken_build-0.31.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      998 2023-08-03 22:30:29.506150 kraken_build-0.30.4/LICENSE
--rw-r--r--   0        0        0      178 2023-08-03 22:30:29.506415 kraken_build-0.30.4/README.md
--rw-r--r--   0        0        0      698 2023-08-03 23:13:40.785327 kraken_build-0.30.4/pyproject.toml
--rw-r--r--   0        0        0       23 2023-08-03 23:13:40.785522 kraken_build-0.30.4/src/kraken/build/__init__.py
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 kraken_build-0.30.4/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-08-03 22:30:29.506150 kraken_build-0.31.0/LICENSE
+-rw-r--r--   0        0        0      178 2023-08-03 22:30:29.506415 kraken_build-0.31.0/README.md
+-rw-r--r--   0        0        0      698 2023-08-08 12:54:53.644739 kraken_build-0.31.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-08-08 12:54:53.644914 kraken_build-0.31.0/src/kraken/build/__init__.py
+-rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 kraken_build-0.31.0/PKG-INFO
```

### Comparing `kraken_build-0.30.4/LICENSE` & `kraken_build-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_build-0.30.4/pyproject.toml` & `kraken_build-0.31.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-build"
-version = "0.30.4"
+version = "0.31.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/build", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_build-0.30.4/PKG-INFO` & `kraken_build-0.31.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-build
-Version: 0.30.4
+Version: 0.31.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


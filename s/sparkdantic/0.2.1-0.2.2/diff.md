# Comparing `tmp/sparkdantic-0.2.1.tar.gz` & `tmp/sparkdantic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkdantic-0.2.1.tar", max compression
+gzip compressed data, was "sparkdantic-0.2.2.tar", max compression
```

## Comparing `sparkdantic-0.2.1.tar` & `sparkdantic-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1570 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/README.md
--rw-r--r--   0        0        0      981 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/src/sparkdantic/__init__.py
--rw-r--r--   0        0        0     4577 2023-07-29 12:14:24.030539 sparkdantic-0.2.1/src/sparkdantic/model.py
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 sparkdantic-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1570 2023-08-08 10:57:03.179660 sparkdantic-0.2.2/README.md
+-rw-r--r--   0        0        0      981 2023-08-08 10:57:03.179660 sparkdantic-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-08-08 10:57:03.179660 sparkdantic-0.2.2/src/sparkdantic/__init__.py
+-rw-r--r--   0        0        0     4577 2023-08-08 10:57:03.179660 sparkdantic-0.2.2/src/sparkdantic/model.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 sparkdantic-0.2.2/PKG-INFO
```

### Comparing `sparkdantic-0.2.1/README.md` & `sparkdantic-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ##  SparkDantic
 
 [![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
 
-> 1️⃣ version: 0.2.1
+> 1️⃣ version: 0.2.2
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```

### Comparing `sparkdantic-0.2.1/pyproject.toml` & `sparkdantic-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkdantic"
-version = "0.2.1"
+version = "0.2.2"
 description = "A pydantic -> spark schema library"
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "sparkdantic", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `sparkdantic-0.2.1/src/sparkdantic/model.py` & `sparkdantic-0.2.2/src/sparkdantic/model.py`

 * *Files identical despite different names*

### Comparing `sparkdantic-0.2.1/PKG-INFO` & `sparkdantic-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdantic
-Version: 0.2.1
+Version: 0.2.2
 Summary: A pydantic -> spark schema library
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: pyspark (>=3.4.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 ##  SparkDantic
 
 [![PyPI version](https://badge.fury.io/py/sparkdantic.svg)](https://badge.fury.io/py/sparkdantic)
 
-> 1️⃣ version: 0.2.1
+> 1️⃣ version: 0.2.2
 
 > ✍️ author: Mitchell Lisle
 
 # PySpark Model Conversion Tool
 
 This Python module provides a utility for converting Pydantic models to PySpark schemas. It's implemented as a class 
 named `SparkModel` that extends the Pydantic's `BaseModel`.
```


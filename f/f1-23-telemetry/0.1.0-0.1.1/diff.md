# Comparing `tmp/f1_23_telemetry-0.1.0.tar.gz` & `tmp/f1_23_telemetry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f1_23_telemetry-0.1.0.tar", max compression
+gzip compressed data, was "f1_23_telemetry-0.1.1.tar", max compression
```

## Comparing `f1_23_telemetry-0.1.0.tar` & `f1_23_telemetry-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-16 09:50:47.607310 f1_23_telemetry-0.1.0/LICENSE
--rw-r--r--   0        0        0      665 2023-07-30 14:56:19.534746 f1_23_telemetry-0.1.0/README.md
--rw-r--r--   0        0        0       31 2023-08-08 16:42:35.020420 f1_23_telemetry-0.1.0/f1_23_telemetry/__init__.py
--rw-r--r--   0        0        0    14825 2023-06-16 09:51:07.171882 f1_23_telemetry-0.1.0/f1_23_telemetry/appendices.py
--rw-r--r--   0        0        0      861 2023-06-16 10:04:07.680739 f1_23_telemetry-0.1.0/f1_23_telemetry/listener.py
--rw-r--r--   0        0        0      759 2023-06-16 07:50:35.705525 f1_23_telemetry-0.1.0/f1_23_telemetry/main.py
--rw-r--r--   0        0        0    59696 2023-06-16 09:51:49.285333 f1_23_telemetry-0.1.0/f1_23_telemetry/packets.py
--rw-r--r--   0        0        0     1289 2023-07-30 15:04:57.705150 f1_23_telemetry-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 f1_23_telemetry-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-16 09:50:47.607310 f1_23_telemetry-0.1.1/LICENSE
+-rw-r--r--   0        0        0      665 2023-07-30 14:56:19.534746 f1_23_telemetry-0.1.1/README.md
+-rw-r--r--   0        0        0       31 2023-08-08 16:42:35.020420 f1_23_telemetry-0.1.1/f1_23_telemetry/__init__.py
+-rw-r--r--   0        0        0    14825 2023-06-16 09:51:07.171882 f1_23_telemetry-0.1.1/f1_23_telemetry/appendices.py
+-rw-r--r--   0        0        0      861 2023-06-16 10:04:07.680739 f1_23_telemetry-0.1.1/f1_23_telemetry/listener.py
+-rw-r--r--   0        0        0      759 2023-06-16 07:50:35.705525 f1_23_telemetry-0.1.1/f1_23_telemetry/main.py
+-rw-r--r--   0        0        0    59696 2023-06-16 09:51:49.285333 f1_23_telemetry-0.1.1/f1_23_telemetry/packets.py
+-rw-r--r--   0        0        0     1289 2023-08-08 16:51:44.379844 f1_23_telemetry-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 f1_23_telemetry-0.1.1/PKG-INFO
```

### Comparing `f1_23_telemetry-0.1.0/LICENSE` & `f1_23_telemetry-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/README.md` & `f1_23_telemetry-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/f1_23_telemetry/appendices.py` & `f1_23_telemetry-0.1.1/f1_23_telemetry/appendices.py`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/f1_23_telemetry/listener.py` & `f1_23_telemetry-0.1.1/f1_23_telemetry/listener.py`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/f1_23_telemetry/main.py` & `f1_23_telemetry-0.1.1/f1_23_telemetry/main.py`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/f1_23_telemetry/packets.py` & `f1_23_telemetry-0.1.1/f1_23_telemetry/packets.py`

 * *Files identical despite different names*

### Comparing `f1_23_telemetry-0.1.0/pyproject.toml` & `f1_23_telemetry-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "f1-23-telemetry"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
   { name="Chris Hannam", email="ch@chrishannam.co.uk" },
 ]
 description = "Decode F1 23 telemetry data."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -36,15 +36,15 @@
   )/
 )
 '''
 skip-string-normalization = true
 
 [tool.poetry]
 name = "f1-23-telemetry"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Chris Hannam <ch@chrishannam.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "f1_23_telemetry"}]
 
 [tool.poetry.dependencies]
```

### Comparing `f1_23_telemetry-0.1.0/PKG-INFO` & `f1_23_telemetry-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f1-23-telemetry
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: Chris Hannam
 Author-email: ch@chrishannam.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


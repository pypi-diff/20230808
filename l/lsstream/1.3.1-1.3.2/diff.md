# Comparing `tmp/lsstream-1.3.1.tar.gz` & `tmp/lsstream-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.3.1.tar", last modified: Tue Aug  8 20:10:13 2023, max compression
+gzip compressed data, was "lsstream-1.3.2.tar", last modified: Tue Aug  8 20:32:43 2023, max compression
```

## Comparing `lsstream-1.3.1.tar` & `lsstream-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 20:10:03.000000 lsstream-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:10:13.620274 lsstream-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 20:10:03.000000 lsstream-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 20:10:03.000000 lsstream-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:10:13.620274 lsstream-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.616274 lsstream-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:32:43.846671 lsstream-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 20:32:34.000000 lsstream-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:32:43.846671 lsstream-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 20:32:34.000000 lsstream-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 20:32:34.000000 lsstream-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:32:43.846671 lsstream-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:32:43.842671 lsstream-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:32:43.846671 lsstream-1.3.2/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 20:32:34.000000 lsstream-1.3.2/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:32:43.846671 lsstream-1.3.2/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:32:43.000000 lsstream-1.3.2/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 20:32:43.000000 lsstream-1.3.2/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:32:43.000000 lsstream-1.3.2/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:32:43.000000 lsstream-1.3.2/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 20:32:43.000000 lsstream-1.3.2/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.3.1/LICENSE` & `lsstream-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/PKG-INFO` & `lsstream-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.3.1
+Version: 1.3.2
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsstream-1.3.1/README.md` & `lsstream-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/pyproject.toml` & `lsstream-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.3.1/src/lsstream/file_generation.py` & `lsstream-1.3.2/src/lsstream/file_generation.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/src/lsstream/prompts.py` & `lsstream-1.3.2/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/src/lsstream/run.py` & `lsstream-1.3.2/src/lsstream/run.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/src/lsstream/test.py` & `lsstream-1.3.2/src/lsstream/test.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.1/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.3.2/src/lsstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.3.1
+Version: 1.3.2
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


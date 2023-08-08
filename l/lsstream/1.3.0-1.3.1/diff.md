# Comparing `tmp/lsstream-1.3.0.tar.gz` & `tmp/lsstream-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsstream-1.3.0.tar", last modified: Tue Aug  8 19:14:45 2023, max compression
+gzip compressed data, was "lsstream-1.3.1.tar", last modified: Tue Aug  8 20:10:13 2023, max compression
```

## Comparing `lsstream-1.3.0.tar` & `lsstream-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.878897 lsstream-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 19:14:35.000000 lsstream-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 19:14:45.878897 lsstream-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 19:14:35.000000 lsstream-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 19:14:35.000000 lsstream-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:14:45.878897 lsstream-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.874897 lsstream-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.874897 lsstream-1.3.0/src/lsstream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/file_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 19:14:35.000000 lsstream-1.3.0/src/lsstream/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:14:45.878897 lsstream-1.3.0/src/lsstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 19:14:45.000000 lsstream-1.3.0/src/lsstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 20:10:03.000000 lsstream-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:10:13.620274 lsstream-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-08 20:10:03.000000 lsstream-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 20:10:03.000000 lsstream-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:10:13.620274 lsstream-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.616274 lsstream-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/src/lsstream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/file_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 20:10:03.000000 lsstream-1.3.1/src/lsstream/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:10:13.620274 lsstream-1.3.1/src/lsstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 20:10:13.000000 lsstream-1.3.1/src/lsstream.egg-info/top_level.txt
```

### Comparing `lsstream-1.3.0/LICENSE` & `lsstream-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.0/PKG-INFO` & `lsstream-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.3.0
+Version: 1.3.1
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lsstream-1.3.0/README.md` & `lsstream-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.0/pyproject.toml` & `lsstream-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lsstream"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Wermutton", email="redacted@redacted.redacted" },
 ]
 description = "To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `lsstream-1.3.0/src/lsstream/file_generation.py` & `lsstream-1.3.1/src/lsstream/file_generation.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.0/src/lsstream/prompts.py` & `lsstream-1.3.1/src/lsstream/prompts.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.0/src/lsstream/run.py` & `lsstream-1.3.1/src/lsstream/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                     os.remove('temp.html')
                 lsstream()
                 break
             elif continue_prompt.lower() == 'd':
                 if os.path.exists('temp.html'):
                     os.remove('temp.html')
                     
-                print(color(f'\n✔ Done!', 'green'))
+                print(color(f'\nGreat work!', None))
                 break
             else:
                 print(color('\nInvalid option, please choose A, B, C or D.', 'red'))
                 
 
 def lsstream():    
     new_files, new_contents = create_content()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lsstream-1.3.0/src/lsstream/test.py` & `lsstream-1.3.1/src/lsstream/test.py`

 * *Files identical despite different names*

### Comparing `lsstream-1.3.0/src/lsstream.egg-info/PKG-INFO` & `lsstream-1.3.1/src/lsstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsstream
-Version: 1.3.0
+Version: 1.3.1
 Summary: To help lazy tech boys and girls at ASU's SILC LSS with Streaming Requests 😴 🖥️ 🎞️
 Author-email: Wermutton <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/Wermutton/lsstream
 Project-URL: Bug Tracker, https://github.com/Wermutton/lsstream/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


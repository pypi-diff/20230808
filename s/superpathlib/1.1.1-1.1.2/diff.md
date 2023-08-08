# Comparing `tmp/superpathlib-1.1.1.tar.gz` & `tmp/superpathlib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.1.1.tar", last modified: Sun Aug  6 22:09:12 2023, max compression
+gzip compressed data, was "superpathlib-1.1.2.tar", last modified: Tue Aug  8 02:36:53 2023, max compression
```

## Comparing `superpathlib-1.1.1.tar` & `superpathlib-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:09:12.537050 superpathlib-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-06 22:08:58.000000 superpathlib-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-06 22:09:12.537050 superpathlib-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-06 22:08:58.000000 superpathlib-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:09:12.537050 superpathlib-1.1.1/plib/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/common_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/content_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/extra_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/metadata_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-06 22:08:58.000000 superpathlib-1.1.1/plib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-06 22:08:58.000000 superpathlib-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 22:09:12.537050 superpathlib-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:09:12.537050 superpathlib-1.1.1/superpathlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-06 22:09:12.000000 superpathlib-1.1.1/superpathlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-06 22:09:12.000000 superpathlib-1.1.1/superpathlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 22:09:12.000000 superpathlib-1.1.1/superpathlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-06 22:09:12.000000 superpathlib-1.1.1/superpathlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-06 22:09:12.000000 superpathlib-1.1.1/superpathlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 22:09:12.537050 superpathlib-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-06 22:08:58.000000 superpathlib-1.1.1/tests/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-06 22:08:58.000000 superpathlib-1.1.1/tests/test_encrypted_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-06 22:08:58.000000 superpathlib-1.1.1/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-06 22:08:58.000000 superpathlib-1.1.1/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:36:53.079917 superpathlib-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 02:36:39.000000 superpathlib-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-08 02:36:53.079917 superpathlib-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-08 02:36:39.000000 superpathlib-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:36:53.075917 superpathlib-1.1.2/plib/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/common_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/content_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/extra_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/metadata_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-08-08 02:36:39.000000 superpathlib-1.1.2/plib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 02:36:39.000000 superpathlib-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 02:36:53.079917 superpathlib-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:36:53.079917 superpathlib-1.1.2/superpathlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-08 02:36:53.000000 superpathlib-1.1.2/superpathlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 02:36:53.000000 superpathlib-1.1.2/superpathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 02:36:53.000000 superpathlib-1.1.2/superpathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 02:36:53.000000 superpathlib-1.1.2/superpathlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 02:36:53.000000 superpathlib-1.1.2/superpathlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 02:36:53.079917 superpathlib-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-08-08 02:36:39.000000 superpathlib-1.1.2/tests/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-08 02:36:39.000000 superpathlib-1.1.2/tests/test_encrypted_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-08 02:36:39.000000 superpathlib-1.1.2/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 02:36:39.000000 superpathlib-1.1.2/tests/test_metadata.py
```

### Comparing `superpathlib-1.1.1/LICENSE` & `superpathlib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/PKG-INFO` & `superpathlib-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Superpathlib
-Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
+Maximize your productivity using minimal code!
+
+Superpathlib enhances file operations, making them more intuitive and easy to implement. 
+This library builds upon Python's standard library [pathlib](https://docs.python.org/3/library/pathlib.html) module, offering an expansive range of added features without compromising performance.
 
 ## Usage
 
 ```shell
 from plib import Path
+
 path = Path(filename)
 ```
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
@@ -90,27 +94,27 @@
 for git_path in root.find(condition):
     process_git(git_path)
 ```
 ### 5) Enhance existing functionality
 * Automatically create parents when writing files, creating new files, renaming files, ..
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
-### 6) Inherit from Path to define your own additional functionality:
+### 6) Inherit from plib Path to define your own additional functionality:
 
 example: 
 
 ```shell
 import plib
 
 class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib Path, not the standard library pathlib Path
+This only works if you inherit from plib Path, not pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.1.1/README.md` & `superpathlib-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Superpathlib
-Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
+Maximize your productivity using minimal code!
+
+Superpathlib enhances file operations, making them more intuitive and easy to implement. 
+This library builds upon Python's standard library [pathlib](https://docs.python.org/3/library/pathlib.html) module, offering an expansive range of added features without compromising performance.
 
 ## Usage
 
 ```shell
 from plib import Path
+
 path = Path(filename)
 ```
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
@@ -77,27 +81,27 @@
 for git_path in root.find(condition):
     process_git(git_path)
 ```
 ### 5) Enhance existing functionality
 * Automatically create parents when writing files, creating new files, renaming files, ..
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
-### 6) Inherit from Path to define your own additional functionality:
+### 6) Inherit from plib Path to define your own additional functionality:
 
 example: 
 
 ```shell
 import plib
 
 class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib Path, not the standard library pathlib Path
+This only works if you inherit from plib Path, not pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.1.1/plib/common_folders.py` & `superpathlib-1.1.2/plib/common_folders.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/content_properties.py` & `superpathlib-1.1.2/plib/content_properties.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/encryption.py` & `superpathlib-1.1.2/plib/encryption.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/extra_functionality.py` & `superpathlib-1.1.2/plib/extra_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/metadata_properties.py` & `superpathlib-1.1.2/plib/metadata_properties.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/override.py` & `superpathlib-1.1.2/plib/override.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/tags.py` & `superpathlib-1.1.2/plib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/plib/utils.py` & `superpathlib-1.1.2/plib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/pyproject.toml` & `superpathlib-1.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [project]
 name = "superpathlib"
-version = "1.1.1"
+version = "1.1.2"
 description = "Extended Pathlib"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies = []
 
 [project.urls]
 "Source Code" = "https://github.com/quintenroets/superpathlib"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
```

### Comparing `superpathlib-1.1.1/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.1.2/superpathlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Superpathlib
-Superpathlib offers Path objects with functionality extended from pathlib to maximize your productivity with a minimal amount of code.
+Maximize your productivity using minimal code!
+
+Superpathlib enhances file operations, making them more intuitive and easy to implement. 
+This library builds upon Python's standard library [pathlib](https://docs.python.org/3/library/pathlib.html) module, offering an expansive range of added features without compromising performance.
 
 ## Usage
 
 ```shell
 from plib import Path
+
 path = Path(filename)
 ```
 
 ### 1) Use properties to read & write path content in different formats
 * text
 * byte_content
 * lines
@@ -90,27 +94,27 @@
 for git_path in root.find(condition):
     process_git(git_path)
 ```
 ### 5) Enhance existing functionality
 * Automatically create parents when writing files, creating new files, renaming files, ..
 * Return default values when path does not exist (e.g. size = 0, lines=[])
 
-### 6) Inherit from Path to define your own additional functionality:
+### 6) Inherit from plib Path to define your own additional functionality:
 
 example: 
 
 ```shell
 import plib
 
 class Path(plib.Path):
     def count_children(self):
         return sum(1 for _ in self.iterdir())
 ```
 
-This only works if you inherit from plib Path, not the standard library pathlib Path
+This only works if you inherit from plib Path, not pathlib Path
 
 
 ## Installation
 
 ```shell
 pip install superpathlib
 ```
```

### Comparing `superpathlib-1.1.1/superpathlib.egg-info/SOURCES.txt` & `superpathlib-1.1.2/superpathlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/tests/test_content.py` & `superpathlib-1.1.2/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/tests/test_encrypted_content.py` & `superpathlib-1.1.2/tests/test_encrypted_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/tests/test_functionality.py` & `superpathlib-1.1.2/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.1.1/tests/test_metadata.py` & `superpathlib-1.1.2/tests/test_metadata.py`

 * *Files identical despite different names*


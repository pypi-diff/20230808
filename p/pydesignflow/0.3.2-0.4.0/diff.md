# Comparing `tmp/pydesignflow-0.3.2.tar.gz` & `tmp/pydesignflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydesignflow-0.3.2.tar", last modified: Fri Mar 24 09:48:20 2023, max compression
+gzip compressed data, was "pydesignflow-0.4.0.tar", last modified: Tue Aug  8 12:12:03 2023, max compression
```

## Comparing `pydesignflow-0.3.2.tar` & `pydesignflow-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/
--rw-r--r--   0 tobias    (1000) tobias    (1000)    11358 2022-07-17 09:38:32.000000 pydesignflow-0.3.2/LICENSE
--rw-r--r--   0 tobias    (1000) tobias    (1000)      411 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/PKG-INFO
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1243 2022-09-19 14:40:21.000000 pydesignflow-0.3.2/README.rst
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/pydesignflow/
--rw-r--r--   0 tobias    (1000) tobias    (1000)      203 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/pydesignflow/__init__.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)      291 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/pydesignflow/ansiterm.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     2800 2022-12-09 16:18:24.000000 pydesignflow-0.3.2/pydesignflow/block.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3506 2023-03-10 11:21:13.000000 pydesignflow-0.3.2/pydesignflow/cli.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)      264 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/pydesignflow/errors.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3806 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/pydesignflow/filemgmt.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     2005 2023-03-10 11:13:33.000000 pydesignflow-0.3.2/pydesignflow/flow.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3176 2023-02-23 09:49:27.000000 pydesignflow-0.3.2/pydesignflow/result.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     7598 2023-03-24 09:43:32.000000 pydesignflow-0.3.2/pydesignflow/session.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1186 2022-12-09 16:18:24.000000 pydesignflow-0.3.2/pydesignflow/shortcut.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     4997 2022-12-09 16:18:24.000000 pydesignflow-0.3.2/pydesignflow/sphinx_ext.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3900 2023-02-23 12:10:55.000000 pydesignflow-0.3.2/pydesignflow/target.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     1039 2023-02-23 12:10:18.000000 pydesignflow-0.3.2/pydesignflow/task.py
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/pydesignflow.egg-info/
--rw-r--r--   0 tobias    (1000) tobias    (1000)      411 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) tobias    (1000)      746 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)        1 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       52 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       16 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       19 2023-03-24 09:48:20.000000 pydesignflow-0.3.2/pydesignflow.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) tobias    (1000)       38 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/setup.cfg
--rw-r--r--   0 tobias    (1000) tobias    (1000)      681 2023-03-24 09:47:30.000000 pydesignflow-0.3.2/setup.py
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/tests/
--rw-r--r--   0 tobias    (1000) tobias    (1000)        0 2022-07-17 09:38:32.000000 pydesignflow-0.3.2/tests/__init__.py
-drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-03-24 09:48:20.455038 pydesignflow-0.3.2/tests/flow_example1/
--rw-r--r--   0 tobias    (1000) tobias    (1000)      115 2022-09-19 11:29:50.000000 pydesignflow-0.3.2/tests/flow_example1/__init__.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     2212 2022-09-19 22:40:04.000000 pydesignflow-0.3.2/tests/flow_example1/example_block.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3022 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/tests/test_dependency_list.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)      579 2023-03-10 11:22:05.000000 pydesignflow-0.3.2/tests/test_exitcode.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     3490 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/tests/test_multiple_blocks.py
--rw-r--r--   0 tobias    (1000) tobias    (1000)     2029 2022-12-21 16:37:04.000000 pydesignflow-0.3.2/tests/test_single_block.py
+drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)    11358 2022-09-20 08:42:05.000000 pydesignflow-0.4.0/LICENSE
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      411 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/PKG-INFO
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     2352 2023-08-08 09:37:56.000000 pydesignflow-0.4.0/README.rst
+drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-08-08 12:12:03.178181 pydesignflow-0.4.0/pydesignflow/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      237 2023-08-08 12:07:17.000000 pydesignflow-0.4.0/pydesignflow/__init__.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      291 2023-02-08 17:01:25.000000 pydesignflow-0.4.0/pydesignflow/ansiterm.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3121 2023-08-08 08:59:54.000000 pydesignflow-0.4.0/pydesignflow/block.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3506 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/pydesignflow/cli.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      264 2023-02-08 17:01:25.000000 pydesignflow-0.4.0/pydesignflow/errors.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     4509 2023-08-08 11:52:45.000000 pydesignflow-0.4.0/pydesignflow/filemgmt.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     2005 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/pydesignflow/flow.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3181 2023-08-08 10:25:51.000000 pydesignflow-0.4.0/pydesignflow/result.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     7598 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/pydesignflow/session.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     1186 2022-09-20 10:05:39.000000 pydesignflow-0.4.0/pydesignflow/shortcut.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     4997 2022-09-20 12:29:01.000000 pydesignflow-0.4.0/pydesignflow/sphinx_ext.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3900 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/pydesignflow/target.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     1039 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/pydesignflow/task.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)       21 2023-08-08 12:07:21.000000 pydesignflow-0.4.0/pydesignflow/version.py
+drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/pydesignflow.egg-info/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      411 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      814 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) tobias    (1000)        1 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) tobias    (1000)       52 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) tobias    (1000)       16 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) tobias    (1000)       19 2023-08-08 12:12:03.000000 pydesignflow-0.4.0/pydesignflow.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) tobias    (1000)       38 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/setup.cfg
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      749 2023-08-08 12:07:08.000000 pydesignflow-0.4.0/setup.py
+drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/tests/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)        0 2022-09-20 08:42:06.000000 pydesignflow-0.4.0/tests/__init__.py
+drwxr-xr-x   0 tobias    (1000) tobias    (1000)        0 2023-08-08 12:12:03.182181 pydesignflow-0.4.0/tests/flow_example1/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      115 2022-09-20 08:42:06.000000 pydesignflow-0.4.0/tests/flow_example1/__init__.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     2212 2022-09-20 08:42:06.000000 pydesignflow-0.4.0/tests/flow_example1/example_block.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3022 2023-02-08 17:01:25.000000 pydesignflow-0.4.0/tests/test_dependency_list.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)      579 2023-03-27 14:52:49.000000 pydesignflow-0.4.0/tests/test_exitcode.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     2104 2023-08-08 11:53:19.000000 pydesignflow-0.4.0/tests/test_filemgmt.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     3490 2023-08-08 09:57:40.000000 pydesignflow-0.4.0/tests/test_multiple_blocks.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     1433 2023-08-08 11:18:23.000000 pydesignflow-0.4.0/tests/test_result.py
+-rw-r--r--   0 tobias    (1000) tobias    (1000)     2029 2023-02-08 17:01:25.000000 pydesignflow-0.4.0/tests/test_single_block.py
```

### Comparing `pydesignflow-0.3.2/LICENSE` & `pydesignflow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/block.py` & `pydesignflow-0.4.0/pydesignflow/block.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,22 @@
     def auto_register_tasks(self):
         """
         Registers all Target objects in the .tasks dictionary.
 
         Alternately, a similar automatic detection can be implemented using a
         metaclass and __prepare__.
         """
+        ordered_keys = list(type(self).__dict__.keys())
+        # This does not cover type(self).__dict__ does not cover everything,
+        # so if there are missing keys, add them at the end of the list:
         for key in dir(self):
+            if key not in ordered_keys:
+                ordered_keys.append(key)
+
+        for key in ordered_keys:
             val = getattr(self, key)
             if isinstance(val, TargetPrototype):
                 # Bidirectional reference:
                 act = val.create()
                 act.register(self, key)
                 self.tasks[key] = act
```

### Comparing `pydesignflow-0.3.2/pydesignflow/cli.py` & `pydesignflow-0.4.0/pydesignflow/cli.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/filemgmt.py` & `pydesignflow-0.4.0/pydesignflow/filemgmt.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 from dataclasses import dataclass
 import re
 
 class FileManagementError(Exception):
     pass
 
 def checkfile(path: Path) -> Path:
+    """
+    Convenience function: check that path exists and is a file, then return path.
+    """
     if not path.exists():
         raise FileManagementError(f"Path '{path}' does not exist.")
     if not path.is_file():
         raise FileManagementError(f"'{path}' is not a file.")
     return path
 
 def checkdir(path: Path) -> Path:
+    """
+    Convenience function: check that path exists and is a directory, then return path.
+    """
     if not path.exists():
         raise FileManagementError(f"Path '{path}' does not exist.")
     if not path.is_dir():
         raise FileManagementError(f"'{path}' is not a directory.")
     return path
 
 @dataclass
@@ -86,17 +92,17 @@
                         return False
             return True
         
         return FileCollection(list(filter(filter_func, self.items)))
 
     def one(self, missing_key_deselects: bool = False, **filters: dict[str, object]):
         """
-        Returns element that matches **filters.
+        Returns element that matches filters.
 
-        Raises FileManagementError if **filters are ambiguous (multiple matches) or when no match is found.
+        Raises FileManagementError if filters are ambiguous (multiple matches) or when no match is found.
         """
         res = self.filter(missing_key_deselects=missing_key_deselects, **filters)
         if len(res) < 1:
             raise FileManagementError(f"No result for FileCollection filters {filters}.")
         elif len(res) > 1:
             raise FileManagementError(f"Ambiguous result for FileCollection filters {filters}.")
         else:
@@ -105,15 +111,29 @@
     def __call__(self, *args, **kwargs):
         """
         Alias for .one()
         """
         return self.one(*args, **kwargs)
 
     @classmethod
-    def frompattern(cls, dir, pattern, decoder):
+    def frompattern(cls, dir: Path, pattern: str, decoder):
+        """
+        Create FileCollection using pattern and decoder function.
+
+        Args:
+            dir: Directory (Path) in which to locate files.
+            pattern: Regular expression (Python's re module) for finding
+                desired files.
+            decoder: Decoder function, receives first regular expression
+                group string as argument, returns dictionary of file
+                attributes.
+
+        Returns:
+            new FileCollection object
+        """
         coll = cls()
 
         for fn in dir.iterdir():
             m = re.match(pattern, fn.name)
             if m:
                 attr_str = m.group(1)
                 attrs = decoder(attr_str)
```

### Comparing `pydesignflow-0.3.2/pydesignflow/flow.py` & `pydesignflow-0.4.0/pydesignflow/flow.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/result.py` & `pydesignflow-0.4.0/pydesignflow/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 import json
 from datetime import datetime
 
 
 class Result:
     supported_scalar_types = (
-        Path, str, bool, float, datetime
+        str, bool, int, float, Path, datetime
     )
 
     def __init__(self):
         self.__dict__["attrs"] = {}
 
     def check_value(self, value):
         if isinstance(value, (list, tuple)):
```

### Comparing `pydesignflow-0.3.2/pydesignflow/session.py` & `pydesignflow-0.4.0/pydesignflow/session.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/shortcut.py` & `pydesignflow-0.4.0/pydesignflow/shortcut.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/sphinx_ext.py` & `pydesignflow-0.4.0/pydesignflow/sphinx_ext.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/target.py` & `pydesignflow-0.4.0/pydesignflow/target.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow/task.py` & `pydesignflow-0.4.0/pydesignflow/task.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/pydesignflow.egg-info/SOURCES.txt` & `pydesignflow-0.4.0/pydesignflow.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 pydesignflow/flow.py
 pydesignflow/result.py
 pydesignflow/session.py
 pydesignflow/shortcut.py
 pydesignflow/sphinx_ext.py
 pydesignflow/target.py
 pydesignflow/task.py
+pydesignflow/version.py
 pydesignflow.egg-info/PKG-INFO
 pydesignflow.egg-info/SOURCES.txt
 pydesignflow.egg-info/dependency_links.txt
 pydesignflow.egg-info/entry_points.txt
 pydesignflow.egg-info/requires.txt
 pydesignflow.egg-info/top_level.txt
 tests/__init__.py
 tests/test_dependency_list.py
 tests/test_exitcode.py
+tests/test_filemgmt.py
 tests/test_multiple_blocks.py
+tests/test_result.py
 tests/test_single_block.py
 tests/flow_example1/__init__.py
 tests/flow_example1/example_block.py
```

### Comparing `pydesignflow-0.3.2/setup.py` & `pydesignflow-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import setuptools
 
+exec(open('pydesignflow/version.py').read()) # --> __version__
+
 setuptools.setup(
     name="pydesignflow",
-    version="0.3.2",
+    version=__version__,
     author="Tobias Kaiser",
     author_email="mail@tb-kaiser.de",
     description="Micro-Framework for FPGA / VLSI Design Flow in Python",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
```

### Comparing `pydesignflow-0.3.2/tests/flow_example1/example_block.py` & `pydesignflow-0.4.0/tests/flow_example1/example_block.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/tests/test_dependency_list.py` & `pydesignflow-0.4.0/tests/test_dependency_list.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/tests/test_exitcode.py` & `pydesignflow-0.4.0/tests/test_exitcode.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/tests/test_multiple_blocks.py` & `pydesignflow-0.4.0/tests/test_multiple_blocks.py`

 * *Files identical despite different names*

### Comparing `pydesignflow-0.3.2/tests/test_single_block.py` & `pydesignflow-0.4.0/tests/test_single_block.py`

 * *Files identical despite different names*


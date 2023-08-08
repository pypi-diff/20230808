# Comparing `tmp/motion_python-0.1.85.tar.gz` & `tmp/motion_python-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.85.tar", max compression
+gzip compressed data, was "motion_python-0.1.86.tar", max compression
```

## Comparing `motion_python-0.1.85.tar` & `motion_python-0.1.86.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3344 2023-07-25 23:36:10.411189 motion_python-0.1.85/README.md
--rw-r--r--   0        0        0      344 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/cli.py
--rw-r--r--   0        0        0    24251 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/component.py
--rw-r--r--   0        0        0     4623 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/dicts.py
--rw-r--r--   0        0        0    17268 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/execute.py
--rw-r--r--   0        0        0    13682 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/instance.py
--rw-r--r--   0        0        0     4897 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1153 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/route.py
--rw-r--r--   0        0        0     4574 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/server/update_task.py
--rw-r--r--   0        0        0    10020 2023-07-25 23:36:10.411189 motion_python-0.1.85/motion/utils.py
--rw-r--r--   0        0        0     1782 2023-07-25 23:36:36.546854 motion_python-0.1.85/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 motion_python-0.1.85/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-08-08 21:23:42.872283 motion_python-0.1.86/README.md
+-rw-r--r--   0        0        0      344 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/cli.py
+-rw-r--r--   0        0        0    24251 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/component.py
+-rw-r--r--   0        0        0     4623 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/dicts.py
+-rw-r--r--   0        0        0    17269 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/execute.py
+-rw-r--r--   0        0        0    13682 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/instance.py
+-rw-r--r--   0        0        0     4897 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1153 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/route.py
+-rw-r--r--   0        0        0     4574 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/server/update_task.py
+-rw-r--r--   0        0        0    10020 2023-08-08 21:23:42.876283 motion_python-0.1.86/motion/utils.py
+-rw-r--r--   0        0        0     1782 2023-08-08 21:24:05.012693 motion_python-0.1.86/pyproject.toml
+-rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 motion_python-0.1.86/PKG-INFO
```

### Comparing `motion_python-0.1.85/README.md` & `motion_python-0.1.86/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/cli.py` & `motion_python-0.1.86/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/component.py` & `motion_python-0.1.86/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/dicts.py` & `motion_python-0.1.86/motion/dicts.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/execute.py` & `motion_python-0.1.86/motion/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if self.disabled:
             return
 
         if not self.running.value:
             return
 
         if is_open:
-            logger.info("Running update operations on remaining data...")
+            logger.debug("Running update operations on remaining data...")
 
         # Set shutdown event
         self.stop_event.set()
         self.running.value = False
 
         if self.worker_task and psutil.pid_exists(self.worker_task.pid):
             self.worker_task.join()
```

### Comparing `motion_python-0.1.85/motion/instance.py` & `motion_python-0.1.86/motion/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import atexit
 import logging
-
 from typing import Any, Awaitable, Callable, Dict, List, Optional
 
 from motion.execute import Executor
 from motion.route import Route
 from motion.utils import DEFAULT_KEY_TTL, configureLogging, logger
 
 
@@ -119,15 +118,15 @@
 
         if not self.running:
             return
 
         is_open = is_logger_open(logger)
 
         if is_open:
-            logger.info(f"Shutting down {self._instance_name}...")
+            logger.debug(f"Shutting down {self._instance_name}...")
 
         self._executor.shutdown(is_open=is_open)
 
         self.running = False
 
     def get_version(self) -> int:
         """
```

### Comparing `motion_python-0.1.85/motion/migrate.py` & `motion_python-0.1.86/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.86/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/route.py` & `motion_python-0.1.86/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/server/update_task.py` & `motion_python-0.1.86/motion/server/update_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/motion/utils.py` & `motion_python-0.1.86/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.85/pyproject.toml` & `motion_python-0.1.86/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.85"
+version = "0.1.86"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.85/PKG-INFO` & `motion_python-0.1.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.85
+Version: 0.1.86
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


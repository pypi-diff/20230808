# Comparing `tmp/robotcode_robot-0.49.0.tar.gz` & `tmp/robotcode_robot-0.50.0.tar.gz`

## Comparing `robotcode_robot-0.49.0.tar` & `robotcode_robot-0.50.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    80002 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/LICENSE.txt
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/README.md
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 robotcode_robot-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    80002 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/LICENSE.txt
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/README.md
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 robotcode_robot-0.50.0/PKG-INFO
```

### Comparing `robotcode_robot-0.49.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.50.0/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.49.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.50.0/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.49.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.50.0/src/robotcode/robot/config/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,40 +28,34 @@
     return result
 
 
 def get_config_files(
     paths: Optional[Sequence[Union[str, Path]]] = None,
     config_files: Optional[Sequence[Path]] = None,
     *,
-    raise_on_error: bool = True,
     verbose_callback: Optional[Callable[[str], None]] = None,
 ) -> Tuple[Sequence[Tuple[Path, ConfigType]], Optional[Path], DiscoverdBy]:
     root_folder, discovered_by = find_project_root(*(paths or []))
 
     if root_folder is None:
-        if raise_on_error:
-            raise FileNotFoundError("Cannot detect root folder. 😥")
+        root_folder = Path.cwd()
         if verbose_callback:
-            verbose_callback("Cannot detect root folder. 😥")
-        return [], None, DiscoverdBy.NOT_FOUND
+            verbose_callback(f"Cannot detect root folder. Use current folder '{root_folder}' as root.")
 
     if verbose_callback:
         verbose_callback(f"Found root at:\n    {root_folder} ({discovered_by.value})")
 
     if config_files:
         if verbose_callback:
             verbose_callback("Using config file:" + "\n    ".join([str(f) for f in config_files]))
 
         result: Sequence[Tuple[Path, ConfigType]] = [(f, ConfigType.CUSTOM_TOML) for f in config_files]
     else:
         result = get_config_files_from_folder(root_folder)
 
-        if not result and raise_on_error:
-            raise FileNotFoundError("Cannot find any configuration file. 😥")
-
         if verbose_callback:
             if result:
                 verbose_callback(
                     "Found configuration files:\n    " + "\n    ".join(str(f[0]) for f in result),
                 )
             else:
                 verbose_callback("No configuration files found.")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `robotcode_robot-0.49.0/.gitignore` & `robotcode_robot-0.50.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.49.0/LICENSE.txt` & `robotcode_robot-0.50.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.49.0/README.md` & `robotcode_robot-0.50.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.49.0/pyproject.toml` & `robotcode_robot-0.50.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
   "platformdirs<3.9.0,>=3.2.0",
-  "robotcode-core==0.49.0",
+  "robotcode-core==0.50.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
```

### Comparing `robotcode_robot-0.49.0/PKG-INFO` & `robotcode_robot-0.50.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-robot
-Version: 0.49.0
+Version: 0.50.0
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: platformdirs<3.9.0,>=3.2.0
-Requires-Dist: robotcode-core==0.49.0
+Requires-Dist: robotcode-core==0.50.0
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```


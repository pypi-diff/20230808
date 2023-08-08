# Comparing `tmp/amhelpers-0.2.5.tar.gz` & `tmp/amhelpers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amhelpers-0.2.5.tar", max compression
+gzip compressed data, was "amhelpers-0.4.0.tar", max compression
```

## Comparing `amhelpers-0.2.5.tar` & `amhelpers-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rwxr-xr-x   0        0        0     1072 2022-05-30 13:43:08.846346 amhelpers-0.2.5/LICENSE
--rw-r--r--   0        0        0      405 2022-05-30 13:43:55.780186 amhelpers-0.2.5/README.md
--rw-r--r--   0        0        0      588 2023-06-01 08:34:26.725673 amhelpers-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      111 2022-05-30 13:43:08.893968 amhelpers-0.2.5/src/amhelpers/__init__.py
--rw-r--r--   0        0        0     1936 2022-05-30 14:19:11.627209 amhelpers-0.2.5/src/amhelpers/amhelpers.py
--rw-r--r--   0        0        0     4236 2023-06-01 08:25:43.146994 amhelpers-0.2.5/src/amhelpers/config_parsing.py
--rw-r--r--   0        0        0      990 2023-06-01 08:36:37.080238 amhelpers-0.2.5/setup.py
--rw-r--r--   0        0        0      850 2023-06-01 08:36:37.080545 amhelpers-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2022-05-30 13:43:08.846346 amhelpers-0.4.0/LICENSE
+-rw-r--r--   0        0        0      405 2022-05-30 13:43:55.780186 amhelpers-0.4.0/README.md
+-rw-r--r--   0        0        0      677 2023-08-08 12:04:08.057065 amhelpers-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2022-05-30 13:43:08.893968 amhelpers-0.4.0/src/amhelpers/__init__.py
+-rw-r--r--   0        0        0     2522 2023-08-08 09:17:45.988457 amhelpers-0.4.0/src/amhelpers/amhelpers.py
+-rw-r--r--   0        0        0     5439 2023-08-08 09:16:50.023727 amhelpers-0.4.0/src/amhelpers/config_parsing.py
+-rw-r--r--   0        0        0    18042 2023-08-08 11:40:01.130625 amhelpers-0.4.0/src/amhelpers/experiment.py
+-rw-r--r--   0        0        0     1249 2023-08-08 12:07:25.730034 amhelpers-0.4.0/setup.py
+-rw-r--r--   0        0        0     1025 2023-08-08 12:07:25.730324 amhelpers-0.4.0/PKG-INFO
```

### Comparing `amhelpers-0.2.5/LICENSE` & `amhelpers-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amhelpers-0.2.5/pyproject.toml` & `amhelpers-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "amhelpers"
-version = "0.2.5"
+version = "0.4.0"
 description = "A collection of handy utilities."
 authors = ["Anton Matsson"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+numpy = {version = "^1.25.2", python = "^3.9"}
+scikit-learn = "^1.3.0"
+pandas = "^2.0.3"
 
 [tool.poetry.dev-dependencies]
 myst-nb = {version = "^0.15.0", python = "^3.8"}
 sphinx-autoapi = "^1.8.4"
 sphinx-rtd-theme = "^1.0.0"
 pytest = "^7.1.2"
 python-semantic-release = {version = "^7.29.0", python = "^3.8"}
```

### Comparing `amhelpers-0.2.5/src/amhelpers/amhelpers.py` & `amhelpers-0.4.0/src/amhelpers/amhelpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 import pydoc
+import yaml
+import pickle
+from os.path import join
+from pathlib import Path
 
 def create_object_from_dict(d, **default_kwargs):
     '''Create an object from a dictionary.
 
     Inspired by `iglovikov_helper_functions.config_parsing.utils`. [1]_
 
     Parameters
@@ -56,18 +60,33 @@
     ----------
     d : dict
         Nested dictionary.
 
     Returns
     -------
     generator
-        Iterator yielding all (non-dict) values from 'd' and its child dictionaries.
+        Iterator yielding all (non-dict) values from `d` and its child dictionaries.
 
     References
     ----------
     .. [2] https://tutorial.eyehunts.com/python/python-get-all-values-from-nested-dictionary-example-code/
     '''
     for v in d.values():
         if isinstance(v, dict):
             yield from yield_nested_dict_values(v)
         else:
             yield v
+
+def save_pickle(data, path, filename):
+    Path(path).mkdir(parents=True, exist_ok=True)
+    with open(join(path, filename + '.pickle'), 'wb') as f:
+        pickle.dump(data, f)
+
+def save_yaml(data, path, filename, **kwargs):
+    Path(path).mkdir(parents=True, exist_ok=True)
+    with open(join(path, filename + '.yaml'), 'w') as f:
+        yaml.dump(data, f, default_flow_style=False, **kwargs)
+
+def load_yaml(path):
+    with open(path) as file:
+        yaml_file = yaml.safe_load(file)
+    return yaml_file
```

### Comparing `amhelpers-0.2.5/src/amhelpers/config_parsing.py` & `amhelpers-0.4.0/src/amhelpers/config_parsing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+import os
 import copy
-from .amhelpers import get_class_from_str
-from .amhelpers import create_object_from_dict
+from pathlib import Path
+from .amhelpers import (
+    get_class_from_str,
+    create_object_from_dict,
+    load_yaml
+)
 
 NET_PARAMS = [
     'module',
     'criterion',
     'optimizer',
     'lr',
     'max_epochs',
@@ -130,7 +135,44 @@
             elif param in default:
                 params[param] = _check_value(default_value)
             else:
                 # Use skorch default
                 pass
 
     return params
+
+def _change_to_local_paths(d, cluster_project_path, local_project_path):
+    out = {}
+    for k, v in d.items():
+        if isinstance(v, dict):
+            recursive = {
+                k: _change_to_local_paths(
+                    v,
+                    cluster_project_path,
+                    local_project_path
+                )
+            }
+            out.update(recursive)
+        elif isinstance(k, str) and 'path' in k and isinstance(v, str):
+            out[k] = v.replace(
+                cluster_project_path,
+                local_project_path
+            )
+        else:
+            out[k] = v
+    return out
+
+def load_config(config_path):
+    config = load_yaml(config_path)
+    try:
+        local_home_path = os.environ['LOCAL_HOME_PATH']
+        cluster_project_path = os.environ['CLUSTER_PROJECT_PATH']
+        local_project_path = os.environ['LOCAL_PROJECT_PATH']
+        home_path = str(Path.home())
+        if home_path == local_home_path:
+            return _change_to_local_paths(
+                config,
+                cluster_project_path,
+                local_project_path
+            )
+    except KeyError:
+        return config
```

### Comparing `amhelpers-0.2.5/PKG-INFO` & `amhelpers-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: amhelpers
-Version: 0.2.5
+Version: 0.4.0
 Summary: A collection of handy utilities.
 License: MIT
 Author: Anton Matsson
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: numpy (>=1.25.2,<2.0.0); python_version >= "3.9" and python_version < "4.0"
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # amhelpers
 
 A collection of handy utilities.
 
 ## Installation
```


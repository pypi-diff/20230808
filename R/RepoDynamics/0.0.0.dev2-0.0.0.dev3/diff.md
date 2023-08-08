# Comparing `tmp/RepoDynamics-0.0.0.dev2.tar.gz` & `tmp/RepoDynamics-0.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepoDynamics-0.0.0.dev2.tar", last modified: Tue Aug  8 15:02:13 2023, max compression
+gzip compressed data, was "RepoDynamics-0.0.0.dev3.tar", last modified: Tue Aug  8 15:10:12 2023, max compression
```

## Comparing `RepoDynamics-0.0.0.dev2.tar` & `RepoDynamics-0.0.0.dev3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.768183 RepoDynamics-0.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:02:13.764183 RepoDynamics-0.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:02:13.768183 RepoDynamics-0.0.0.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.760183 RepoDynamics-0.0.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.764183 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 15:02:13.000000 RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.764183 RepoDynamics-0.0.0.dev2/src/repodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.764183 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/actions/meta_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/cd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:02:13.764183 RepoDynamics-0.0.0.dev2/src/repodynamics/files/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/files/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/files/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/files/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/format_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 15:02:04.000000 RepoDynamics-0.0.0.dev2/src/repodynamics/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:10:11.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 15:10:12.000000 RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.071517 RepoDynamics-0.0.0.dev3/src/repodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/cd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:10:12.075517 RepoDynamics-0.0.0.dev3/src/repodynamics/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/files/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/format_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-08 15:10:00.000000 RepoDynamics-0.0.0.dev3/src/repodynamics/workflow.py
```

### Comparing `RepoDynamics-0.0.0.dev2/pyproject.toml` & `RepoDynamics-0.0.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 where = ["src"]
 namespaces = true
 
 
 # ----------------------------------------- Project Metadata -------------------------------------
 #
 [project]
-version = "0.0.0.dev2"
+version = "0.0.0.dev3"
 name = "RepoDynamics"
 #dependencies = [
 #    # https://yaml.readthedocs.io/en/stable/
 #    "ruamel.yaml >= 0.17.32, < 0.18",
 #    # https://tomlkit.readthedocs.io/en/stable/
 #    "tomlkit >= 0.11.8, < 0.12",
 #    "trove-classifiers",
```

### Comparing `RepoDynamics-0.0.0.dev2/src/RepoDynamics.egg-info/SOURCES.txt` & `RepoDynamics-0.0.0.dev3/src/RepoDynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/actions/__main__.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/actions/context.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/context.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/actions/io.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             sys.exit(1)
         if typ is str:
             args[param] = val
         elif typ is bool:
             if isinstance(val, bool):
                 args[param] = val
             elif isinstance(val, str):
-                if val.lower() not in ("true", "false"):
+                if val.lower() not in ("true", "false", ""):
                     print(
                         "ERROR! Invalid boolean input: "
                         f"'{param_env_name}' has value '{val}' with type {type(val)}."
                     )
                     sys.exit(1)
                 args[param] = val.lower() == "true"
             else:
```

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/actions/meta.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/actions/meta_summary.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/actions/meta_summary.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/cd.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/cd.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/files/__main__.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/files/__main__.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/files/pyproject.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/files/pyproject.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/files/readme.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/files/readme.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/files/templates.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/files/templates.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/format_issue.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/format_issue.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/metadata.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/metadata.py`

 * *Files identical despite different names*

### Comparing `RepoDynamics-0.0.0.dev2/src/repodynamics/workflow.py` & `RepoDynamics-0.0.0.dev3/src/repodynamics/workflow.py`

 * *Files identical despite different names*


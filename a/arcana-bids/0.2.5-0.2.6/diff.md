# Comparing `tmp/arcana_bids-0.2.5.tar.gz` & `tmp/arcana_bids-0.2.6.tar.gz`

## Comparing `arcana_bids-0.2.5.tar` & `arcana_bids-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/_version.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/cli.py
--rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/data.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/deploy.py
--rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tasks.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_cli.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/arcana/bids/tests/test_tasks.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/LICENSE
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/README.rst
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/_version.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/cli.py
+-rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/data.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/deploy.py
+-rw-r--r--   0        0        0    15435 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tasks.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_cli.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_data.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/arcana/bids/tests/test_tasks.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/README.rst
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.6/PKG-INFO
```

### Comparing `arcana_bids-0.2.5/arcana/bids/cli.py` & `arcana_bids-0.2.6/arcana/bids/cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/arcana/bids/data.py` & `arcana_bids-0.2.6/arcana/bids/data.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/arcana/bids/tasks.py` & `arcana_bids-0.2.6/arcana/bids/tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/arcana/bids/tests/test_cli.py` & `arcana_bids-0.2.6/arcana/bids/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,36 +91,37 @@
         format_str = ClassResolver.tostr(datatype)
         varname = path2varname(path)
         inputs_config[varname] = {
             "configuration": {
                 "path": path,
             },
             "datatype": format_str,
-            "help_string": "dummy",
+            "help": "dummy",
         }
 
     outputs_config = {}
     for path, _, datatype, _ in blueprint.derivatives:
         format_str = ClassResolver.tostr(datatype)
         varname = path2varname(path)
         outputs_config[varname] = {
             "configuration": {
                 "path": path,
             },
             "datatype": format_str,
-            "help_string": "dummy",
+            "help": "dummy",
         }
 
     image_spec = App(
+        title="a test image",
         name="test_bids_app_entrypoint",
-        version="1.0",
-        build_iteration="1",
-        description="a test image",
+        version={"package": "1.0", "build": "1"},
         authors=[{"name": "Some One", "email": "some.one@an.email.org"}],
-        info_url="http://concatenate.readthefakedocs.io",
+        docs={
+            "info_url": "http://concatenate.readthefakedocs.io",
+        },
         command={
             "task": "arcana.bids.tasks:bids_app",
             "row_frequency": "medimage:Clinical[session]",
             "inputs": inputs_config,
             "outputs": outputs_config,
             "configuration": {
                 "executable": str(mock_bids_app_executable),
```

### Comparing `arcana_bids-0.2.5/arcana/bids/tests/test_data.py` & `arcana_bids-0.2.6/arcana/bids/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/arcana/bids/tests/test_tasks.py` & `arcana_bids-0.2.6/arcana/bids/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/LICENSE` & `arcana_bids-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/README.rst` & `arcana_bids-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/pyproject.toml` & `arcana_bids-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.5/PKG-INFO` & `arcana_bids-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-bids
-Version: 0.2.5
+Version: 0.2.6
 Summary: An Arcana extension for interacting with Brain Imaging Structure (BIDS) datasets and associated "Apps"
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-bids.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```


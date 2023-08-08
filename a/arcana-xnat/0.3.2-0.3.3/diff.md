# Comparing `tmp/arcana_xnat-0.3.2.tar.gz` & `tmp/arcana_xnat-0.3.3.tar.gz`

## Comparing `arcana_xnat-0.3.2.tar` & `arcana_xnat-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/base.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/entrypoint.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/update_release.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_add_columns.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_dataset_export.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_store.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_xnat_images.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/__init__.py
--rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/api.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/cs.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/tests/test_store.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/__init__.py
--rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/command.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/image.py
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/utils/__init__.py
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/utils/testing.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/.gitignore
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/LICENSE
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/README.rst
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/base.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/entrypoint.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/update_release.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_add_columns.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_dataset_export.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_xnat_images.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/__init__.py
+-rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/api.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/cs.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/data/tests/test_store.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/__init__.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/command.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/image.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/deploy/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/utils/__init__.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/arcana/xnat/utils/testing.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/.gitignore
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/README.rst
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.3/PKG-INFO
```

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/entrypoint.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/update_release.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/update_release.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_add_columns.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_add_columns.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_dataset_export.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_dataset_export.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_store.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_xnat_images.py` & `arcana_xnat-0.3.3/arcana/xnat/cli/tests/test_cli_xnat_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,24 @@
 
     for name, cmd_spec in (
         ("forward_concat-pullimages", command_spec),
         ("reverse_concat-pullimages", reverse_command_spec),
     ):
 
         image_spec = {
+            "title": "a command to test build process",
             "command": cmd_spec,
-            "version": PKG_VERSION,
-            "build_iteration": WRAPPER_VERSION,
+            "version": {
+                "package": PKG_VERSION,
+                "build": WRAPPER_VERSION,
+            },
             "authors": [{"name": "Some One", "email": "some.one@an.email.org"}],
-            "info_url": "http://concatenate.readthefakedocs.io",
-            "description": "a command to test build process",
+            "docs": {
+                "info_url": "http://concatenate.readthefakedocs.io",
+            }
         }
 
         with open((pkg_path / name).with_suffix(".yaml"), "w") as f:
             yaml.dump(image_spec, f)
 
         expected_images.append(
             f"{docker_registry_for_xnat_uri}/{DOCKER_ORG}/{IMAGE_GROUP_NAME}"
```

### Comparing `arcana_xnat-0.3.2/arcana/xnat/data/api.py` & `arcana_xnat-0.3.3/arcana/xnat/data/api.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/data/cs.py` & `arcana_xnat-0.3.3/arcana/xnat/data/cs.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/data/tests/test_store.py` & `arcana_xnat-0.3.3/arcana/xnat/data/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/deploy/command.py` & `arcana_xnat-0.3.3/arcana/xnat/deploy/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,26 +59,19 @@
         should be run
 
         Returns
         -------
         dict[str, *]
             the JSON-like dictionary to specify the command to the XNAT CS
         """
-        # Generate the complete configuration JSON
-        build_iteration_str = (
-            f" ({self.image.build_iteration})"
-            if self.image.build_iteration is None
-            else ""
-        )
 
         cmd_json = {
             "name": self.name,
             "description": (
-                f"{self.name} {self.image.version}{build_iteration_str}: "
-                f"{self.image.description}"
+                f"{self.name} {self.image.version}: {self.image.title}"
             ),
             "label": self.name,
             "schema-version": "1.0",
             "image": self.image.reference,
             "index": self.image.registry,
             "datatype": "docker",
             # "command-line": cmdline,
@@ -94,15 +87,15 @@
             ],
             "ports": {},
             "inputs": [],  # inputs_json,
             "outputs": [],  # outputs_json,
             "xnat": [
                 {
                     "name": self.name,
-                    "description": self.image.description,
+                    "description": self.image.title,
                     "contexts": [],  # context,
                     "external-inputs": [],  # external_inputs,
                     "derived-inputs": [],  # derived_inputs,
                     "output-handlers": [],  # output_handlers,
                 }
             ],
         }
@@ -124,18 +117,18 @@
             list of arguments to be appended to the command line
         """
         # Add task inputs to inputs JSON specification
         cmd_args = []
         for inpt in self.inputs:
             replacement_key = f"[{inpt.field.upper()}_INPUT]"
             if issubclass(inpt.datatype, FileSet):
-                desc = f"Match resource [SCAN_TYPE]: {inpt.help_string} "
+                desc = f"Match resource [SCAN_TYPE]: {inpt.help} "
                 input_type = "string"
             else:
-                desc = f"Match field ({inpt.datatype}) [FIELD_NAME]: {inpt.help_string} "
+                desc = f"Match field ({inpt.datatype}) [FIELD_NAME]: {inpt.help} "
                 input_type = self.COMMAND_INPUT_TYPES.get(inpt.datatype, "string")
             cmd_json["inputs"].append(
                 {
                     "name": self.path2xnatname(inpt.name),
                     "description": desc,
                     "type": input_type,
                     "default-value": inpt.config_dict.get("path", ""),
@@ -149,15 +142,15 @@
         return cmd_args
 
     def add_parameter_fields(self, cmd_json):
 
         # Add parameters as additional inputs to inputs JSON specification
         cmd_args = []
         for param in self.parameters:
-            desc = f"Parameter ({param.datatype}): " + param.help_string
+            desc = f"Parameter ({param.datatype}): " + param.help
 
             replacement_key = f"[{param.field.upper()}_PARAM]"
 
             cmd_json["inputs"].append(
                 {
                     "name": param.name,
                     "description": desc,
```

### Comparing `arcana_xnat-0.3.2/arcana/xnat/deploy/image.py` & `arcana_xnat-0.3.3/arcana/xnat/deploy/image.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/arcana/xnat/deploy/tests/test_app.py` & `arcana_xnat-0.3.3/arcana/xnat/deploy/tests/test_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,23 @@
     run_prefix,
 ):
     spec = {}
     if request.param == "func":
         spec["build"] = {
             "org": "arcana-tests",
             "name": "concatenate-xnat-cs",
-            "version": "1.0",
-            "description": "A pipeline to test Arcana's deployment tool",
+            "version": {
+                "package": "1.0",
+            },
+            "title": "A pipeline to test Arcana's deployment tool",
             "command": command_spec,
             "authors": [{"name": "Some One", "email": "some.one@an.email.org"}],
-            "info_url": "http://concatenate.readthefakedocs.io",
+            "docs": {
+                "info_url": "http://concatenate.readthefakedocs.io",
+            },
             "readme": "This is a test README",
             "registry": "a.docker.registry.io",
             "packages": {
                 "system": ["git", "vim"],
                 "pip": [
                     "arcana",
                     "arcana-xnat",
@@ -63,16 +67,18 @@
         )
         spec["params"] = {"duplicates": 2}
     elif request.param == "bids_app":
         bids_command_spec["configuration"]["executable"] = "/launch.sh"
         spec["build"] = {
             "org": "arcana-tests",
             "name": "bids-app-xnat-cs",
-            "version": "1.0",
-            "description": "A pipeline to test wrapping of BIDS apps",
+            "version": {
+                "package": "1.0",
+            },
+            "title": "A pipeline to test wrapping of BIDS apps",
             "base_image": {
                 "name": mock_bids_app_image,
                 "package_manager": "apt",
             },
             "packages": {
                 "system": ["git", "vim"],
                 "pip": [
@@ -85,15 +91,17 @@
                     "pydra",
                 ],
             },
             "command": bids_command_spec,
             "authors": [
                 {"name": "Some One Else", "email": "some.oneelse@an.email.org"}
             ],
-            "info_url": "http://a-bids-app.readthefakedocs.io",
+            "docs": {
+                "info_url": "http://a-bids-app.readthefakedocs.io",
+            },
             "readme": "This is another test README for BIDS app image",
             "registry": "another.docker.registry.io",
         }
         blueprint = TestXnatDatasetBlueprint(
             dim_lengths=[1, 1, 1],
             scans=[
                 ScanBP(
```

### Comparing `arcana_xnat-0.3.2/arcana/xnat/utils/testing.py` & `arcana_xnat-0.3.3/arcana/xnat/utils/testing.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/LICENSE` & `arcana_xnat-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/README.rst` & `arcana_xnat-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/pyproject.toml` & `arcana_xnat-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.2/PKG-INFO` & `arcana_xnat-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-xnat
-Version: 0.3.2
+Version: 0.3.3
 Summary: An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-xnat.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
```


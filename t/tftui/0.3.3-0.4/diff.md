# Comparing `tmp/tftui-0.3.3.tar.gz` & `tmp/tftui-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftui-0.3.3.tar", last modified: Sun Aug  6 07:20:19 2023, max compression
+gzip compressed data, was "tftui-0.4.tar", last modified: Tue Aug  8 15:19:13 2023, max compression
```

## Comparing `tftui-0.3.3.tar` & `tftui-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-06 07:20:09.000000 tftui-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-06 07:20:09.000000 tftui-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:20:19.936768 tftui-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-06 07:20:09.000000 tftui-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-06 07:20:10.000000 tftui-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 07:20:19.936768 tftui-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.932768 tftui-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/src/tftui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-06 07:20:09.000000 tftui-0.3.3/src/tftui/ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 07:20:19.936768 tftui-0.3.3/src/tftui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 07:20:19.000000 tftui-0.3.3/src/tftui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:19:13.654289 tftui-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 15:18:59.000000 tftui-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-08 15:18:59.000000 tftui-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-08-08 15:19:13.654289 tftui-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-08 15:18:59.000000 tftui-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-08 15:19:00.000000 tftui-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:19:13.654289 tftui-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:19:13.654289 tftui-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:19:13.654289 tftui-0.4/src/tftui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:18:59.000000 tftui-0.4/src/tftui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-08-08 15:18:59.000000 tftui-0.4/src/tftui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-08 15:18:59.000000 tftui-0.4/src/tftui/ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:19:13.654289 tftui-0.4/src/tftui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 15:19:13.000000 tftui-0.4/src/tftui.egg-info/top_level.txt
```

### Comparing `tftui-0.3.3/LICENSE` & `tftui-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tftui-0.3.3/PKG-INFO` & `tftui-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.3
+Version: 0.4
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,20 +212,28 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TFTUI - The Terraform textual UI
 
+[![PyPI version](https://badge.fury.io/py/tftui.svg)](https://badge.fury.io/py/tftui)
+![GitHub](https://img.shields.io/github/license/idoavrah/terraform-tui)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tftui)
+
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
-With its latest version [0.3.0](https://github.com/idoavrah/terraform-tui/releases/tag/v0.3.0) you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
+With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.4
+- [x] Fixed the erroneous flattening of submodules
+- [x] Added collapse levels for the state tree
+
 ### version 0.3
 - [x] Added loading screen and status bar
 - [x] Added selection of resources
 - [x] Added refresh state functionality
 - [x] Added taint/untaint functionality
 - [x] Refactoring
 
@@ -242,8 +250,7 @@
 | Tool            | Install             | Upgrade                       | Run                                      |
 |-----------------| ------------------- | ----------------------------- | ---------------------------------------- |
 | PIP             | `pip install tftui` | `pip install --upgrade tftui` | `cd /path/to/terraform/project && tftui` |
 | PIPX            | `pipx install tftui`| `pipx upgrade tftui`          | `cd /path/to/terraform/project && tftui` |
 
 ## Stargazers over time
 [![Stargazers over time](https://starchart.cc/idoavrah/terraform-tui.svg)](https://starchart.cc/idoavrah/terraform-tui)
-
```

### Comparing `tftui-0.3.3/README.md` & `tftui-0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # TFTUI - The Terraform textual UI
 
+[![PyPI version](https://badge.fury.io/py/tftui.svg)](https://badge.fury.io/py/tftui)
+![GitHub](https://img.shields.io/github/license/idoavrah/terraform-tui)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tftui)
+
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
-With its latest version [0.3.0](https://github.com/idoavrah/terraform-tui/releases/tag/v0.3.0) you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
+With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.4
+- [x] Fixed the erroneous flattening of submodules
+- [x] Added collapse levels for the state tree
+
 ### version 0.3
 - [x] Added loading screen and status bar
 - [x] Added selection of resources
 - [x] Added refresh state functionality
 - [x] Added taint/untaint functionality
 - [x] Refactoring
 
@@ -26,8 +34,7 @@
 | Tool            | Install             | Upgrade                       | Run                                      |
 |-----------------| ------------------- | ----------------------------- | ---------------------------------------- |
 | PIP             | `pip install tftui` | `pip install --upgrade tftui` | `cd /path/to/terraform/project && tftui` |
 | PIPX            | `pipx install tftui`| `pipx upgrade tftui`          | `cd /path/to/terraform/project && tftui` |
 
 ## Stargazers over time
 [![Stargazers over time](https://starchart.cc/idoavrah/terraform-tui.svg)](https://starchart.cc/idoavrah/terraform-tui)
-
```

### Comparing `tftui-0.3.3/pyproject.toml` & `tftui-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tftui"
-version = "0.3.3"
+version = "0.4"
 description = "Terraform Textual User Interface"
 readme = "README.md"
 authors = [{ name = "Ido Avraham" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `tftui-0.3.3/src/tftui/__main__.py` & `tftui-0.4/src/tftui/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,34 +86,41 @@
             parts = line[2:-1].split(".")
             i = 0
             module = ""
             while parts[i] == "module":
                 module += f"{parts[i]}.{parts[i+1]}."
                 modules.add(module[:-1])
                 i += 2
+
         for module_fullname in sorted(modules):
             parts = module_fullname.split(".")
-            qualifier = ""
+            sub_module = ""
             i = 0
             while i < len(parts):
-                qualifier = f"{parts[i]}.{parts[i+1]}."
-                if qualifier[:-1] not in module_nodes:
-                    node = self.root.add(qualifier[:-1], data=module_fullname)
-                    module_nodes[qualifier[:-1]] = node
+                parent = sub_module
+                short_name = f"{parts[i]}.{parts[i+1]}."
+                sub_module += short_name
+                if sub_module[:-1] not in module_nodes:
+                    if module_nodes.get(parent[:-1]) is None:
+                        parent_node = self.root
+                    else:
+                        parent_node = module_nodes[parent[:-1]]
+                    node = parent_node.add(short_name[:-1], data=sub_module[:-1])
+                    module_nodes[sub_module[:-1]] = node
                 i += 2
 
         # parse objects
         name = ""
         for line in lines:
             if line.startswith("#"):
                 parts = line[2:].split(".")
                 i = 0
                 qualifier = ""
                 while parts[i] == "module":
-                    qualifier = f"{parts[i]}.{parts[i+1]}."
+                    qualifier += f"{parts[i]}.{parts[i+1]}."
                     i += 2
                 name = ".".join(parts[i:]).replace(":", "")
                 data = ""
                 if qualifier[:-1] in module_nodes:
                     module_node = module_nodes[qualifier[:-1]]
                 else:
                     module_node = self.root
@@ -148,19 +155,20 @@
     BINDINGS = [
         ("Enter", "", "View state"),
         Binding("escape", "back", "Back"),
         ("s", "select", "Select"),
         ("t", "taint", "Taint"),
         ("u", "untaint", "Untaint"),
         ("r", "refresh", "Refresh state"),
+        ("1-9", "collapse", "Collapse level"),
         ("m", "toggle_dark", "Toggle dark mode"),
         Binding("y", "yes", "Yes", show=False),
         Binding("n", "no", "No", show=False),
         ("q", "quit", "Quit"),
-    ]
+    ] + [Binding(f"{i}", f"collapse({i})", show=False) for i in range(10)]
 
     def compose(self) -> ComposeResult:
         yield Header(classes="header")
         with ContentSwitcher(id="switcher", initial="loading"):
             yield LoadingIndicator(id="loading")
             yield StateTree("State", id="tree")
             yield TextLog(
@@ -266,14 +274,35 @@
         if not self.switcher.current == "tree":
             return
         self.tree.refresh_state()
 
     def action_toggle_dark(self) -> None:
         self.dark = not self.dark
 
+    def expand_node(self, level, node) -> None:
+        if not node.allow_expand:
+            return
+        cnt = node.data.count(".module.") + 1
+        if level <= cnt:
+            return
+        for child in node.children:
+            self.expand_node(level, child)
+        node.expand()
+
+    def action_collapse(self, level=0) -> None:
+        if not self.switcher.current == "tree":
+            return
+        if level == 0:
+            self.tree.root.expand_all()
+            return
+        self.tree.root.collapse_all()
+        for node in self.tree.root.children:
+            self.expand_node(level, node)
+        self.tree.root.expand()
+
 
 async def execute_async(*command: str) -> tuple[str, str]:
     proc = await asyncio.create_subprocess_exec(
         *command, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
     )
 
     stdout, strerr = await proc.communicate()
```

### Comparing `tftui-0.3.3/src/tftui/ui.css` & `tftui-0.4/src/tftui/ui.css`

 * *Files identical despite different names*

### Comparing `tftui-0.3.3/src/tftui.egg-info/PKG-INFO` & `tftui-0.4/src/tftui.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftui
-Version: 0.3.3
+Version: 0.4
 Summary: Terraform Textual User Interface
 Author: Ido Avraham
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,20 +212,28 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TFTUI - The Terraform textual UI
 
+[![PyPI version](https://badge.fury.io/py/tftui.svg)](https://badge.fury.io/py/tftui)
+![GitHub](https://img.shields.io/github/license/idoavrah/terraform-tui)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tftui)
+
 `TFTUI` is a powerful textual GUI that empowers users to effortlessly view and interact with their Terraform state.
 
-With its latest version [0.3.0](https://github.com/idoavrah/terraform-tui/releases/tag/v0.3.0) you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
+With its latest version you can easily visualize the complete state tree, gaining deeper insights into your infrastructure's current configuration. Additionally, the ability to inspect individual resource states allows you to focus on specific details for better analysis and management. Lastly, it's now possible to select resources and perform actions such as tainting and untainting.
 
 ## Key Features
 
+### version 0.4
+- [x] Fixed the erroneous flattening of submodules
+- [x] Added collapse levels for the state tree
+
 ### version 0.3
 - [x] Added loading screen and status bar
 - [x] Added selection of resources
 - [x] Added refresh state functionality
 - [x] Added taint/untaint functionality
 - [x] Refactoring
 
@@ -242,8 +250,7 @@
 | Tool            | Install             | Upgrade                       | Run                                      |
 |-----------------| ------------------- | ----------------------------- | ---------------------------------------- |
 | PIP             | `pip install tftui` | `pip install --upgrade tftui` | `cd /path/to/terraform/project && tftui` |
 | PIPX            | `pipx install tftui`| `pipx upgrade tftui`          | `cd /path/to/terraform/project && tftui` |
 
 ## Stargazers over time
 [![Stargazers over time](https://starchart.cc/idoavrah/terraform-tui.svg)](https://starchart.cc/idoavrah/terraform-tui)
-
```


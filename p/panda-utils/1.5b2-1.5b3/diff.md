# Comparing `tmp/panda_utils-1.5b2.tar.gz` & `tmp/panda_utils-1.5b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.5b2.tar", last modified: Wed Aug  2 22:44:18 2023, max compression
+gzip compressed data, was "panda_utils-1.5b3.tar", last modified: Tue Aug  8 16:21:30 2023, max compression
```

## Comparing `panda_utils-1.5b2.tar` & `panda_utils-1.5b3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.822243 panda_utils-1.5b2/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.5b2/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-02 22:44:18.822243 panda_utils-1.5b2/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.5b2/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.5b2/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.815577 panda_utils-1.5b2/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b2/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.5b2/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.5b2/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.5b2/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.5b2/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15739 2023-08-02 21:27:11.000000 panda_utils-1.5b2/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.5b2/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.5b2/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2025 2023-08-01 22:08:01.000000 panda_utils-1.5b2/panda_utils/blender/export_with_yabee.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.5b2/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.5b2/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.5b2/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     6010 2023-08-02 21:34:30.000000 panda_utils-1.5b2/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.5b2/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.822243 panda_utils-1.5b2/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b2/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.5b2/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.5b2/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.5b2/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.5b2/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.5b2/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.5b2/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-02 22:44:18.818910 panda_utils-1.5b2/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-08-02 22:44:18.000000 panda_utils-1.5b2/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-08-02 22:44:08.000000 panda_utils-1.5b2/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.5b2/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-08-02 22:44:18.822243 panda_utils-1.5b2/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.284520 panda_utils-1.5b3/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.5b3/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-08 16:21:30.284520 panda_utils-1.5b3/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.5b3/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.5b3/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.277853 panda_utils-1.5b3/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b3/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.5b3/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.281187 panda_utils-1.5b3/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.5b3/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.5b3/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.5b3/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.5b3/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    16295 2023-08-08 15:23:02.000000 panda_utils-1.5b3/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.5b3/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.281187 panda_utils-1.5b3/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.5b3/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.5b3/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2025 2023-08-01 22:08:01.000000 panda_utils-1.5b3/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.5b3/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.5b3/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.281187 panda_utils-1.5b3/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.5b3/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5559 2023-08-08 15:23:12.000000 panda_utils-1.5b3/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.5b3/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.284520 panda_utils-1.5b3/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.5b3/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.5b3/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.5b3/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.5b3/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.5b3/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.5b3/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.5b3/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-08-08 16:21:30.281187 panda_utils-1.5b3/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-08-08 16:21:30.000000 panda_utils-1.5b3/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-08-08 16:21:30.000000 panda_utils-1.5b3/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-08-08 16:21:30.000000 panda_utils-1.5b3/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-08-08 16:21:30.000000 panda_utils-1.5b3/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-08-08 16:21:30.000000 panda_utils-1.5b3/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-08-08 16:05:43.000000 panda_utils-1.5b3/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.5b3/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-08-08 16:21:30.284520 panda_utils-1.5b3/setup.cfg
```

### Comparing `panda_utils-1.5b2/LICENSE` & `panda_utils-1.5b3/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/PKG-INFO` & `panda_utils-1.5b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.5b2
+Version: 1.5b3
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.5b2/README.md` & `panda_utils-1.5b3/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/__main__.py` & `panda_utils-1.5b3/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.5b3/panda_utils/assetpipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/assetpipeline/misc.py` & `panda_utils-1.5b3/panda_utils/assetpipeline/misc.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/assetpipeline/models.py` & `panda_utils-1.5b3/panda_utils/assetpipeline/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 def action_transparent(ctx):
     ctx.cache_eggs()
     for file, tree in ctx.eggs.items():
         logger.info("%s: Adding transparency to: %s", ctx.name, file)
         new_node = eggparse.EggLeaf("Scalar", "alpha", "dual")
         for tex in tree.findall("Texture"):
             for child in tex.children:
-                if child.equals(new_node):
+                if repr(child) == repr(new_node):
                     break
             else:
                 tex.add_child(new_node)
 
 
 def action_model_parent(ctx):
     ctx.cache_eggs()
@@ -316,24 +316,37 @@
         ctx.putil_ctx,
         "egg-palettize",
         "-opt",
         "-redo",
         "-nodb",
         "-inplace",
         *all_eggs,
-        "-inplace",
+        "-dm",
+        "palette-temp",
         "-tn",
         f"{ctx.model_name}_palette_%p_%i",
         timeout=60,
     )
 
     if "ordered" in flag_list:
         for file in all_eggs:
             remove_palette_indices(file)
 
+    logger.info("%s: Patching textures after palettization...", ctx.name)
+    ctx.cache_eggs()
+    for eggtree in ctx.eggs.values():
+        for texture in eggtree.findall("Texture"):
+            texture_name = texture.get_child(0)
+            texture_name.value = texture_name.value.replace("palette-temp/", "", 1)
+    palette_folder = pathlib.Path("palette-temp")
+    for file in os.listdir(palette_folder):
+        if "_palette_" in file:
+            shutil.move(palette_folder / file, file)
+    shutil.rmtree(palette_folder)
+
 
 def action_optchar(ctx, flags, expose):
     ctx.uncache_eggs()
     if isinstance(flags, str):
         flags = flags.split(",")
     if isinstance(expose, str):
         expose = expose.split(",")
```

### Comparing `panda_utils-1.5b2/panda_utils/assetpipeline/textures.py` & `panda_utils-1.5b3/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/blender/export_glb.py` & `panda_utils-1.5b3/panda_utils/blender/export_glb.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/blender/export_with_yabee.py` & `panda_utils-1.5b3/panda_utils/blender/export_with_yabee.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/blender/import_model.py` & `panda_utils-1.5b3/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/eggtree/eggparse.py` & `panda_utils-1.5b3/panda_utils/eggtree/eggparse.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,14 @@
     def remove_nodes(self, nodeset):
         pass
 
     @abc.abstractmethod
     def get_child(self, index):
         pass
 
-    # We can't use __eq__ because it breaks set()
-    def equals(self, other):
-        return False
-
 
 class EggString(EggNode):
     def __init__(self, value):
         self.value = value
 
     def __repr__(self):
         return self.value
@@ -67,32 +63,21 @@
 
     def remove_nodes(self, nodeset):
         pass
 
     def get_child(self, index):
         return None
 
-    def equals(self, other):
-        return isinstance(other, EggString) and other.value == self.value
-
 
 class EggLeaf(EggNode):
     def __init__(self, node_type, node_name, node_value):
         self.node_type = node_type
         self.node_name = (node_name or "").strip()
         self.node_value = node_value
 
-    def equals(self, other):
-        return (
-            isinstance(other, EggLeaf)
-            and other.node_name == self.node_name
-            and other.node_value == self.node_value
-            and other.node_type == self.node_type
-        )
-
     def __repr__(self):
         if self.node_name:
             return f"<{self.node_type}> {self.node_name.strip()} {{ {self.node_value.strip()} }}"
         return f"<{self.node_type}> {{ {self.node_value.strip()} }}"
 
     def findall(self, node_type):
         if self.node_type == node_type:
@@ -144,16 +129,16 @@
 
 def sanitize_string(val):
     if val and val[0] in "\"'":
         return val[1:-1]
     return val
 
 
-single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$*]+)> ([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
-preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> ([-a-z0-9A-Z_.<>\" ]+ )?\{([^\n]*)")
+single_line_leaf_regex = re.compile(r"<([A-Za-z0-9_$*]+)> +([-a-z0-9A-Z_.]+ )?\{ ?(.+) ?}")
+preline_regex = re.compile(r"<([A-Za-z0-9_$]+)> +([-a-z0-9A-Z_.<>\" ]+ )?\{([^\n]*)")
 
 
 def subtree_tokenize(lines: List[str]):
     last_line = lines[-1].strip()
     if len(lines) == 1:
         if last_line.count("}") > 1 and not last_line.startswith("<VertexRef>"):
             parts = [x + "}" for x in last_line.split("}")[:-1]]
```

### Comparing `panda_utils-1.5b2/panda_utils/eggtree/operations.py` & `panda_utils-1.5b3/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/tools/animconvert.py` & `panda_utils-1.5b3/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/tools/convert.py` & `panda_utils-1.5b3/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/tools/downscale.py` & `panda_utils-1.5b3/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/tools/palettize.py` & `panda_utils-1.5b3/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/tools/toontown.py` & `panda_utils-1.5b3/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils/util.py` & `panda_utils-1.5b3/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.5b3/panda_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.5b2
+Version: 1.5b3
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.5b2/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.5b3/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.5b2/pyproject.toml` & `panda_utils-1.5b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.5b2"
+version = "1.5b3"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```


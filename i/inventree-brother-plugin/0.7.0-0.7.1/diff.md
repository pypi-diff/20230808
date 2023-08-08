# Comparing `tmp/inventree-brother-plugin-0.7.0.tar.gz` & `tmp/inventree-brother-plugin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-brother-plugin-0.7.0.tar", last modified: Sat Jul 15 09:17:08 2023, max compression
+gzip compressed data, was "dist/inventree-brother-plugin-0.7.1.tar", last modified: Tue Aug  8 11:42:28 2023, max compression
```

## Comparing `inventree-brother-plugin-0.7.0.tar` & `inventree-brother-plugin-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/brother_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/inventree_brother/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 09:17:08.000000 inventree-brother-plugin-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-15 09:16:58.000000 inventree-brother-plugin-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/inventree_brother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/inventree_brother/brother_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/inventree_brother/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-08 11:42:28.000000 inventree-brother-plugin-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-08 11:42:16.000000 inventree-brother-plugin-0.7.1/setup.py
```

### Comparing `inventree-brother-plugin-0.7.0/LICENSE` & `inventree-brother-plugin-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-brother-plugin-0.7.0/PKG-INFO` & `inventree-brother-plugin-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-brother-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: Brother label printer plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-brother-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree label printer printing inventory
 Requires-Python: >=3.9
```

### Comparing `inventree-brother-plugin-0.7.0/README.md` & `inventree-brother-plugin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `inventree-brother-plugin-0.7.0/inventree_brother/brother_plugin.py` & `inventree-brother-plugin-0.7.1/inventree_brother/brother_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -135,22 +135,35 @@
 
         # Get specifications of media type
         media_specs = None
         for label_specs in ALL_LABELS:
             if label_specs.identifier == media_type:
                 media_specs = label_specs
 
+        rotation = int(self.get_setting('ROTATION'))
+
         try:
             # Resize image if media type is a die cut label (the brother_ql library only accepts images
             # with a specific size in that case)
             # TODO: Make it generic for all media types
             # TODO: Add GUI settings to configure scaling and margins
             if media_specs.form_factor in [FormFactor.DIE_CUT, FormFactor.ROUND_DIE_CUT]:
                 # Scale image to fit the entire printable area and pad with whitespace (while preserving aspect ratio)
                 printable_image = ImageOps.pad(label_image, media_specs.dots_printable, color="white")
+
+                if rotation == 90:
+                    # Rotate image 90 degrees
+                    printable_image = printable_image.rotate(90, expand=True)
+                elif rotation == 180:
+                    # Rotate image 180 degrees
+                    printable_image = printable_image.rotate(180, expand=True)
+                elif rotation == 270:
+                    # Rotate image 270 degrees
+                    printable_image = printable_image.rotate(270, expand=True)
+
             else:
                 # Just leave image as-is
                 printable_image = label_image
         except AttributeError as e:
             raise AttributeError("Could not find specifications of label media type '%s'" % media_type) from e
         except Exception as e:
             raise e
@@ -165,15 +178,15 @@
 
         # Generate instructions for printing
         params = {
             'qlr': printer,
             'images': [printable_image],
             'label': media_type,
             'cut': self.get_setting('AUTO_CUT'),
-            'rotate': self.get_setting('ROTATION'),
+            'rotate': rotation,
             'compress': self.get_setting('COMPRESSION'),
             'hq': self.get_setting('HQ'),
             'red': red,
         }
 
         instructions = convert(**params)
```

### Comparing `inventree-brother-plugin-0.7.0/inventree_brother_plugin.egg-info/PKG-INFO` & `inventree-brother-plugin-0.7.1/inventree_brother_plugin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-brother-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: Brother label printer plugin for InvenTree
 Home-page: https://github.com/inventree/inventree-brother-plugin
 Author: Oliver Walters
 Author-email: oliver.henry.walters@gmail.com
 License: MIT
 Keywords: inventree label printer printing inventory
 Requires-Python: >=3.9
```

### Comparing `inventree-brother-plugin-0.7.0/setup.py` & `inventree-brother-plugin-0.7.1/setup.py`

 * *Files identical despite different names*


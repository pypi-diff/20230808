# Comparing `tmp/kiauto-2.2.6.tar.gz` & `tmp/kiauto-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiauto-2.2.6.tar", last modified: Mon Jun 12 11:51:05 2023, max compression
+gzip compressed data, was "kiauto-2.2.7.tar", last modified: Tue Aug  8 13:01:18 2023, max compression
```

## Comparing `kiauto-2.2.6.tar` & `kiauto-2.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-06-12 11:48:32.000000 kiauto-2.2.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       67 2023-06-12 11:48:32.000000 kiauto-2.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17079 2023-06-12 11:51:05.902936 kiauto-2.2.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13874 2023-06-12 11:48:32.000000 kiauto-2.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14967 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto/interposer/
--rwxrwxr-x   0 root         (0) root         (0)    27344 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/interposer/libinterposer.so
--rw-rw-r--   0 root         (0) root         (0)    28139 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/interposer.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/log.py
--rw-rw-r--   0 root         (0) root         (0)    14389 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/misc.py
--rw-rw-r--   0 root         (0) root         (0)    19007 2023-06-12 11:48:32.000000 kiauto-2.2.6/kiauto/ui_automation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/kiauto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17079 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 11:51:05.000000 kiauto-2.2.6/kiauto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 11:51:05.902936 kiauto-2.2.6/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1410 2023-06-12 11:48:32.000000 kiauto-2.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:05.902936 kiauto-2.2.6/src/
--rwxrwxr-x   0 root         (0) root         (0)    43858 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/eeschema_do
--rwxrwxr-x   0 root         (0) root         (0)     7104 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/kicad2step_do
--rwxrwxr-x   0 root         (0) root         (0)    76566 2023-06-12 11:48:32.000000 kiauto-2.2.6/src/pcbnew_do
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:01:18.455676 kiauto-2.2.7/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-08-08 12:59:21.000000 kiauto-2.2.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-08-08 12:59:21.000000 kiauto-2.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-08-08 13:01:18.455676 kiauto-2.2.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    13874 2023-08-08 12:59:21.000000 kiauto-2.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:01:18.451676 kiauto-2.2.7/kiauto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14967 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:01:18.455676 kiauto-2.2.7/kiauto/interposer/
+-rwxrwxr-x   0 root         (0) root         (0)    27344 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/interposer/libinterposer.so
+-rw-rw-r--   0 root         (0) root         (0)    28456 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/interposer.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/log.py
+-rw-rw-r--   0 root         (0) root         (0)    14389 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    19007 2023-08-08 12:59:21.000000 kiauto-2.2.7/kiauto/ui_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:01:18.455676 kiauto-2.2.7/kiauto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-08-08 13:01:18.000000 kiauto-2.2.7/kiauto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-08-08 13:01:18.000000 kiauto-2.2.7/kiauto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 13:01:18.000000 kiauto-2.2.7/kiauto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-08 13:01:18.000000 kiauto-2.2.7/kiauto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-08 13:01:18.000000 kiauto-2.2.7/kiauto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 13:01:18.455676 kiauto-2.2.7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1410 2023-08-08 12:59:21.000000 kiauto-2.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 13:01:18.455676 kiauto-2.2.7/src/
+-rwxrwxr-x   0 root         (0) root         (0)    44086 2023-08-08 12:59:21.000000 kiauto-2.2.7/src/eeschema_do
+-rwxrwxr-x   0 root         (0) root         (0)     7104 2023-08-08 12:59:21.000000 kiauto-2.2.7/src/kicad2step_do
+-rwxrwxr-x   0 root         (0) root         (0)    76655 2023-08-08 12:59:21.000000 kiauto-2.2.7/src/pcbnew_do
```

### Comparing `kiauto-2.2.6/LICENSE` & `kiauto-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/PKG-INFO` & `kiauto-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.6
+Version: 2.2.7
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.6/README.md` & `kiauto-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/kiauto/file_util.py` & `kiauto-2.2.7/kiauto/file_util.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/kiauto/interposer/libinterposer.so` & `kiauto-2.2.7/kiauto/interposer/libinterposer.so`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/kiauto/interposer.py` & `kiauto-2.2.7/kiauto/interposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
     """ Wait until we get the file name """
     wait_queue(cfg, 'PANGO:'+name, dialog_interrupts=True)
 
 
 def paste_text_i(cfg, msg, text):
     """ Paste some text and check the echo from KiCad, then wait for sleep """
     # Paste the name
-    cfg.logger.info(msg)
+    cfg.logger.info('{} ({})'.format(msg, text))
     wait_point(cfg)
     retry = True
     while retry:
         retry = False
         text_replace(text)
         try:
             # Look for the echo
@@ -480,15 +480,24 @@
 
 
 def dismiss_file_open_error(cfg, title):
     """ KiCad 6: File is already opened """
     msgs = collect_dialog_messages(cfg, title)
     kind = 'PCB' if cfg.is_pcbnew else 'Schematic'
     fname = os.path.basename(cfg.input_file)
-    if 'Open Anyway' in msgs and kind+" '"+fname+"' is already open." in msgs:
+    # KiCad 6.x and <7.0.7: PCB 'xxxx' is already open.
+    # KiCad 7.0.7: PCB 'xxxx' is already open by 'user' at 'host'
+    start = kind+" '"+fname+"' is already open"
+    found = False
+    for msg in msgs:
+        if msg.startswith(start) and msg.endswith("."):
+            found = True
+            fname = msg
+            break
+    if 'Open Anyway' in msgs and found:
         cfg.logger.warning('This file is already opened ({})'.format(fname))
         dismiss_dialog(cfg, title, ['Left', 'Return'])
         return
     unknown_dialog(cfg, title, msgs)
 
 
 def dismiss_already_running(cfg, title):
```

### Comparing `kiauto-2.2.6/kiauto/log.py` & `kiauto-2.2.7/kiauto/log.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/kiauto/misc.py` & `kiauto-2.2.7/kiauto/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,8 +342,8 @@
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2018-2023, INTI/Productize SPRL'
 __credits__ = ['Salvador E. Tropea', 'Seppe Stas', 'Jesse Vincent', 'Scott Bezek']
 __license__ = 'Apache 2.0'
 __email__ = 'stropea@inti.gob.ar'
 __status__ = 'stable'
 __url__ = 'https://github.com/INTI-CMNB/KiAuto/'
-__version__ = '2.2.6'
+__version__ = '2.2.7'
```

### Comparing `kiauto-2.2.6/kiauto/ui_automation.py` & `kiauto-2.2.7/kiauto/ui_automation.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/kiauto.egg-info/PKG-INFO` & `kiauto-2.2.7/kiauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.6
+Version: 2.2.7
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.6/setup.py` & `kiauto-2.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/src/eeschema_do` & `kiauto-2.2.7/src/eeschema_do`

 * *Files 1% similar despite different names*

```diff
@@ -481,14 +481,16 @@
     wait_point(cfg)
     xdotool(['key', 'Return'])
     wait_for_file_created_by_process(cfg.eeschema_pid, cfg.output_file)
     # Close the ERC dialog
     logger.info('Exit ERC')
     wait_point(cfg)
     xdotool(['key', 'Escape'])
+    # KiCad 7.0.7 lack of ESC support
+    xdotool(['key', 'shift+Tab', 'shift+Tab', 'Return'])
 
 
 def eeschema_run_erc_schematic_6_0_i(cfg):
     # KiCad 7.99 particularities:
     # 1. Forces ".rpt" in the name, no matter what name was selected in the dialog and no matter if it already has an extension
     # 2. The ERC dialog isn't destroyed, most probably hidden
     # Open the ERC dialog
@@ -520,15 +522,17 @@
         file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s')
     # Paste the output file
     paste_bogus_filename(cfg)
     send_keys(cfg, 'Create the report', 'Return', closes=file_dlg, delay_io=True)
     # Wait until created
     wait_create_i(cfg, 'ERC', forced_ext='rpt')
     # Close the ERC dialog
-    send_keys(cfg, 'Exit ERC', 'Escape', closes=dialog, no_destroy=cfg.ki8)
+    # KiCad 7.0.7 no longer closes this dialog with ESC
+    # send_keys(cfg, 'Exit ERC', 'Escape', closes=dialog, no_destroy=cfg.ki8)
+    send_keys(cfg, 'Exit ERC', 'alt+l', closes=dialog, no_destroy=cfg.ki8)
 
 
 def eeschema_run_erc_schematic(cfg):
     if cfg.ki5:
         if cfg.use_interposer:
             eeschema_run_erc_schematic_5_1_i(cfg)
         else:
```

### Comparing `kiauto-2.2.6/src/kicad2step_do` & `kiauto-2.2.7/src/kicad2step_do`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.6/src/pcbnew_do` & `kiauto-2.2.7/src/pcbnew_do`

 * *Files 0% similar despite different names*

```diff
@@ -671,16 +671,17 @@
 
 
 def export_gencad_i(cfg, keys):
     # Open the "Export to GenCAD settings"
     dialog, _ = open_dialog_i(cfg, 'Export to GenCAD settings', keys)
     # KiCad dialogs are unreliable, you never know which widget is selected
     # This goes to the top left corner of the dialog
-    # Note: lamentably this widget doesn't have a label
-    xdotool(['key', 'alt+f', 'Up'])
+    # Note 1: lamentably this widget doesn't have a label
+    # Note 2: KiCad 7.0.7 behavior changed, up goes to the button (when no WM)
+    xdotool(['key', 'alt+f', 'Up', 'Left'])
     # Paste the name
     paste_output_file_i(cfg)
     # Change the settings to what the user wants
     # To make it easier we add accelerators
     keys = ['key']
     if not cfg.flip_bottom_padstacks:
         # We used Alt+F to go to the file name, so here the logic is inverted
```


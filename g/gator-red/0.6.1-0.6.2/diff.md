# Comparing `tmp/gator-red-0.6.1.tar.gz` & `tmp/gator-red-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gator-red-0.6.1.tar", last modified: Tue Aug  8 19:38:44 2023, max compression
+gzip compressed data, was "gator-red-0.6.2.tar", last modified: Tue Aug  8 20:20:49 2023, max compression
```

## Comparing `gator-red-0.6.1.tar` & `gator-red-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.072758 gator-red-0.6.1/
--rw-rw-rw-   0        0        0        0 2023-08-07 13:03:31.000000 gator-red-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       79 2023-08-08 19:38:44.072758 gator-red-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-08-07 13:03:31.000000 gator-red-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.029816 gator-red-0.6.1/gator/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.1/gator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.033814 gator-red-0.6.1/gator/auth/
--rw-rw-rw-   0        0        0        0 2023-08-06 05:55:43.000000 gator-red-0.6.1/gator/auth/__init__.py
--rw-rw-rw-   0        0        0     7136 2023-08-08 17:54:40.000000 gator-red-0.6.1/gator/auth/auth_commands.py
--rw-rw-rw-   0        0        0     1493 2023-08-08 17:37:12.000000 gator-red-0.6.1/gator/auth/credentials.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.036814 gator-red-0.6.1/gator/cli/
--rw-rw-rw-   0        0        0       88 2023-08-08 03:28:10.000000 gator-red-0.6.1/gator/cli/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-08-08 17:24:03.000000 gator-red-0.6.1/gator/cli/functions_cli.py
--rw-rw-rw-   0        0        0     2313 2023-08-08 17:23:27.000000 gator-red-0.6.1/gator/cli/storage_cli.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.038833 gator-red-0.6.1/gator/custom/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.1/gator/custom/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-08-08 02:28:09.000000 gator-red-0.6.1/gator/custom/custom_cli.py
--rw-rw-rw-   0        0        0      702 2023-08-08 17:23:06.000000 gator-red-0.6.1/gator/main.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.039814 gator-red-0.6.1/gator/modules/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.1/gator/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.043815 gator-red-0.6.1/gator/modules/functions/
--rw-rw-rw-   0        0        0      236 2023-08-08 04:42:36.000000 gator-red-0.6.1/gator/modules/functions/__init__.py
--rw-rw-rw-   0        0        0     7225 2023-08-08 17:24:28.000000 gator-red-0.6.1/gator/modules/functions/functions.py
--rw-rw-rw-   0        0        0     3626 2023-08-08 17:24:42.000000 gator-red-0.6.1/gator/modules/functions/permissions.py
--rw-rw-rw-   0        0        0     2717 2023-08-08 17:24:52.000000 gator-red-0.6.1/gator/modules/functions/triggers.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.046813 gator-red-0.6.1/gator/modules/storage/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.1/gator/modules/storage/__init__.py
--rw-rw-rw-   0        0        0     4840 2023-08-08 17:25:06.000000 gator-red-0.6.1/gator/modules/storage/buckets.py
--rw-rw-rw-   0        0        0     2005 2023-08-08 17:25:14.000000 gator-red-0.6.1/gator/modules/storage/permissions.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.048815 gator-red-0.6.1/gator/utils/
--rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.1/gator/utils/__init__.py
--rw-rw-rw-   0        0        0      872 2023-08-08 17:25:18.000000 gator-red-0.6.1/gator/utils/print_helpers.py
-drwxrwxrwx   0        0        0        0 2023-08-08 19:38:44.070788 gator-red-0.6.1/gator_red.egg-info/
--rw-rw-rw-   0        0        0       79 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      418 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-08 19:38:43.000000 gator-red-0.6.1/gator_red.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-08 19:38:44.073746 gator-red-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      380 2023-08-08 19:38:22.000000 gator-red-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.941558 gator-red-0.6.2/
+-rw-rw-rw-   0        0        0        0 2023-08-07 13:03:31.000000 gator-red-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     7638 2023-08-08 20:20:49.940557 gator-red-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7516 2023-08-08 20:12:25.000000 gator-red-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.912557 gator-red-0.6.2/gator/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.2/gator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.915557 gator-red-0.6.2/gator/auth/
+-rw-rw-rw-   0        0        0        0 2023-08-06 05:55:43.000000 gator-red-0.6.2/gator/auth/__init__.py
+-rw-rw-rw-   0        0        0     7136 2023-08-08 17:54:40.000000 gator-red-0.6.2/gator/auth/auth_commands.py
+-rw-rw-rw-   0        0        0     1493 2023-08-08 17:37:12.000000 gator-red-0.6.2/gator/auth/credentials.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.918558 gator-red-0.6.2/gator/cli/
+-rw-rw-rw-   0        0        0       88 2023-08-08 03:28:10.000000 gator-red-0.6.2/gator/cli/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-08-08 17:24:03.000000 gator-red-0.6.2/gator/cli/functions_cli.py
+-rw-rw-rw-   0        0        0     2313 2023-08-08 17:23:27.000000 gator-red-0.6.2/gator/cli/storage_cli.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.919557 gator-red-0.6.2/gator/custom/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.2/gator/custom/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-08-08 02:28:09.000000 gator-red-0.6.2/gator/custom/custom_cli.py
+-rw-rw-rw-   0        0        0      716 2023-08-08 20:16:09.000000 gator-red-0.6.2/gator/main.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.920557 gator-red-0.6.2/gator/modules/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.2/gator/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.925558 gator-red-0.6.2/gator/modules/functions/
+-rw-rw-rw-   0        0        0      236 2023-08-08 04:42:36.000000 gator-red-0.6.2/gator/modules/functions/__init__.py
+-rw-rw-rw-   0        0        0     7225 2023-08-08 17:24:28.000000 gator-red-0.6.2/gator/modules/functions/functions.py
+-rw-rw-rw-   0        0        0     3626 2023-08-08 17:24:42.000000 gator-red-0.6.2/gator/modules/functions/permissions.py
+-rw-rw-rw-   0        0        0     2717 2023-08-08 17:24:52.000000 gator-red-0.6.2/gator/modules/functions/triggers.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.928557 gator-red-0.6.2/gator/modules/storage/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.2/gator/modules/storage/__init__.py
+-rw-rw-rw-   0        0        0     4840 2023-08-08 17:25:06.000000 gator-red-0.6.2/gator/modules/storage/buckets.py
+-rw-rw-rw-   0        0        0     2005 2023-08-08 17:25:14.000000 gator-red-0.6.2/gator/modules/storage/permissions.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.930557 gator-red-0.6.2/gator/utils/
+-rw-rw-rw-   0        0        0        0 2023-08-05 18:37:15.000000 gator-red-0.6.2/gator/utils/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-08-08 17:25:18.000000 gator-red-0.6.2/gator/utils/print_helpers.py
+drwxrwxrwx   0        0        0        0 2023-08-08 20:20:49.939558 gator-red-0.6.2/gator_red.egg-info/
+-rw-rw-rw-   0        0        0     7638 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      418 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-08 20:20:49.000000 gator-red-0.6.2/gator_red.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 20:20:49.941558 gator-red-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      652 2023-08-08 20:14:03.000000 gator-red-0.6.2/setup.py
```

### Comparing `gator-red-0.6.1/gator/auth/auth_commands.py` & `gator-red-0.6.2/gator/auth/auth_commands.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/auth/credentials.py` & `gator-red-0.6.2/gator/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/cli/functions_cli.py` & `gator-red-0.6.2/gator/cli/functions_cli.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/cli/storage_cli.py` & `gator-red-0.6.2/gator/cli/storage_cli.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/custom/custom_cli.py` & `gator-red-0.6.2/gator/custom/custom_cli.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/main.py` & `gator-red-0.6.2/gator/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from gator.auth import auth_commands
 from gator.cli.storage_cli import storage
 from gator.cli.functions_cli import functions
 
 @click.group(cls=CustomGroup)
 def main():
     """GATOR - GCP Attack Toolkit for Offensive Research, a tool designed to aid in 
-    research and exploiting Google Cloud Environments. It offers a comprehensive 
+    research and exploiting Google Cloud and Workspace Environments. It offers a comprehensive 
     range of modules tailored to support users in various attack stages, spanning 
     from Reconnaissance to Impact."""
     pass
 
 main.add_command(auth_commands.auth)
 main.add_command(storage)
 main.add_command(functions)
```

### Comparing `gator-red-0.6.1/gator/modules/functions/functions.py` & `gator-red-0.6.2/gator/modules/functions/functions.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/modules/functions/permissions.py` & `gator-red-0.6.2/gator/modules/functions/permissions.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/modules/functions/triggers.py` & `gator-red-0.6.2/gator/modules/functions/triggers.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/modules/storage/buckets.py` & `gator-red-0.6.2/gator/modules/storage/buckets.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/modules/storage/permissions.py` & `gator-red-0.6.2/gator/modules/storage/permissions.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator/utils/print_helpers.py` & `gator-red-0.6.2/gator/utils/print_helpers.py`

 * *Files identical despite different names*

### Comparing `gator-red-0.6.1/gator_red.egg-info/SOURCES.txt` & `gator-red-0.6.2/gator_red.egg-info/SOURCES.txt`

 * *Files identical despite different names*


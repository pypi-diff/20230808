# Comparing `tmp/pulumi_cloudinit-1.4.0a1691127304.tar.gz` & `tmp/pulumi_cloudinit-1.4.0a1691508515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.4.0a1691127304.tar", last modified: Fri Aug  4 05:38:36 2023, max compression
+gzip compressed data, was "pulumi_cloudinit-1.4.0a1691508515.tar", last modified: Tue Aug  8 15:33:20 2023, max compression
```

## Comparing `pulumi_cloudinit-1.4.0a1691127304.tar` & `pulumi_cloudinit-1.4.0a1691508515.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:38:36.973554 pulumi_cloudinit-1.4.0a1691127304/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-04 05:38:36.973554 pulumi_cloudinit-1.4.0a1691127304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:38:36.969554 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:38:36.973554 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 05:38:36.973554 pulumi_cloudinit-1.4.0a1691127304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-04 05:38:36.000000 pulumi_cloudinit-1.4.0a1691127304/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:33:20.207852 pulumi_cloudinit-1.4.0a1691508515/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-08 15:33:20.207852 pulumi_cloudinit-1.4.0a1691508515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:33:20.203851 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:33:20.207852 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 15:33:20.000000 pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:33:20.211851 pulumi_cloudinit-1.4.0a1691508515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-08 15:33:19.000000 pulumi_cloudinit-1.4.0a1691508515/setup.py
```

### Comparing `pulumi_cloudinit-1.4.0a1691127304/PKG-INFO` & `pulumi_cloudinit-1.4.0a1691508515/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.4.0a1691127304
+Version: 1.4.0a1691508515
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi cloudinit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.4.0a1691127304/README.md` & `pulumi_cloudinit-1.4.0a1691508515/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-cloudinit
-Version: 1.4.0a1691127304
+Version: 1.4.0a1691508515
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi cloudinit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.4.0a1691127304/pulumi_cloudinit.egg-info/SOURCES.txt` & `pulumi_cloudinit-1.4.0a1691508515/pulumi_cloudinit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.4.0a1691127304/setup.py` & `pulumi_cloudinit-1.4.0a1691508515/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.4.0a1691127304"
-PLUGIN_VERSION = "1.4.0-alpha.1691127304+292fb6ed"
+VERSION = "1.4.0a1691508515"
+PLUGIN_VERSION = "1.4.0-alpha.1691508515+06495580"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cloudinit', PLUGIN_VERSION])
         except OSError as error:
```


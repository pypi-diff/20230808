# Comparing `tmp/system_config_tools-0.0.1.tar.gz` & `tmp/system_config_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_config_tools-0.0.1.tar", last modified: Tue Aug  8 07:14:57 2023, max compression
+gzip compressed data, was "system_config_tools-0.0.2.tar", last modified: Tue Aug  8 07:27:20 2023, max compression
```

## Comparing `system_config_tools-0.0.1.tar` & `system_config_tools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:57.454858 system_config_tools-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 07:14:41.000000 system_config_tools-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:14:57.454858 system_config_tools-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 07:14:41.000000 system_config_tools-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 07:14:41.000000 system_config_tools-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:14:57.458858 system_config_tools-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:57.454858 system_config_tools-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:14:41.000000 system_config_tools-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-08 07:14:41.000000 system_config_tools-0.0.1/src/sys_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:14:57.454858 system_config_tools-0.0.1/src/system_config_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:14:57.000000 system_config_tools-0.0.1/src/system_config_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 07:14:57.000000 system_config_tools-0.0.1/src/system_config_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:14:57.000000 system_config_tools-0.0.1/src/system_config_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:14:57.000000 system_config_tools-0.0.1/src/system_config_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:14:57.000000 system_config_tools-0.0.1/src/system_config_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.475768 system_config_tools-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/src/sys_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/src/system_config_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/top_level.txt
```

### Comparing `system_config_tools-0.0.1/LICENSE` & `system_config_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `system_config_tools-0.0.1/PKG-INFO` & `system_config_tools-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: system_config_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary:     Toolchain used to read configuration file by section.
 Author-email: Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Roberto Aldea <r.aldea.csic+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Project-URL: Homepage, https://github.com/WattRex/Battery-Cycler-Drivers
 Project-URL: Bug Tracker, https://github.com/WattRex/Battery-Cycler-Drivers/issues
 Keywords: yaml,configuration
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # System configuration module
 Module used for system configuration based on config file. Reads config yaml file
 and return it on a dictionary. It also allows to read sections of configuration
 files.
```

### Comparing `system_config_tools-0.0.1/pyproject.toml` & `system_config_tools-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "system_config_tools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Marius Crisan", email="mariuscrsn+pypi@gmail.com" },
   { name="Pablo Pastor", email="pastorpflores+pypi@gmail.com" },
   { name="Javier Sanz", email="javiersanzmoline@gmail.com" },
   { name="Roberto Aldea", email="r.aldea.csic+pypi@gmail.com" },
   { name="Luis Roche", email="luis.roche@hotmail.com" }
 ]
 keywords= ["yaml", "configuration"]
 
 description ="""
     Toolchain used to read configuration file by section."""
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Topic :: Software Development :: Embedded Systems",
     "Operating System :: OS Independent",
 ]
```

### Comparing `system_config_tools-0.0.1/src/sys_conf.py` & `system_config_tools-0.0.2/src/sys_conf.py`

 * *Files identical despite different names*

### Comparing `system_config_tools-0.0.1/src/system_config_tools.egg-info/PKG-INFO` & `system_config_tools-0.0.2/src/system_config_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: system-config-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary:     Toolchain used to read configuration file by section.
 Author-email: Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Roberto Aldea <r.aldea.csic+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
 Project-URL: Homepage, https://github.com/WattRex/Battery-Cycler-Drivers
 Project-URL: Bug Tracker, https://github.com/WattRex/Battery-Cycler-Drivers/issues
 Keywords: yaml,configuration
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # System configuration module
 Module used for system configuration based on config file. Reads config yaml file
 and return it on a dictionary. It also allows to read sections of configuration
 files.
```


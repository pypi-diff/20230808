# Comparing `tmp/system_config_tools-0.0.2.tar.gz` & `tmp/system_config_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_config_tools-0.0.2.tar", last modified: Tue Aug  8 07:27:20 2023, max compression
+gzip compressed data, was "/home/runner/work/System-Tools/System-Tools/dist/.tmp-7tbbmw2m/system_config_tools-0.0.3.tar", last modified: Tue Aug  8 09:14:20 2023, max compression
```

## Comparing `system_config_tools-0.0.2.tar` & `system_config_tools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.475768 system_config_tools-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-08 07:27:00.000000 system_config_tools-0.0.2/src/sys_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:27:20.479768 system_config_tools-0.0.2/src/system_config_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 07:27:20.000000 system_config_tools-0.0.2/src/system_config_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 09:13:56.000000 system_config_tools-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 09:13:56.000000 system_config_tools-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-08 09:13:56.000000 system_config_tools-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 09:13:56.000000 system_config_tools-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-08 09:13:56.000000 system_config_tools-0.0.3/src/sys_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 09:14:20.000000 system_config_tools-0.0.3/src/system_config_tools.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `system_config_tools-0.0.2/LICENSE` & `system_config_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `system_config_tools-0.0.2/PKG-INFO` & `system_config_tools-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: system_config_tools
-Version: 0.0.2
-Summary:     Toolchain used to read configuration file by section.
+Version: 0.0.3
+Summary: Toolchain used to read configuration file by section.
 Author-email: Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Roberto Aldea <r.aldea.csic+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
-Project-URL: Homepage, https://github.com/WattRex/Battery-Cycler-Drivers
+Project-URL: Homepage, https://github.com/WattRex/System-Tools
+Project-URL: Bug Reports, https://github.com/WattRex/System-Tools/issues
 Project-URL: Bug Tracker, https://github.com/WattRex/Battery-Cycler-Drivers/issues
+Project-URL: Source, https://github.com/WattRex/System-Tools
+Project-URL: Funding, https://donate.pypi.org
 Keywords: yaml,configuration
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # System configuration module
 Module used for system configuration based on config file. Reads config yaml file
 and return it on a dictionary. It also allows to read sections of configuration
 files.
```

### Comparing `system_config_tools-0.0.2/src/sys_conf.py` & `system_config_tools-0.0.3/src/sys_conf.py`

 * *Files identical despite different names*

### Comparing `system_config_tools-0.0.2/src/system_config_tools.egg-info/PKG-INFO` & `system_config_tools-0.0.3/src/system_config_tools.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 Metadata-Version: 2.1
 Name: system-config-tools
-Version: 0.0.2
-Summary:     Toolchain used to read configuration file by section.
+Version: 0.0.3
+Summary: Toolchain used to read configuration file by section.
 Author-email: Marius Crisan <mariuscrsn+pypi@gmail.com>, Pablo Pastor <pastorpflores+pypi@gmail.com>, Javier Sanz <javiersanzmoline@gmail.com>, Roberto Aldea <r.aldea.csic+pypi@gmail.com>, Luis Roche <luis.roche@hotmail.com>
-Project-URL: Homepage, https://github.com/WattRex/Battery-Cycler-Drivers
+Project-URL: Homepage, https://github.com/WattRex/System-Tools
+Project-URL: Bug Reports, https://github.com/WattRex/System-Tools/issues
 Project-URL: Bug Tracker, https://github.com/WattRex/Battery-Cycler-Drivers/issues
+Project-URL: Source, https://github.com/WattRex/System-Tools
+Project-URL: Funding, https://donate.pypi.org
 Keywords: yaml,configuration
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
 # System configuration module
 Module used for system configuration based on config file. Reads config yaml file
 and return it on a dictionary. It also allows to read sections of configuration
 files.
```


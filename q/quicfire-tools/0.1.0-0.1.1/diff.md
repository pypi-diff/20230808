# Comparing `tmp/quicfire-tools-0.1.0.tar.gz` & `tmp/quicfire-tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicfire-tools-0.1.0.tar", last modified: Tue Aug  8 15:40:10 2023, max compression
+gzip compressed data, was "quicfire-tools-0.1.1.tar", last modified: Tue Aug  8 18:30:52 2023, max compression
```

## Comparing `quicfire-tools-0.1.0.tar` & `quicfire-tools-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:40:10.650054 quicfire-tools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 15:40:10.650054 quicfire-tools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:40:10.650054 quicfire-tools-0.1.0/quicfire_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/quicfire_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/quicfire_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/quicfire_tools/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/quicfire_tools/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/quicfire_tools/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:40:10.650054 quicfire-tools-0.1.0/quicfire_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 15:40:10.000000 quicfire-tools-0.1.0/quicfire_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 15:40:10.000000 quicfire-tools-0.1.0/quicfire_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:40:10.000000 quicfire-tools-0.1.0/quicfire_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 15:40:10.000000 quicfire-tools-0.1.0/quicfire_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 15:40:10.000000 quicfire-tools-0.1.0/quicfire_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:40:10.650054 quicfire-tools-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 15:39:57.000000 quicfire-tools-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/quicfire_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/quicfire_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/setup.py
```

### Comparing `quicfire-tools-0.1.0/LICENSE` & `quicfire-tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.0/PKG-INFO` & `quicfire-tools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.1.0/quicfire_tools/inputs.py` & `quicfire-tools-0.1.1/quicfire_tools/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 
         Returns
         -------
         None:
             Sets up simulation files in the simulation directory.
 
         """
+        # Convert params to dict
+        params = params.to_dict()
+
         # Get current unix time
         params["timenow"] = int(time.time())
 
         # Write fuels data
         (params["fuel_density"], params["fuel_moisture"],
          params["fuel_height_flag"]) = self._write_fuel(params)
```

### Comparing `quicfire-tools-0.1.0/quicfire_tools/outputs.py` & `quicfire-tools-0.1.1/quicfire_tools/outputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.0/quicfire_tools/parameters.py` & `quicfire-tools-0.1.1/quicfire_tools/parameters.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.0/quicfire_tools.egg-info/PKG-INFO` & `quicfire-tools-0.1.1/quicfire_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.1.0/setup.py` & `quicfire-tools-0.1.1/setup.py`

 * *Files identical despite different names*


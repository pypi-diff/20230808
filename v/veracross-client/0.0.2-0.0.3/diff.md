# Comparing `tmp/veracross-client-0.0.2.tar.gz` & `tmp/veracross-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veracross-client-0.0.2.tar", last modified: Tue Aug  8 21:08:12 2023, max compression
+gzip compressed data, was "veracross-client-0.0.3.tar", last modified: Tue Aug  8 21:45:34 2023, max compression
```

## Comparing `veracross-client-0.0.2.tar` & `veracross-client-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/
--rw-rw-r--   0 hudson    (1000) hudson    (1000)     1074 2023-08-08 20:06:06.000000 veracross-client-0.0.2/LICENSE
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:08:12.016316 veracross-client-0.0.2/PKG-INFO
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       18 2023-08-08 20:06:06.000000 veracross-client-0.0.2/README.md
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      648 2023-08-08 21:08:03.000000 veracross-client-0.0.2/pyproject.toml
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      295 2023-08-08 21:08:12.016316 veracross-client-0.0.2/setup.cfg
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      351 2023-08-08 21:07:59.000000 veracross-client-0.0.2/setup.py
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/veracross_client/
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       45 2023-08-08 21:07:38.000000 veracross-client-0.0.2/src/veracross_client/__init__.py
--rw-rw-r--   0 hudson    (1000) hudson    (1000)   440433 2023-08-08 20:54:13.000000 veracross-client-0.0.2/src/veracross_client/veracross_client.py
-drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:08:12.016316 veracross-client-0.0.2/src/veracross_client.egg-info/
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      613 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/PKG-INFO
--rw-rw-r--   0 hudson    (1000) hudson    (1000)      344 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)        1 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       16 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/requires.txt
--rw-rw-r--   0 hudson    (1000) hudson    (1000)       17 2023-08-08 21:08:12.000000 veracross-client-0.0.2/src/veracross_client.egg-info/top_level.txt
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:45:34.835423 veracross-client-0.0.3/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)     1074 2023-08-08 20:06:06.000000 veracross-client-0.0.3/LICENSE
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)     2553 2023-08-08 21:45:34.835423 veracross-client-0.0.3/PKG-INFO
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)     1959 2023-08-08 21:44:34.000000 veracross-client-0.0.3/README.md
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      648 2023-08-08 21:45:18.000000 veracross-client-0.0.3/pyproject.toml
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      295 2023-08-08 21:45:34.835423 veracross-client-0.0.3/setup.cfg
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      351 2023-08-08 21:45:20.000000 veracross-client-0.0.3/setup.py
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:45:34.831423 veracross-client-0.0.3/src/
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:45:34.831423 veracross-client-0.0.3/src/veracross_client/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       45 2023-08-08 21:16:34.000000 veracross-client-0.0.3/src/veracross_client/__init__.py
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)   440413 2023-08-08 21:31:28.000000 veracross-client-0.0.3/src/veracross_client/veracross_client.py
+drwxrwxr-x   0 hudson    (1000) hudson    (1000)        0 2023-08-08 21:45:34.835423 veracross-client-0.0.3/src/veracross_client.egg-info/
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)     2553 2023-08-08 21:45:34.000000 veracross-client-0.0.3/src/veracross_client.egg-info/PKG-INFO
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)      344 2023-08-08 21:45:34.000000 veracross-client-0.0.3/src/veracross_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)        1 2023-08-08 21:45:34.000000 veracross-client-0.0.3/src/veracross_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       16 2023-08-08 21:45:34.000000 veracross-client-0.0.3/src/veracross_client.egg-info/requires.txt
+-rw-rw-r--   0 hudson    (1000) hudson    (1000)       17 2023-08-08 21:45:34.000000 veracross-client-0.0.3/src/veracross_client.egg-info/top_level.txt
```

### Comparing `veracross-client-0.0.2/LICENSE` & `veracross-client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `veracross-client-0.0.2/pyproject.toml` & `veracross-client-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "veracross-client"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hudson Harper", email="hudson@harpertech.io" },
 ]
 description = "Python wrapper for communicating with the Veracross API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `veracross-client-0.0.2/src/veracross_client/veracross_client.py` & `veracross-client-0.0.3/src/veracross_client/veracross_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5753,20 +5753,20 @@
             primary_teacher_id (int, optional): Only return classes taught by the specified primary teacher ID.
             room_id (int, optional): Only return classes taught in the specified room ID.
 
         Returns:
             pandas.DataFrame: A DataFrame containing the list of academic classes.
 
         """
-        if 'academics.classes:list' not in self.scopes:
+        if 'classes:list' not in self.scopes:
             print(
                 "Error: You don't have the required scope for this endpoint. Please add 'academics.classes:list' to your scopes.")
             return pd.DataFrame()
 
-        endpoint = "academics/classes"
+        endpoint = "classes"
         headers = {
             'Authorization': f'Bearer {self.access_token}',
             'X-API-Revision': x_api_revision,
             'X-API-Value-Lists': x_api_value_lists,
             'X-Page-Number': str(x_page_number),
             'X-Page-Size': str(x_page_size)
         }
```


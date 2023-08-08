# Comparing `tmp/automation_anywhere-2.1.6.tar.gz` & `tmp/automation_anywhere-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.1.6.tar", last modified: Fri Jun 16 20:30:12 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.7.tar", last modified: Tue Aug  8 13:49:56 2023, max compression
```

## Comparing `automation_anywhere-2.1.6.tar` & `automation_anywhere-2.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:30:12.117269 automation_anywhere-2.1.6/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.6/LICENSE
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-16 20:30:12.117269 automation_anywhere-2.1.6/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3470 2023-06-15 15:04:13.000000 automation_anywhere-2.1.6/README.md
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:30:12.117269 automation_anywhere-2.1.6/automation_anywhere/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.6/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.6/automation_anywhere/base.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.6/automation_anywhere/errors.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)    11891 2023-06-16 20:29:40.000000 automation_anywhere-2.1.6/automation_anywhere/executor.py
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-06-16 20:30:12.117269 automation_anywhere-2.1.6/automation_anywhere.egg-info/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-06-16 20:30:12.000000 automation_anywhere-2.1.6/automation_anywhere.egg-info/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-06-16 20:30:12.000000 automation_anywhere-2.1.6/automation_anywhere.egg-info/SOURCES.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-06-16 20:30:12.000000 automation_anywhere-2.1.6/automation_anywhere.egg-info/dependency_links.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-06-16 20:30:12.000000 automation_anywhere-2.1.6/automation_anywhere.egg-info/top_level.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-06-16 20:29:47.000000 automation_anywhere-2.1.6/pyproject.toml
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-06-16 20:30:12.117269 automation_anywhere-2.1.6/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-08-08 13:49:56.473824 automation_anywhere-2.1.7/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.7/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-08-08 13:49:56.473824 automation_anywhere-2.1.7/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3470 2023-06-15 15:04:13.000000 automation_anywhere-2.1.7/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-08-08 13:49:56.473824 automation_anywhere-2.1.7/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.7/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.7/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.7/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    12113 2023-08-07 18:01:55.000000 automation_anywhere-2.1.7/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-08-08 13:49:56.473824 automation_anywhere-2.1.7/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4047 2023-08-08 13:49:56.000000 automation_anywhere-2.1.7/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-08-08 13:49:56.000000 automation_anywhere-2.1.7/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-08-08 13:49:56.000000 automation_anywhere-2.1.7/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-08-08 13:49:56.000000 automation_anywhere-2.1.7/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-08-08 13:47:42.000000 automation_anywhere-2.1.7/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-08-08 13:49:56.473824 automation_anywhere-2.1.7/setup.cfg
```

### Comparing `automation_anywhere-2.1.6/LICENSE` & `automation_anywhere-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.6/PKG-INFO` & `automation_anywhere-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_anywhere
-Version: 2.1.6
+Version: 2.1.7
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.6/README.md` & `automation_anywhere-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.6/automation_anywhere/base.py` & `automation_anywhere-2.1.7/automation_anywhere/base.py`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.6/automation_anywhere/executor.py` & `automation_anywhere-2.1.7/automation_anywhere/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         :type page: dict, optional
         :param run_as_user: If configured, it'll search for the exact username on the "defaultUsers" list, in order to filter it, defaults to None
         :type run_as_user: str, optional
         :param hostname: If configured, it'll search for the hostname (as a substring) on all the devices the user has permission to see, defaults to None
         :type hostname: str, optional
         :param custom_filter: If sent, it'll add to the other filters on the query, defaults to None
         :type custom_filter: dict, optional
-        :return: A tuple with a list of devices, a list of page data and a string to show errors
+        :return: A tuple with a list of devices, a list of page data and a string to show errors. The list of page data may be None sometimes.
         :rtype: tuple[list, dict, str]
         """
         devices = None
         page_data = None
         error = None
         endpoint = f'{self._base_url}v2/devices/list'
         payload = dict()
@@ -51,15 +51,19 @@
         local_filter = {'operator': 'and', 'operands': []}
         if hostname:
             local_filter['operands'].append({'operator': 'substring', 'field': 'hostName', 'value': hostname})
         if custom_filter:
             local_filter['operands'].append(custom_filter)
         response = post(url=endpoint, headers=self.headers, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
-            page_data = response.json()['page']
+            try:
+                # Sometimes the 'page' is missing from the AA Return, so just check for them
+                page_data = response.json()['page']
+            except KeyError:
+                page_data = None
             devices = response.json()['list']
             if run_as_user:
                 found_devices = list()
                 for device in devices:
                     found_users = next((x for x in device['defaultUsers'] if x['username'] == run_as_user), None)
                     if found_users:
                         found_devices.append(device.copy())
```

### Comparing `automation_anywhere-2.1.6/automation_anywhere.egg-info/PKG-INFO` & `automation_anywhere-2.1.7/automation_anywhere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-anywhere
-Version: 2.1.6
+Version: 2.1.7
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.6/pyproject.toml` & `automation_anywhere-2.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="automation_anywhere"
-version="2.1.6"
+version="2.1.7"
 authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
 description="A Python Package to deploy tasks on Automation Anywhere 360"
 readme="README.md"
 requires-python=">=3.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```


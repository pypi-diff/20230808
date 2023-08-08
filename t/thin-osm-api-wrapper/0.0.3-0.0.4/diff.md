# Comparing `tmp/thin_osm_api_wrapper-0.0.3.tar.gz` & `tmp/thin_osm_api_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thin_osm_api_wrapper-0.0.3.tar", last modified: Fri Jul 21 15:08:12 2023, max compression
+gzip compressed data, was "thin_osm_api_wrapper-0.0.4.tar", last modified: Tue Aug  8 10:44:48 2023, max compression
```

## Comparing `thin_osm_api_wrapper-0.0.3.tar` & `thin_osm_api_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1383 2023-03-06 02:35:50.000000 thin_osm_api_wrapper-0.0.3/README.md
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/setup.cfg
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2023-07-21 15:08:03.000000 thin_osm_api_wrapper-0.0.3/setup.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.696694 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/__init__.py
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     4339 2023-07-21 15:07:23.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/api.py
-drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-07-21 15:08:12.697694 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2023-07-21 15:08:12.000000 thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-08-08 10:44:48.554196 thin_osm_api_wrapper-0.0.4/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-08-08 10:44:48.554196 thin_osm_api_wrapper-0.0.4/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     1383 2023-03-06 02:35:50.000000 thin_osm_api_wrapper-0.0.4/README.md
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       38 2023-08-08 10:44:48.554196 thin_osm_api_wrapper-0.0.4/setup.cfg
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      740 2023-08-08 10:44:01.000000 thin_osm_api_wrapper-0.0.4/setup.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-08-08 10:44:48.554196 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       31 2022-12-24 14:34:38.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper/__init__.py
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     4391 2023-08-08 10:43:33.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper/api.py
+drwxrwxr-x   0 mateusz   (1000) mateusz   (1001)        0 2023-08-08 10:44:48.554196 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)     2290 2023-08-08 10:44:48.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)      255 2023-08-08 10:44:48.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)        1 2023-08-08 10:44:48.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1000) mateusz   (1001)       21 2023-08-08 10:44:48.000000 thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/top_level.txt
```

### Comparing `thin_osm_api_wrapper-0.0.3/PKG-INFO` & `thin_osm_api_wrapper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin_osm_api_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: thin wrapper of https://wiki.openstreetmap.org/wiki/API
 Home-page: https://github.com/matkoniecz/thin_osm_api_python_wrapper
 Author: Mateusz Konieczny
 License: UNKNOWN
 Description: # Replaced
         See [osm_easy_api](https://github.com/docentYT/osm_easy_api)
```

### Comparing `thin_osm_api_wrapper-0.0.3/README.md` & `thin_osm_api_wrapper-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `thin_osm_api_wrapper-0.0.3/setup.py` & `thin_osm_api_wrapper-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thin_osm_api_wrapper",
-    version="0.0.3",
+    version="0.0.4",
     author="Mateusz Konieczny",
     description="thin wrapper of https://wiki.openstreetmap.org/wiki/API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/matkoniecz/thin_osm_api_python_wrapper",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper/api.py` & `thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 from lxml import etree
+import time
 
 def history_json(object_type, object_id, user_agent=None):
     url = 'https://api.openstreetmap.org/api/0.6/' + object_type + '/' + str(object_id) + '/history.json'
     params = {}
     if user_agent != None:
         params = {
             'user_agent': user_agent
@@ -103,9 +104,10 @@
         # not sure is it happening on poor connection or explicit request by server
         # to slow down, in either case waiting a bit is a good idea
         except urllib3.exceptions.ProtocolError as e:
             print(e)
             sleep_before_retry("urllib3.exceptions.ProtocolError", url, params, json_data)
             continue
 
-if __name__ == "__main__":
-    element_list_touched_by_changeset('133124436')
+def sleep_before_retry(message, url, params, json_data):
+    time.sleep(10)
+    print(message, url, params, json_data)
```

### Comparing `thin_osm_api_wrapper-0.0.3/thin_osm_api_wrapper.egg-info/PKG-INFO` & `thin_osm_api_wrapper-0.0.4/thin_osm_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thin-osm-api-wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: thin wrapper of https://wiki.openstreetmap.org/wiki/API
 Home-page: https://github.com/matkoniecz/thin_osm_api_python_wrapper
 Author: Mateusz Konieczny
 License: UNKNOWN
 Description: # Replaced
         See [osm_easy_api](https://github.com/docentYT/osm_easy_api)
```


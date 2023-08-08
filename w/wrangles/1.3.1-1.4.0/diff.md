# Comparing `tmp/wrangles-1.3.1.tar.gz` & `tmp/wrangles-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.3.1.tar", last modified: Tue Jun 13 22:13:05 2023, max compression
+gzip compressed data, was "wrangles-1.4.0.tar", last modified: Tue Aug  8 18:37:46 2023, max compression
```

## Comparing `wrangles-1.3.1.tar` & `wrangles-1.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.189765 wrangles-1.3.1/
--rw-rw-rw-   0        0        0     3615 2023-06-13 22:13:05.189765 wrangles-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.166825 wrangles-1.3.1/Wrangles.egg-info/
--rw-rw-rw-   0        0        0     3615 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1573 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      159 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 22:13:05.000000 wrangles-1.3.1/Wrangles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 22:13:05.190761 wrangles-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-06-13 22:13:01.000000 wrangles-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.164832 wrangles-1.3.1/wrangles/
--rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.3.1/wrangles/__init__.py
--rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/auth.py
--rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/batching.py
--rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/classify.py
--rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.182782 wrangles-1.3.1/wrangles/connectors/
--rw-rw-rw-   0        0        0      449 2023-05-15 15:40:44.000000 wrangles-1.3.1/wrangles/connectors/__init__.py
--rw-rw-rw-   0        0        0     7108 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/akeneo.py
--rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/ckan.py
--rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/file.py
--rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/http.py
--rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/jinja.py
--rw-rw-rw-   0        0        0     4830 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/mongodb.py
--rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/mssql.py
--rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/mysql.py
--rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/notification.py
--rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.3.1/wrangles/connectors/postgres.py
--rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/pricefx.py
--rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/connectors/recipe.py
--rw-rw-rw-   0        0        0     8527 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/s3.py
--rw-rw-rw-   0        0        0     4754 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/connectors/salesforce.py
--rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/sftp.py
--rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.3.1/wrangles/connectors/ssh.py
--rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.3.1/wrangles/connectors/test.py
--rw-rw-rw-   0        0        0     8037 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/connectors/train.py
--rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/console.py
--rw-rw-rw-   0        0        0     1588 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/data.py
--rw-rw-rw-   0        0        0    10100 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/extract.py
--rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/format.py
--rw-rw-rw-   0        0        0    22513 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/recipe.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:13:05.188768 wrangles-1.3.1/wrangles/recipe_wrangles/
--rw-rw-rw-   0        0        0      585 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/convert.py
--rw-rw-rw-   0        0        0     8695 2023-06-13 22:13:01.000000 wrangles-1.3.1/wrangles/recipe_wrangles/create.py
--rw-rw-rw-   0        0        0    21176 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/extract.py
--rw-rw-rw-   0        0        0     8126 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/format.py
--rw-rw-rw-   0        0        0    27181 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/main.py
--rw-rw-rw-   0        0        0     8584 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/merge.py
--rw-rw-rw-   0        0        0     4041 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/pandas.py
--rw-rw-rw-   0        0        0     8715 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/select.py
--rw-rw-rw-   0        0        0     6791 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/recipe_wrangles/split.py
--rw-rw-rw-   0        0        0     1883 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/select.py
--rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.3.1/wrangles/standardize.py
--rw-rw-rw-   0        0        0     6067 2023-06-09 22:13:53.000000 wrangles-1.3.1/wrangles/train.py
--rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.3.1/wrangles/translate.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:37:46.293949 wrangles-1.4.0/
+-rw-rw-rw-   0        0        0     3615 2023-08-08 18:37:46.293949 wrangles-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:37:46.272008 wrangles-1.4.0/Wrangles.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1573 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      165 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 18:37:46.000000 wrangles-1.4.0/Wrangles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-08 18:37:46.297939 wrangles-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-08-08 18:00:54.000000 wrangles-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:37:46.270012 wrangles-1.4.0/wrangles/
+-rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.4.0/wrangles/__init__.py
+-rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/auth.py
+-rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/batching.py
+-rw-rw-rw-   0        0        0     2080 2023-07-21 21:17:23.000000 wrangles-1.4.0/wrangles/classify.py
+-rw-rw-rw-   0        0        0      754 2023-08-08 17:38:17.000000 wrangles-1.4.0/wrangles/config.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:37:46.285976 wrangles-1.4.0/wrangles/connectors/
+-rw-rw-rw-   0        0        0      449 2023-05-15 15:40:44.000000 wrangles-1.4.0/wrangles/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7108 2023-06-13 22:13:01.000000 wrangles-1.4.0/wrangles/connectors/akeneo.py
+-rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.4.0/wrangles/connectors/ckan.py
+-rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.4.0/wrangles/connectors/file.py
+-rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/connectors/http.py
+-rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.4.0/wrangles/connectors/jinja.py
+-rw-rw-rw-   0        0        0     4830 2023-06-13 22:13:01.000000 wrangles-1.4.0/wrangles/connectors/mongodb.py
+-rw-rw-rw-   0        0        0     6942 2023-08-08 15:52:45.000000 wrangles-1.4.0/wrangles/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4889 2023-08-08 15:52:45.000000 wrangles-1.4.0/wrangles/connectors/mysql.py
+-rw-rw-rw-   0        0        0     8286 2023-08-03 14:40:43.000000 wrangles-1.4.0/wrangles/connectors/notification.py
+-rw-rw-rw-   0        0        0     8752 2023-08-08 15:52:45.000000 wrangles-1.4.0/wrangles/connectors/postgres.py
+-rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/connectors/pricefx.py
+-rw-rw-rw-   0        0        0     4534 2023-08-08 17:58:45.000000 wrangles-1.4.0/wrangles/connectors/recipe.py
+-rw-rw-rw-   0        0        0     8527 2023-06-13 22:13:01.000000 wrangles-1.4.0/wrangles/connectors/s3.py
+-rw-rw-rw-   0        0        0     4754 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/connectors/salesforce.py
+-rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.4.0/wrangles/connectors/sftp.py
+-rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.4.0/wrangles/connectors/ssh.py
+-rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.4.0/wrangles/connectors/test.py
+-rw-rw-rw-   0        0        0     8037 2023-06-13 22:13:01.000000 wrangles-1.4.0/wrangles/connectors/train.py
+-rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/console.py
+-rw-rw-rw-   0        0        0     1822 2023-07-21 21:34:01.000000 wrangles-1.4.0/wrangles/data.py
+-rw-rw-rw-   0        0        0     9955 2023-07-21 21:17:23.000000 wrangles-1.4.0/wrangles/extract.py
+-rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.4.0/wrangles/format.py
+-rw-rw-rw-   0        0        0    26941 2023-08-08 17:38:17.000000 wrangles-1.4.0/wrangles/recipe.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:37:46.292952 wrangles-1.4.0/wrangles/recipe_wrangles/
+-rw-rw-rw-   0        0        0      585 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/recipe_wrangles/__init__.py
+-rw-rw-rw-   0        0        0     8620 2023-07-21 14:06:13.000000 wrangles-1.4.0/wrangles/recipe_wrangles/convert.py
+-rw-rw-rw-   0        0        0     8882 2023-08-08 17:38:17.000000 wrangles-1.4.0/wrangles/recipe_wrangles/create.py
+-rw-rw-rw-   0        0        0    21179 2023-07-21 21:17:23.000000 wrangles-1.4.0/wrangles/recipe_wrangles/extract.py
+-rw-rw-rw-   0        0        0     8126 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/recipe_wrangles/format.py
+-rw-rw-rw-   0        0        0    27597 2023-08-08 18:01:11.000000 wrangles-1.4.0/wrangles/recipe_wrangles/main.py
+-rw-rw-rw-   0        0        0     8584 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/recipe_wrangles/merge.py
+-rw-rw-rw-   0        0        0     4041 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/recipe_wrangles/pandas.py
+-rw-rw-rw-   0        0        0     8964 2023-07-21 14:06:13.000000 wrangles-1.4.0/wrangles/recipe_wrangles/select.py
+-rw-rw-rw-   0        0        0     6870 2023-08-08 17:38:17.000000 wrangles-1.4.0/wrangles/recipe_wrangles/split.py
+-rw-rw-rw-   0        0        0     1883 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/select.py
+-rw-rw-rw-   0        0        0     2110 2023-07-21 21:17:23.000000 wrangles-1.4.0/wrangles/standardize.py
+-rw-rw-rw-   0        0        0     6067 2023-06-09 22:13:53.000000 wrangles-1.4.0/wrangles/train.py
+-rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.4.0/wrangles/translate.py
```

### Comparing `wrangles-1.3.1/PKG-INFO` & `wrangles-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.3.1
+Version: 1.4.0
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.3.1/README.md` & `wrangles-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/Wrangles.egg-info/PKG-INFO` & `wrangles-1.4.0/Wrangles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.3.1
+Version: 1.4.0
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.3.1/Wrangles.egg-info/SOURCES.txt` & `wrangles-1.4.0/Wrangles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/setup.py` & `wrangles-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.3.1',
+    version = '1.4.0',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.3.1/wrangles/__init__.py` & `wrangles-1.4.0/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/auth.py` & `wrangles-1.4.0/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/batching.py` & `wrangles-1.4.0/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/classify.py` & `wrangles-1.4.0/wrangles/classify.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,14 @@
     if model_properties.get('message', None) == 'error': raise ValueError('Incorrect model_id.\nmodel_id may be wrong or does not exists')
     batch_size = model_properties['batch_size'] or 5000
     
     
     # Using model_id in wrong function
     purpose = model_properties['purpose']
     if purpose != 'classify':
-        raise ValueError(f'Using {purpose} model_id in a classify function.')
+        raise ValueError(f'Using {purpose} model_id {model_id} in a classify function.')
 
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
     if isinstance(input, str): results = results[0]
 
     return results
```

### Comparing `wrangles-1.3.1/wrangles/connectors/akeneo.py` & `wrangles-1.4.0/wrangles/connectors/akeneo.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/ckan.py` & `wrangles-1.4.0/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/file.py` & `wrangles-1.4.0/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/http.py` & `wrangles-1.4.0/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/jinja.py` & `wrangles-1.4.0/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/mongodb.py` & `wrangles-1.4.0/wrangles/connectors/mongodb.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/mssql.py` & `wrangles-1.4.0/wrangles/connectors/mssql.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,40 +6,41 @@
 import logging as _logging
 import pymssql as _pymssql
 
 
 _schema = {}
 
 
-def read(host: str, user: str, password: str, command: str, port = 1433, database: str = '', columns: _Union[str, list] = None) -> _pd.DataFrame:
+def read(host: str, user: str, password: str, command: str, port = 1433, database: str = '', columns: _Union[str, list] = None, params: _Union[list, dict] = None) -> _pd.DataFrame:
     """
     Import data from a Microsoft SQL database.
 
     >>> from wrangles.connectors import mssql
     >>> df = mssql.read(host='sql.domain', user='user', password='password', command='SELECT * FROM table')
 
     :param host: Hostname or IP of the database
     :param user: User with access to the database
     :param password: Password of user
     :param command: SQL command or table name
     :param port: (Optional) If not provided, the default port will be used
     :param database: (Optional) Database to be queried
     :param columns: (Optional) Subset of columns to be returned. This is less efficient than specifying in the SQL command.
+    :param params: (Optional) List of parameters to pass to execute method. The syntax used to pass parameters is database driver dependent.
     :return: Pandas Dataframe of the imported data
     """
     _logging.info(f": Importing Data :: {host}")
 
     conn = f"mssql+pymssql://{user}:{password}@{host}:{port}/{database}?charset=utf8"
-    df = _pd.read_sql(command, conn)
+    df = _pd.read_sql(command, conn, params)
 
     if columns is not None: df = df[columns]
     
     return df
 
-_schema['read'] = """
+_schema['read'] = r"""
 type: object
 description: Import data from a Microsoft SQL Server
 required:
   - host
   - user
   - password
   - command
@@ -51,24 +52,35 @@
     type: string
     description: The user to connect to the database with
   password:
     type: string
     description: Password for the specified user
   command:
     type: string
-    description: Table name or SQL command to select data
+    description: |-
+      Table name or SQL command to select data.
+      Note - using variables here can make your recipe vulnerable
+      to sql injection. Use params if using variables from
+      untrusted sources.
   database:
     type: string
     description: The database to connect to
   port:
     type: integer
     description: The Port to connect to. Defaults to 1433.
   columns:
     type: array
     description: A list with a subset of the columns to import. This is less efficient than specifying in the command.
+  params:
+    type: 
+      - array
+      - dict
+    description: |-
+      List of parameters to pass to execute method.
+      This may use %s or %(name)s syntax
 """
 
 
 def write(df: _pd.DataFrame, host: str, database: str, table: str, user: str, password: str, action = 'INSERT', port = 1433, columns: _Union[str, list] = None) -> None:
     """
     Export data to a Microsoft SQL database.
 
@@ -129,37 +141,45 @@
     description: The Port to connect to. Defaults to 1433.
   columns:
     type: array
     description: A list of the columns to write to the table. If omitted, all columns will be written.
 """
 
 
-def run(host: str, user: str, password: str, command: _Union[str, list], **kwargs) -> None:
+def run(
+  host: str,
+  user: str,
+  password: str,
+  command: _Union[str, list],
+  params: _Union[list, dict] = None,
+  **kwargs
+) -> None:
   """
   Run a command on a Microsoft SQL Server
 
   >>> from wrangles.connectors import mssql
-  >>> df = mssql.run(host='sql.domain', user='user', password='password', command='exec myStoredProcedure')
+  >>> mssql.run(host='sql.domain', user='user', password='password', command='exec myStoredProcedure')
 
   :param host: Hostname or IP of the database
   :param user: User with access to the database
   :param password: Password of user
   :param command: SQL command or a list of SQL commands to execute
+  :param params: Variables to pass to a parameterized query.
   """
   _logging.info(f": Executing Command :: {host}")
 
   # If user has provided a single command, convert to a list of one.
   if isinstance(command, str): command = [command]
 
   # Establish connection
   conn = _pymssql.connect(server=host, user=user, password=password, autocommit=True, **kwargs)
   cursor = conn.cursor()
 
   for sql in command:
-    cursor.execute(sql)
+    cursor.execute(sql, params)
 
   conn.close()
 
 _schema['run'] = """
 type: object
 description: Run a command against a Microsoft SQL Server such as triggering a query or stored procedure
 required:
@@ -184,8 +204,15 @@
     description: SQL command or a list of SQL commands to execute
   database:
     type: string
     description: The database to connect to
   port:
     type: integer
     description: The Port to connect to. Defaults to 1433.
+  params:
+    type:
+      - array
+      - object
+    description: |-
+      Variables to pass to a parameterized query.
+      This may use %s or %(name)s syntax
 """
```

### Comparing `wrangles-1.3.1/wrangles/connectors/mysql.py` & `wrangles-1.4.0/wrangles/connectors/mysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 from typing import Union as _Union
 import logging as _logging
 
 
 _schema = {}
 
 
-def read(host: str, user: str, password: str, command: str, port = 3306, database: str = '', columns: _Union[str, list] = None) -> _pd.DataFrame:
+def read(host: str, user: str, password: str, command: str, port = 3306, database: str = '', columns: _Union[str, list] = None, params: _Union[list, dict] = None) -> _pd.DataFrame:
     """
     Import data from a MySQL database.
 
     >>> from wrangles.connectors import mysql
     >>> df = mysql.read(host='sql.domain', user='user', password='password', command='SELECT * FROM table')
 
     :param host: Hostname or IP of the database
     :param user: User with access to the database
     :param password: Password of user
     :param command: SQL command or table name
     :param port: (Optional) If not provided, the default port will be used
     :param database: (Optional) Database to be queried
     :param columns: (Optional) Subset of columns to be returned. This is less efficient than specifying in the SQL command.
+    :param params: (Optional) List of parameters to pass to execute method. The syntax used to pass parameters is database driver dependent.
     :return: Pandas Dataframe of the imported data
     """
     _logging.info(f": Importing Data :: {host}")
 
     conn = f"mysql+pymysql://{user}:{password}@{host}:{port}/{database}"
-    df = _pd.read_sql(command, conn)
+    df = _pd.read_sql(command, conn, params)
 
     if columns is not None: df = df[columns]
     
     return df
 
 _schema['read'] = """
 type: object
@@ -50,24 +51,35 @@
     type: string
     description: The user to connect to the database with
   password:
     type: string
     description: Password for the specified user
   command:
     type: string
-    description: Table name or SQL command to select data
+    description: |-
+      Table name or SQL command to select data.
+      Note - using variables here can make your recipe vulnerable
+      to sql injection. Use params if using variables from
+      untrusted sources.
   database:
     type: string
     description: The database to connect to
   port:
     type: integer
     description: The Port to connect to. Defaults to 3306.
   columns:
     type: array
     description: A list with a subset of the columns to import. This is less efficient than specifying in the command.
+  params:
+    type: 
+      - array
+      - dict
+    description: |-
+      List of parameters to pass to execute method.
+      This may use %s or %(name)s syntax
 """
 
 
 def write(df: _pd.DataFrame, host: str, database: str, table: str, user: str, password: str, action = 'INSERT', port = 3306, columns: _Union[str, list] = None) -> None:
     """
     Export data to a MySQL database.
```

### Comparing `wrangles-1.3.1/wrangles/connectors/postgres.py` & `wrangles-1.4.0/wrangles/connectors/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Connector to read/write from a PostgreSQL Database.
 """
 import pandas as _pd
 from typing import Union as _Union
 import logging as _logging
 import csv as _csv
 from io import StringIO as _StringIO
+import psycopg2 as _psycopg2
 
 
 _schema = {}
 
 
 # Internal methods - custom sql callbacks 
 def _psql_insert_copy(table, conn, keys, data_iter):
@@ -39,40 +40,41 @@
             table_name = table.name
 
         sql = 'COPY {} ({}) FROM STDIN WITH CSV'.format(table_name, columns)
         cur.copy_expert(sql=sql, file=s_buf)
 
 
 # Public methods
-def read(host: str, user: str, password: str, command: str, port = 5432, database: str = '', columns: _Union[str, list] = None) -> _pd.DataFrame:
+def read(host: str, user: str, password: str, command: str, port = 5432, database: str = '', columns: _Union[str, list] = None, params: _Union[list, dict] = None) -> _pd.DataFrame:
     """
     Import data from a PostgreSQL database.
 
     >>> from wrangles.connectors import postgres
     >>> df = postgres.read(host='sql.domain', user='user', password='password', command='SELECT * FROM table')
 
     :param host: Hostname or IP of the database
     :param user: User with access to the database
     :param password: Password of user
     :param command: SQL command or table name
     :param port: (Optional) If not provided, the default port will be used
     :param database: (Optional) Database to be queried
     :param columns: (Optional) Subset of columns to be returned. This is less efficient than specifying in the SQL command.
+    :param params: (Optional) List of parameters to pass to execute method. The syntax used to pass parameters is database driver dependent.
     :return: Pandas Dataframe of the imported data
     """
     _logging.info(f": Importing Data :: {host}")
 
     conn = f"postgresql+psycopg2://{user}:{password}@{host}:{port}/{database}"
-    df = _pd.read_sql(command, conn)
+    df = _pd.read_sql(command, conn, params)
 
     if columns is not None: df = df[columns]
     
     return df
 
-_schema['read'] = """
+_schema['read'] = r"""
 type: object
 description: Import data from a PostgreSQL Server
 required:
   - host
   - user
   - password
   - command
@@ -84,24 +86,35 @@
     type: string
     description: The user to connect to the database with
   password:
     type: string
     description: Password for the specified user
   command:
     type: string
-    description: Table name or SQL command to select data
+    description: |-
+      Table name or SQL command to select data.
+      Note - using variables here can make your recipe vulnerable
+      to sql injection. Use params for variables from
+      untrusted sources.
   database:
     type: string
     description: The database to connect to
   port:
     type: integer
     description: The Port to connect to. Defaults to 5432.
   columns:
     type: array
     description: A list with a subset of the columns to import. This is less efficient than specifying in the command.
+  params:
+    type: 
+      - array
+      - dict
+    description: |-
+      List of parameters to pass to execute method.
+      This may use %s or %(name)s syntax
 """
 
 
 def write(df: _pd.DataFrame, host: str, database: str, table: str, user: str, password: str, action = 'INSERT', port = 5432, columns: _Union[str, list] = None) -> None:
     """
     Export data to a PostgreSQL database.
 
@@ -165,8 +178,97 @@
     description: The name of the table to insert the data into
   port:
     type: integer
     description: The Port to connect to. Defaults to 5432.
   columns:
     type: array
     description: A list of the columns to write to the table. If omitted, all columns will be written.
-"""
+"""
+
+
+def run(
+    host: str,
+    database: str,
+    user: str,
+    password: str,
+    command: _Union[str, list],
+    port = 5432,
+    params: _Union[list, dict] = None
+) -> None:
+    """
+    Run a command on a PostgreSQL Server
+
+    >>> wrangles.connectors.postgres.run(
+    >>>    host='sql.domain',
+    >>>    database='db',
+    >>>    user='user',
+    >>>    password='password',
+    >>>    command='CALL myStoredProcedure'
+    >>> )
+
+    :param host: Hostname or IP of the database
+    :param database: The name of the database
+    :param user: User with access to the database
+    :param password: Password of user
+    :param command: SQL command or a list of SQL commands to execute
+    :param port: The Port to connect to. Defaults to 5432.
+    :param params: Variables to pass to a parameterized query.
+    """
+    _logging.info(f": Executing Command :: {host}")
+
+    # If user has provided a single command, convert to a list of one.
+    if isinstance(command, str): command = [command]
+
+    # Establish connection
+    conn = _psycopg2.connect(
+        host = host,
+        port = port,
+        dbname = database,
+        user = user,
+        password = password
+    )
+    conn.autocommit = True
+    cursor = conn.cursor()
+
+    for sql in command:
+        cursor.execute(sql, params)
+
+    conn.close()
+
+_schema['run'] = r"""
+type: object
+description: Run a command against a PostgreSQL Server such as triggering a query or stored procedure
+required:
+  - host
+  - database
+  - user
+  - password
+  - command
+properties:
+  host:
+    type: string
+    description: Hostname or IP address of the server
+  database:
+    type: string
+    description: The name of the database to execute the query against
+  user:
+    type: string
+    description: The user to connect to the server as
+  password:
+    type: string
+    description: Password for the specified user
+  command:
+    type:
+      - string
+      - array
+    description: SQL command or a list of SQL commands to execute
+  port:
+    type: integer
+    description: The Port to connect to. Defaults to 5432.
+  params:
+    type:
+      - array
+      - object
+    description: |-
+      Variables to pass to a parameterized query.
+      This may use %s or %(name)s syntax
+"""
```

### Comparing `wrangles-1.3.1/wrangles/connectors/pricefx.py` & `wrangles-1.4.0/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/recipe.py` & `wrangles-1.4.0/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/s3.py` & `wrangles-1.4.0/wrangles/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/salesforce.py` & `wrangles-1.4.0/wrangles/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/sftp.py` & `wrangles-1.4.0/wrangles/connectors/sftp.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/ssh.py` & `wrangles-1.4.0/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/test.py` & `wrangles-1.4.0/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/connectors/train.py` & `wrangles-1.4.0/wrangles/connectors/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/console.py` & `wrangles-1.4.0/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/data.py` & `wrangles-1.4.0/wrangles/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,9 +43,15 @@
 
     :param id: Model ID
     :param purpose: classify, extract, standardize
     :return: Model data as a list of lists
     """
     params = {'model_id': id, 'type': purpose}
     response = _requests.get(f'{_config.api_host}/model/content', params=params, headers={'Authorization': f'Bearer {_auth.get_access_token()}'})
-    results = response.json()
+    if response.ok:
+        results = response.json()
+    elif response.status_code in [401, 403]:
+        raise RuntimeError('Not able to validate access, check wrangle to ensure accessibility')
+    else:
+        raise RuntimeError('Model data not found')
+
     return results['Data']
```

### Comparing `wrangles-1.3.1/wrangles/extract.py` & `wrangles-1.4.0/wrangles/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,37 +115,32 @@
     else:
         raise TypeError('Invalid input data provided. The input must be either a string or a list of strings.')
         
     # If the Model Id is not appropriate, raise error (Only for Recipes)
     if isinstance(model_id, dict):
         raise ValueError('Incorrect model_id type.\nIf using Recipe, may be missing "${ }" around value')
     
-    # If the model_id is a list, then split the contents
-    if isinstance(model_id, str): model_id = [model_id]
-    for model in model_id:
-        # Checking to see if GUID format is correct
-        if [len(x) for x in model.split('-')] != [8, 4, 4]:
-            raise ValueError('Incorrect or missing values in model_id. Check format is XXXXXXXX-XXXX-XXXX')
+    # Checking to see if GUID format is correct
+    if [len(x) for x in model_id.split('-')] != [8, 4, 4]:
+        raise ValueError('Incorrect or missing values in model_id. Check format is XXXXXXXX-XXXX-XXXX')
 
     url = f'{_config.api_host}/wrangles/extract/custom'
     params = {'responseFormat': 'array', 'model_id': model_id, 'use_labels': use_labels}
     model_properties = _data.model(model_id)
     # If model_id format is correct but no mode_id exists
     if model_properties.get('message', None) == 'error': raise ValueError('Incorrect model_id.\nmodel_id may be wrong or does not exists')
     batch_size = model_properties['batch_size'] or 10000
     
     # Using model_id in wrong function
     purpose = model_properties['purpose']
     if purpose != 'extract':
-        raise ValueError(f'Using {purpose} model_id in an extract function.')
+        raise ValueError(f'Using {purpose} model_id {model_id} in an extract function.')
     
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
-
-
     if first_element and not use_labels:
         results = [x[0] if len(x) >= 1 else "" for x in results]
     
     if use_labels and first_element:
         results = [{k:v[0] for (k, v) in zip(objs.keys(), objs.values())} for objs in results]
```

### Comparing `wrangles-1.3.1/wrangles/format.py` & `wrangles-1.4.0/wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/recipe.py` & `wrangles-1.4.0/wrangles/recipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import inspect as _inspect
 import re as _re
 import warnings as _warnings
 import pandas as _pandas
 import requests as _requests
 from . import recipe_wrangles as _recipe_wrangles
 from . import connectors as _connectors
+from .config import no_where_list
 
 
 _logging.getLogger().setLevel(_logging.INFO)
 
 
 # Suppress pandas performance warnings
 # this appears in some instances during the recipe execution when generating new columns.
@@ -271,14 +272,29 @@
     :return: Pandas Dataframe of the Wrangled data
     """
     for step in wrangles_list:
         for wrangle, params in step.items():
             if params is None: params = {}
             _logging.info(f": Wrangling :: {wrangle} :: {params.get('input', 'None')} >> {params.get('output', 'Dynamic')}")
 
+            original_params = params.copy()
+            if 'where' in params.keys() and wrangle not in no_where_list:
+                df_original = df.copy()
+                
+                # Save original index, filter data, then restore index
+                df['original_index_ikdejsrvjazl'] = df.index
+                df = _filter_dataframe(
+                    df,
+                    where = params.pop('where'),
+                    where_params= params.pop('where_params', None)
+                )
+                df = df.set_index(df['original_index_ikdejsrvjazl'])
+                df = df.drop('original_index_ikdejsrvjazl', axis = 1)
+                df.index.names = [None]
+
             if wrangle.split('.')[0] == 'pandas':
                 # Execute a pandas method
                 # TODO: disallow any hidden methods
                 # TODO: remove parameters, allow selecting in/out columns
                 try:
                     df[params['output']] = getattr(df[params['input']], wrangle.split('.')[1])(**params.get('parameters', {}))
                 except:
@@ -325,34 +341,41 @@
                     # from the parameters or the columns
                     if not fn_argspec.varkw:
                         params_temp2 = params_temp.copy()
                         for param in params_temp2.keys():
                             if param not in fn_argspec.args:
                                 params_temp.pop(param)
 
-                        cols = [
-                            col for col in 
-                            df_temp.columns.to_list()
-                            if col in fn_argspec.args
-                        ]
+                        cols = df_temp.columns.to_list()
+                        cols_renamed = [col.replace(' ', '_') for col in cols]
+
+                        # Create a dictionary of columns with spaces and their replacement
+                        # with an underscore. Used in df_temp.rename
+                        colDict = {
+                            col: col.replace(' ', '_') for col in cols
+                            if (' ' in col and col.replace(' ', '_') in fn_argspec.args)
+                        }
+
+                        df_temp.rename(columns=colDict, inplace=True)
+                        cols_renamed = [col for col in cols_renamed if col in fn_argspec.args]
 
                         # Ensure we don't remove all columns
                         # if user hasn't specified any
-                        if cols:
-                            df_temp = df_temp[cols]
+                        if cols_renamed:
+                            df_temp = df_temp[cols_renamed]
                     
                     # If user specifies multiple outputs, expand any list output
                     # across the columns else return as a single column
                     if isinstance(params['output'], list) and len(params['output']) > 1:
                         result_type = 'expand'
                     else:
                         result_type = 'reduce'
 
                     # {**x, **params_temp} deals with columns in 
-                    # function args and  **params_temp without columns
+                    # function args and **params_temp without columns
                     # There may be no columns in the case that the user
                     # does not specify any columns in their function parameters
                     try:
                         df[params['output']] = df_temp.apply(
                             lambda x: custom_function(**{**x, **params_temp}),
                             axis=1,
                             result_type=result_type
@@ -374,28 +397,96 @@
                 obj = _recipe_wrangles
                 for element in wrangle.split('.'):
                     obj = getattr(obj, element)
 
                 if wrangle == 'recipe':
                     params['functions'] = functions
 
-                # Execute the requested function and return the value
                 df = obj(df, **params)
 
+            # If the user specified a where, we need to merge this back to the original dataframe
+            if 'where' in original_params and wrangle not in no_where_list:
+                if 'output' in params.keys():
+                    # Wrangle explictly defined the output
+                    output_columns = (
+                        params['output']
+                        if isinstance(params['output'], list)
+                        else [params['output']]
+                    )
+                    df = _pandas.merge(
+                        df_original,
+                        df[output_columns],
+                        left_index=True,
+                        right_index=True,
+                        how='left',
+                        suffixes=('_x',None)
+                    )
+                    for output_col in output_columns:
+                        if output_col + '_x' in df.columns:
+                            df = _recipe_wrangles.merge.coalesce(
+                                df,
+                                [output_col, output_col+'_x'],
+                                output_col
+                            )
+                            df.drop([output_col+'_x'], axis = 1, inplace=True)
+                elif list(df.columns) == list(df_original.columns) and 'input' in list(params.keys()):
+                    # Wrangle overwrote the input
+                    output_columns = params['input']
+                    df = _pandas.merge(
+                        df_original,
+                        df[output_columns],
+                        left_index=True,
+                        right_index=True,
+                        how='left',
+                        suffixes=('_x',None)
+                    )
+                    for input_col in params['input']:
+                        if input_col + '_x' in df.columns:
+                            df = _recipe_wrangles.merge.coalesce(
+                                df,
+                                [input_col, input_col+'_x'],
+                                input_col
+                            )
+                            df.drop([input_col+'_x'], axis = 1, inplace=True)
+                elif list(df.columns) != list(df_original.columns):
+                    # Wrangle added columns
+                    output_columns = [col for col in list(df.columns) if col not in list(df_original.columns)]
+                    df = _pandas.merge(
+                        df_original,
+                        df[output_columns],
+                        left_index=True,
+                        right_index=True,
+                        how='left'
+                    )
+
+            # Clean up NaN's
+            df.fillna('', inplace = True)
+            # Run a second pass of df.fillna() in order to fill NaT's (not picked up before) with zeros
+            # Could also use _pandas.api.types.is_datetime64_any_dtype(df) as a check
+            df.fillna('0', inplace = True)
+
     return df
 
 
-def _filter_dataframe(df: _pandas.DataFrame, columns: list = None, not_columns: list = None, where: str = None, **_) -> _pandas.DataFrame:
+def _filter_dataframe(
+    df: _pandas.DataFrame,
+    columns: list = None,
+    not_columns: list = None,
+    where: str = None,
+    where_params: _Union[list, dict] = None, 
+    **_
+) -> _pandas.DataFrame:
     """
     Filter a DataFrame
 
     :param df: Input DataFrame
     :param columns: List of columns to include
     :param not_columns: List of columns to exclude
     :param where: SQL where criteria to filter based on
+    :param params: List of parameters to pass to execute method. The syntax used to pass parameters is database driver dependent.
     """
     # Reduce to user chosen columns
     if columns:
         columns = _wildcard_expansion(df.columns.tolist(), columns)
         df = df[columns]
 
     # Remove any columns specified by the user
@@ -408,15 +499,16 @@
     if where:
         df = _recipe_wrangles.sql(
             df,
             f"""
             SELECT *
             FROM df
             WHERE {where};
-            """
+            """,
+            where_params
         )
 
     return df
 
 
 def _write_data(df: _pandas.DataFrame, recipe: dict, functions: dict = {}) -> _pandas.DataFrame:
     """
@@ -436,15 +528,15 @@
 
     # Loop through all exports, get type and execute appropriate export
     for export in recipe:
         for export_type, params in export.items():
             # Filter the dataframe as requested before passing
             # to the desired write function
             df_temp = _filter_dataframe(df, **params)
-            for key in ['columns', 'not_columns', 'where']:
+            for key in ['columns', 'not_columns', 'where', 'where_params']:
                 if key in params:
                     params.pop(key)
 
             if export_type == 'dataframe':
                 # Define the dataframe that is returned
                 df_return = df_temp
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/convert.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -166,15 +166,20 @@
           results.append(item)
           
       df[out_col] = results
     
     return df
 
 
-def from_json(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None) -> _pd.DataFrame:
+def from_json(
+        df: _pd.DataFrame, 
+        input: _Union[str, list], 
+        output: _Union[str, list] = None,
+        **kwargs
+        ) -> _pd.DataFrame:
     """
     type: object
     description: Convert a JSON representation into an object
     additionalProperties: false
     required:
       - input
     properties:
@@ -198,21 +203,26 @@
     
     # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The lists for input and output must be the same length.')
         
     # Loop through and apply for all columns
     for input_column, output_column in zip(input, output):
-        df[output_column] = [_json.loads(x) for x in df[input_column]]
+        df[output_column] = [_json.loads(x, **kwargs) for x in df[input_column]]
     
     return df
 
 
-def to_json(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None) -> _pd.DataFrame:
-    """
+def to_json(
+        df: _pd.DataFrame, 
+        input: _Union[str, list], 
+        output: _Union[str, list] = None, 
+        **kwargs
+        ) -> _pd.DataFrame:
+    r"""
     type: object
     description: Convert an object to a JSON representation.
     additionalProperties: false
     required:
       - input
     properties:
       input:
@@ -221,24 +231,38 @@
           - array
         description: Name of the input column.
       output:
         type:
           - string
           - array
         description: Name of the output column. If omitted, the input column will be overwritten
+      indent:
+        type:
+          - string
+          - integer
+        description: If indent is a non-negative integer or string, then JSON array elements and object members will be pretty-printed 
+          with that indent level. An indent level of 0, negative, or "" will only insert newlines. None (the default) selects the most 
+          compact representation. Using a positive integer indent indents that many spaces per level. If indent is a string (such as '\t'), 
+          that string is used to indent each level.
+      sort_keys:
+        type: boolean
+        description: If sort_keys is true (default: False), then the output of dictionaries will be sorted by key.
     """
     # Set output column as input if not provided
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
     
     # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The lists for input and output must be the same length.')
         
     # Loop through and apply for all columns
     for input_columns, output_column in zip(input, output):
-        df[output_column] = [_json.dumps(row) for row in df[input_columns].values.tolist()]
+        df[output_column] = [
+            _json.dumps(row, **kwargs) 
+            for row in df[input_columns].values.tolist()
+            ]
         
     return df
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/create.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,20 +59,21 @@
           if bins[-1] == '+':
               bins[-1] = _math.inf
           
           # Dealing with negative infinity. At start of bins list
           if bins[0] == '-':
               bins[0] = -_math.inf
       
+      # Set to string in order to be able to fill NaN values when using where
       df[out_col] = _pd.cut(
           x=df[in_col],
           bins=bins,
           labels=labels,
           **kwargs
-      )
+      ).astype(str)
     
     return df
 
 
 def column(df: _pd.DataFrame, output: _Union[str, list], value = None) -> _pd.DataFrame:
     """
     type: object
@@ -115,14 +116,15 @@
     check_list = [x for x in output if x in existing_column]
     if len(check_list) > 0:
       raise ValueError(f'{check_list} column(s) already exists in the dataFrame') 
     
     for output_column, values_list in zip(output, value):
         # Data to generate
         data = _pd.DataFrame(_generate_cell_values(values_list, rows), columns=[output_column])
+        data.set_index(df.index, inplace=True)  # use the same index as original to match rows
         # Merging existing dataframe with values created
         df = _pd.concat([df, data], axis=1)
 
     return df
 
 
 def guid(df: _pd.DataFrame, output: _Union[str, list]) -> _pd.DataFrame:
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/extract.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         # if one model_id, then use that model for all columns inputs and outputs
         model_id = [model_id[0] for _ in range(len(input))]
         for in_col, out_col, model in zip(input, output, model_id):
             df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element, use_labels=use_labels)
     
     elif len(input) > 1 and len(output) == 1 and len(model_id) == 1:
         # if there are multiple inputs and one output and one model_id. concatenate the inputs
-        df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id, first_element=first_element, use_labels=use_labels)
+        df[output[0]] = _extract.custom(_format.concatenate(df[input].astype(str).values.tolist(), ' '), model_id=model_id[0], first_element=first_element, use_labels=use_labels)
     
     else:
         # Iterate through the inputs, outputs and model_ids
         for in_col, out_col, model in zip(input, output, model_id):
             df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element, use_labels=use_labels)
         
     return df
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/format.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/main.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,32 +150,41 @@
           less_than: _Union[int, float] = None,
           less_than_equal_to: _Union[int, float] = None,
           between: list = None,
           contains: str = None,
           not_contains: str = None,
           is_null: bool = None,
           where: str = None,
+          where_params: _Union[list, dict] = None,
           **kwargs,
           ) -> _pd.DataFrame:
     """
     type: object
-    description: |
+    description: |-
       Filter the dataframe based on the contents.
       If multiple filters are specified, all must be correct.
       For complex filters, use the where parameter.
     additionalProperties: false
     properties:
       where:
         type: string
         description: Use a SQL WHERE clause to filter the data.
+      where_params:
+        type: 
+          - array
+          - dict
+        description: |-
+          Variables to use in conjunctions with where.
+          This allows the query to be parameterized.
+          This uses sqlite syntax (? or :name)
       input:
         type:
           - string
           - array
-        description: |
+        description: |-
           Name of the column to filter on.
           If multiple are provided, all must match the criteria.
       equal:
         type:
           - string
           - array
         description: Select rows where the values equal a given value.
@@ -231,15 +240,16 @@
     if where != None:
         df = sql(
             df,
             f"""
             SELECT *
             FROM df
             WHERE {where};
-            """
+            """,
+            where_params
         )
 
     # If a string provided, convert to list
     if not isinstance(input, list): input = [input]
 
     for input_column in input: 
         if equal != None:
@@ -569,22 +579,21 @@
         
         # Otherwise create a dict from input and output columns
         rename_dict = dict(zip(input, output))
 
     return df.rename(columns=rename_dict)
 
 
-def replace(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list], find: str, replace: str) -> _pd.DataFrame:
+def replace(df: _pd.DataFrame, input: _Union[str, list], find: str, replace: str, output: _Union[str, list] = None) -> _pd.DataFrame:
     """
     type: object
     description: Quick find and replace for simple values. Can use regex in the find field.
     additionalProperties: false
     required:
       - input
-      - output
       - find
       - replace
     properties:
       input:
         type:
           - string
           - array
@@ -609,60 +618,68 @@
     if not isinstance(output, list): output = [output]
 
     # Ensure input and output are equal lengths
     if len(input) != len(output):
         raise ValueError('The lists for input and output must be the same length.')
     
     # Loop through and apply for all columns
-    for input_column, output_column in zip(input, output):  
-        df[output_column] = df[input_column].apply(lambda x: _re.sub(find, replace, x))
-    
+    for input_column, output_column in zip(input, output):
+        df[output_column] = df[input_column].apply(lambda x: _re.sub(str(find), str(replace), str(x)))
+        
     return df
 
 
-def sql(df: _pd.DataFrame, command: str) -> _pd.DataFrame:
+def sql(df: _pd.DataFrame, command: str, params: _Union[list, dict] = None) -> _pd.DataFrame:
     """
     type: object
     description: Apply a SQL command to the current dataframe. Only SELECT statements are supported - the result will be the output.
     additionalProperties: false
     required:
       - command
     properties:
       command:
         type: string
         description: SQL Command. The table is called df. For specific SQL syntax, this uses the SQLite dialect.
+      params:
+        type: 
+          - array
+          - dict
+        description: |-
+          Variables to use in conjunctions with query.
+          This allows the query to be parameterized.
+          This uses sqlite syntax (? or :name)
     """
     if command.strip().split()[0].upper() != 'SELECT':
       raise ValueError('Only SELECT statements are supported for sql wrangles')
 
     # Create an in-memory db with the contents of the current dataframe
     db = _sqlite3.connect(':memory:')
     
     # List of columns changed
     cols_changed = []
     for cols in df.columns:
         count = 0        
         for row in df[cols]:
             # If row contains objects, then convert to json
-            if isinstance(row, dict):
+            if isinstance(row, dict) or isinstance(row, list):
                 # Check if there is an object in the column and record column name to convert to json
                 cols_changed.append(cols)
                 break
             # Only check the first 10 rows of a column
             count += 1
             if count > 10: break
             
         if cols in cols_changed:
             # If the column is in cols_changed then convert to json
             _to_json(df=df, input=cols)
     
     df.to_sql('df', db, if_exists='replace', index = False, method='multi', chunksize=1000)
     
     # Execute the user's query against the database and return the results
-    df = _pd.read_sql(command, db)
+    df = _pd.read_sql(command, db, params = params)
     db.close()
     
     # Change the columns back to an object
     for new_cols in df.columns:
         
         if new_cols in cols_changed:
             # If the column is in cols changed, then change back to an object
@@ -690,22 +707,14 @@
           - array
         description: Name or list of output columns
       model_id:
         type:
           - string
           - array
         description: The ID of the wrangle to use (do not include 'find' and 'replace')
-      find:
-        type:
-          - string
-        description: Pattern to find using regex (do not include model_id)
-      replace:
-        type:
-          - string
-        description: Value to replace the pattern found (do not include model_id)
     """
     # If user hasn't specified an output column, overwrite the input
     if output is None: output = input
 
     # If user provides a single string, convert all the arguments to lists for consistency
     if isinstance(input, str): input = [input]
     if isinstance(output, str): output = [output]
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/merge.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/merge.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/pandas.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/pandas.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/select.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/select.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 
 
 def dictionary_element(
     df: _pd.DataFrame,
     input: _Union[str, list],
     element: str,
     output: _Union[str, list] = None,
-    default = ''
+    default: any = ''
 ) -> _pd.DataFrame:
     """
     type: object
     description: Select a named element of a dictionary.
     additionalProperties: false
     required:
       - input
-      - output
       - element
     properties:
       input:
         type: 
           - string
           - array
         description: Name of the input column
@@ -32,14 +31,21 @@
           - string
           - array
         description: Name of the output column
       element:
         type: string
         description: The key from the dictionary to select.
       default:
+        type: 
+          - string
+          - number
+          - array
+          - object
+          - boolean
+          - 'null'
         description: Set the default value to return if the specified element doesn't exist.
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
@@ -114,22 +120,21 @@
     # Loop through and get left characters of the length requested for all columns
     for input_column, output_column in zip(input, output):
         df[output_column] = df[input_column].str[:length]
 
     return df
 
 
-def list_element(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None, element: int = 0, default = '') -> _pd.DataFrame:
+def list_element(df: _pd.DataFrame, input: _Union[str, list], output: _Union[str, list] = None, element: int = 0, default: any = '') -> _pd.DataFrame:
     """
     type: object
     description: Select a numbered element of a list (zero indexed).
     additionalProperties: false
     required:
       - input
-      - output
       - element
     properties:
       input:
         type: 
           - string
           - array
         description: Name of the input column
@@ -138,14 +143,21 @@
           - string
           - array
         description: Name of the output column
       element:
         type: integer
         description: The numbered element of the list to select. Starts from zero
       default:
+        type:
+          - string
+          - number
+          - array
+          - object
+          - boolean
+          - 'null'
         description: Set the default value to return if the specified element doesn't exist.
     """
     if output is None: output = input
     
     # Ensure input and outputs are lists
     if not isinstance(input, list): input = [input]
     if not isinstance(output, list): output = [output]
```

### Comparing `wrangles-1.3.1/wrangles/recipe_wrangles/split.py` & `wrangles-1.4.0/wrangles/recipe_wrangles/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,18 @@
     """ 
     # storing data as df temp to prevent the original data to be changed
     df_temp = df[input]
     try:
         df_temp = [_json.loads('{}') if x == '' else _json.loads(x) for x in df_temp]
     except:
         df_temp = [{} if x == None else x for x in df[input]]
-            
-    exploded_df = _pd.json_normalize(df_temp, max_level=1).fillna('')
+
+    exploded_df = _pd.json_normalize(df_temp, max_level=0).fillna('')
+    exploded_df.set_index(df.index, inplace=True)  # Restore index to ensure rows match
+
     df[exploded_df.columns] = exploded_df
     return df
 
     
 def list(df: _pd.DataFrame, input: str, output: _Union[str, list]) -> _pd.DataFrame:
     """
     type: object
```

### Comparing `wrangles-1.3.1/wrangles/select.py` & `wrangles-1.4.0/wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/standardize.py` & `wrangles-1.4.0/wrangles/standardize.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,14 @@
     # If model_id format is correct but no mode_id exists
     if model_properties.get('message', None) == 'error': raise ValueError('Incorrect model_id.\nmodel_id may be wrong or does not exists')
     batch_size = model_properties['batch_size'] or 10000
     
     # Using model_id in wrong function
     purpose = model_properties['purpose']
     if purpose != 'standardize':
-        raise ValueError(f'Using {purpose} model_id in a standardize function.')
+        raise ValueError(f'Using {purpose} model_id {model_id} in a standardize function.')
 
     results = _batching.batch_api_calls(url, params, json_data, batch_size)
 
     if isinstance(input, str): results = results[0]
     
     return results
```

### Comparing `wrangles-1.3.1/wrangles/train.py` & `wrangles-1.4.0/wrangles/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.3.1/wrangles/translate.py` & `wrangles-1.4.0/wrangles/translate.py`

 * *Files identical despite different names*

